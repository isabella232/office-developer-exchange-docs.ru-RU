---
title: Контроль доступа к EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Узнайте, как управлять доступом к EWS для пользователей, приложений или всей Организации.
localization_priority: Priority
ms.openlocfilehash: bd65b099ab15c1514945d8a1cfa4e9b1428a4755
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456880"
---
# <a name="control-access-to-ews-in-exchange"></a>Контроль доступа к EWS в Exchange

Узнайте, как управлять доступом к EWS для пользователей, приложений или всей Организации.
  
Независимо от того, используется ли управляемый API EWS или веб-сайт EWS напрямую, вы можете управлять доступом к веб-службам Exchange (EWS). Если вы обладаете правами администратора на доступ к серверу Exchange Server, вы можете управлять доступом к EWS, используя командную консоль Exchange для глобального управления доступом, для каждого пользователя и для каждого приложения.
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a>Командлеты командной консоли Exchange для настройки управления доступом
<a name="bk_Cmdlets"> </a>

Вы можете использовать следующие командлеты командной консоли Exchange для просмотра текущей конфигурации доступа и задания средств контроля доступа EWS:
  
- [Get – CASMailbox](https://technet.microsoft.com/library/bb124754.aspx) — показывает, какие параметры задаются для определенного почтового ящика.   
- [Set – CASMailbox](https://technet.microsoft.com/library/bb125264.aspx) — задает параметры для определенного почтового ящика.    
- [Get – OrganizationConfig](https://technet.microsoft.com/library/aa997571.aspx) — показывает параметры для всей Организации.    
- [Set – OrganizationConfig](https://technet.microsoft.com/library/aa997443.aspx) — задает параметры для всей Организации. 

<a name="bk_Examples"> </a>

## <a name="examples-controlling-access-to-ews"></a>Примеры: Управление доступом к EWS

Рассмотрим несколько сценариев, показывающих, как можно управлять доступом к приложению.
  
**Таблица 1. Команды для управления доступом к EWS**

|Задача |Используйте эту команду|
|:-----|:-----|
|Блокировать использование EWS всеми клиентскими приложениями. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/>Это позволяет приложениям, перечисленным в Алловлист, подключаться. В этом примере приложения не включены в Алловлист, поэтому приложения не могут использовать EWS. |
|Разрешить списку клиентских приложений использовать EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/>Это позволяет определенным приложениям использовать EWS. В этом примере доступ к приложению, имеющему строку агента пользователя, начинающуюся с "OWA/", разрешено. |
|Разрешите всем клиентским приложениям использовать EWS, кроме специально заблокированных. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/>В этом примере приложения не могут использовать веб-служб EWS, у которых есть строка агента пользователя, начинающаяся с "OWA/". |
|Разрешите всем клиентским приложениям использовать EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> Так как Блокклист не указан, все приложения могут использовать EWS. |
|Блокировать использование EWS всей Организацией. | `Set-OrganizationConfig -EwsEnabled:$false` |
|Разрешите всей Организации использовать EWS. | `Set-OrganizationConfig -EwsEnabled:$true`|
|Блокировка отдельного почтового ящика с помощью EWS. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|Разрешить отдельному почтовому ящику использовать EWS. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a>См. также

- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)    
- [Управление доступом клиентских приложений к EWS в Exchange](controlling-client-application-access-to-ews-in-exchange.md)   
- [PowerShell в Exchange Server (Командная консоль Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

