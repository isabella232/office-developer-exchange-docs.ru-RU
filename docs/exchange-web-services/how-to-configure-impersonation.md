---
title: Настройка олицетворения
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: 'Сведения о предоставлении роли олицетворения учетной записи службы с помощью командной консоли Exchange. '
ms.openlocfilehash: 57ccef48a7553bcc06e3b3ae940b376b8555ef84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760991"
---
# <a name="configure-impersonation"></a>Настройка олицетворения

Сведения о предоставлении роли олицетворения учетной записи службы с помощью командной консоли Exchange.  
  
Олицетворение позволяет вызывающего абонента, такие как приложения-службы, чтобы олицетворять учетную запись пользователя. Звонящий операции можно выполнить с помощью разрешений, которые связаны с олицетворенным учетной записи вместо разрешения, связанные с учетной записью вызывающего абонента.
  
Exchange Online, Exchange Online как часть Office 365 и версии Exchange, начиная с Exchange 2013 использование управления доступом на основе ролей (RBAC) для назначения разрешений учетным записям. Администратор сервера Exchange, необходимо предоставить роль **ApplicationImpersonation** любой учетной записи службы, которая будет олицетворения другим пользователям с помощью командлета [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) . 
  
## <a name="configuring-the-applicationimpersonation-role"></a>Настройка роли ApplicationImpersonation

Когда пользователь или администратор сервера обменника присваивает роль **ApplicationImpersonation** , используйте следующие параметры командлета **New-ManagementRoleAssignment** : 
  
-  _Имя_ &ndash; Понятное имя назначения роли. Каждый раз, когда нужно назначить роль, записываются в списке роли RBAC. Вы можете проверить назначения ролей с помощью командлета [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) . 
    
-  _Роль_ &ndash; Роль RBAC для назначения. При настройке олицетворения нужно назначить роль **ApplicationImpersonation** . 
    
-  _Пользователь_ &ndash; Учетной записи службы. 
    
-  _CustomRecipientScope_ &ndash; Область пользователей, которые могут олицетворять учетную запись службы. Учетная запись службы будет разрешено только для олицетворения другим пользователям в пределах указанной области. Если диапазон не указан, учетную запись службы предоставляется роль **ApplicationImpersonation** по всем пользователям в организации. Можно создавать настраиваемые области управления с помощью командлета [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) . 
    
Перед настройкой олицетворения вам понадобятся:
  
- Учетные данные администратора для сервера Exchange Server.
    
- Учетные данные администратора домена или другие учетные данные с разрешением на создание и назначение ролей и областей.
    
- Средства управления Exchange. Их нужно установить на компьютере, с которого будут выполняться команды.
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a>Настройка олицетворения для всех пользователей в организации

1. Откройте консоль управления Exchange. В меню Пуск выберите **Все программы** > **Microsoft Exchange Server 2013**. 
    
2. Выполните командлет **New-ManagementRoleAssignment** , чтобы добавить разрешение олицетворения для указанного пользователя. Приведенный ниже показано, как настроить олицетворения для включения учетной записи службы для олицетворения всех пользователей в организации. 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a>Настройка олицетворения для определенных пользователей или групп пользователей

1. Откройте консоль управления Exchange. В меню Пуск выберите **Все программы** > **Microsoft Exchange Server 2013**. 
    
2. Выполните командлет **New-ManagementScope** , чтобы создать область, к которому можно назначить роль олицетворения. Если существующей области, этот шаг можно пропустить. Приведенный ниже показано, как создавать области управления для конкретной группы. 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   Параметр _RecipientRestrictionFilter_ командлет **New-ManagementScope** определяет элементы из области действия. Можно использовать свойства объекта **удостоверения** для создания фильтра. В следующем примере представлен фильтр, который ограничивает результатов отдельному пользователю с именем пользователя «john.» 
    
   ```powershell
   Name -eq "john"
   ```

3. Выполните командлет **New-ManagementRoleAssignment** , чтобы добавить разрешением для олицетворения члены указанной области. Приведенный ниже показано, как настроить учетную запись службы для олицетворения всех пользователей в области. 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


После администратор предоставляет разрешений на олицетворение, можно использовать учетную запись службы для совершать звонки от учетные записи других пользователей. Вы можете проверить назначения ролей с помощью командлета [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) . 
  
## <a name="see-also"></a>См. также

- [Олицетворение и EWS в Exchange](impersonation-and-ews-in-exchange.md)
- [Роль ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)   
- [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

