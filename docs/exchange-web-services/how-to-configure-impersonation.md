---
title: Настройка олицетворения
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: Сведения о предоставлении роли олицетворения учетной записи службы с помощью командной консоли Exchange.
ms.openlocfilehash: 57ccef48a7553bcc06e3b3ae940b376b8555ef84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760991"
---
# <a name="configure-impersonation"></a>Настройка олицетворения

Сведения о предоставлении роли олицетворения учетной записи службы с помощью командной консоли Exchange. 
  
С помощью олицетворения вызывающая сторона, например приложение службы, может олицетворять учетную запись пользователя. Вызывающая сторона может выполнять операции, используя вместо разрешений своей учетной записи те, которые сопоставлены с олицетворенной учетной записью.
  
Для назначения разрешений учетным записям в Exchange Online (автономной службе и в составе Office 365) и всех версиях Exchange, начиная с Exchange 2013, используется управление доступом на основе ролей (RBAC). Чтобы учетная запись службы могла олицетворять других пользователей, администратору сервера Exchange Server потребуется предоставить ей роль **ApplicationImpersonation** с помощью командлета [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx). 
  
## <a name="configuring-the-applicationimpersonation-role"></a>Настройка роли ApplicationImpersonation

Вам или администратору сервера Exchange Server следует использовать указанные ниже параметры командлета **New-ManagementRoleAssignment** при назначении роли **ApplicationImpersonation**. 
  
-  _Name_ &ndash; — понятное имя назначения роли. При каждом назначении роли запись о ней вносится в список ролей RBAC. Используйте командлет [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx), чтобы проверить назначения ролей. 
    
-  _Role_ &ndash; — роль RBAC, которую нужно назначить. Для настройки олицетворения нужно назначить роль **ApplicationImpersonation**. 
    
-  _User_ &ndash; — учетная запись службы. 
    
-  _CustomRecipientScope_ &ndash; — область пользователей, которых может олицетворять учетная запись службы. Учетная запись службы может олицетворять только тех пользователей, которые входят в указанную область. Если область не указана, учетная запись службы получает роль **ApplicationImpersonation** для всех пользователей организации. Можно создавать специальные области управления с помощью командлета [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx). 
    
Перед настройкой олицетворения вам понадобятся:
  
- Учетные данные администратора для сервера Exchange Server.
    
- Учетные данные администратора домена или другие учетные данные с разрешением на создание и назначение ролей и областей.
    
- Средства управления Exchange. Их нужно установить на компьютере, с которого будут выполняться команды.
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a>Настройка олицетворения для всех пользователей в организации

1. Запустите командную консоль Exchange. В меню "Пуск" выберите **Все приложения** >  > **Microsoft Exchange Server 2013**. 
    
2. Запустите командлет **New-ManagementRoleAssignment**, чтобы добавить разрешение на олицетворение для указанного пользователя. В приведенном ниже примере показано, как настроить олицетворение так, чтобы учетная запись службы могла олицетворять всех остальных пользователей в организации. 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a>Настройка олицетворения для определенных пользователей или групп пользователей

1. Запустите командную консоль Exchange. В меню "Пуск" выберите **Все приложения** >  > **Microsoft Exchange Server 2013**. 
    
2. Запустите командлет **New-ManagementScope**, чтобы создать область, которой можно назначить роль олицетворения. Если такая область уже есть, этот шаг можно пропустить. В приведенном ниже примере показано, как создать область управления для определенной группы. 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   Параметр _RecipientRestrictionFilter_ командлета**New-ManagementScope** определяет участников области. Можно использовать свойства объекта **Identity**, чтобы создать фильтр. В примере ниже показан фильтр, который ограничивает результаты одним пользователем с именем "john". 
    
   ```powershell
   Name -eq "john"
   ```

3. Запустите командлет **New-ManagementRoleAssignment**, чтобы добавить разрешение на олицетворение пользователей, входящих в указанную область. В приведенном ниже примере показано, как настроить учетную запись службы так, чтобы она могла олицетворять всех пользователей в области. 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


Когда администратор предоставит разрешения на олицетворение, с помощью учетной записи службы можно будет вызывать учетные записи других пользователей. Используйте командлет [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx), чтобы проверить назначения ролей. 
  
## <a name="see-also"></a>См. также

- [Олицетворение и EWS в Exchange](impersonation-and-ews-in-exchange.md)
- [Роль ApplicationImpersonation](http://technet.microsoft.com/ru-RU/library/dd776119%28v=exchg.150%29.aspx)   
- [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

