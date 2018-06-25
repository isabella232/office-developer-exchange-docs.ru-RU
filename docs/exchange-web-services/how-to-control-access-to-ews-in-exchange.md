---
title: Управление доступом к веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Узнайте, как для управления доступом к веб-служб Exchange для пользователей, приложений или во всей организации.
ms.openlocfilehash: 956c28faba105ecf2a6b1452abe629ea2fc930e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760986"
---
# <a name="control-access-to-ews-in-exchange"></a>Управление доступом к веб-служб Exchange в Exchange

Узнайте, как для управления доступом к веб-служб Exchange для пользователей, приложений или во всей организации.
  
Используется ли управляемый API EWS или веб-служб Exchange напрямую, в приложении, можно управлять доступом для веб-служб Exchange (EWS). Если имеется доступ с правами администратора на сервере Exchange, доступ к веб-служб Exchange можно управлять с помощью командной консоли Exchange для управления доступом к глобально, для каждого пользователя и для каждого приложения.
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a>Командлеты командной консоли Exchange для настройки управления доступом
<a name="bk_Cmdlets"> </a>

Можно использовать следующие командлеты командной консоли Exchange для просмотра текущих настроек доступа и задания элементов управления доступа к веб-служб Exchange:
  
- [Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) - показано, какие параметры настраиваются для определенного почтового ящика.   
- [Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) - наборов параметров для определенного почтового ящика.    
- [Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) - указываются параметры для всей организации.    
- [Set-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx) - задает параметры для всей организации. 

<a name="bk_Examples"> </a>

## <a name="examples-controlling-access-to-ews"></a>Примеры: Управление доступом к веб-служб Exchange

Давайте рассмотрим несколько сценариев, которые показывают, как контролировать доступ к приложению.
  
**В таблице 1. Команды для управления доступом к веб-служб Exchange**

|Назначение |Используйте следующую команду|
|:-----|:-----|
|Блокировать все клиентские приложения с помощью веб-служб Exchange. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/>Это позволяет приложений, перечисленных в AllowList для подключения. В этом примере приложения не включены в AllowList, поэтому приложения не могут использовать веб-служб Exchange. |
|Разрешить список клиентских приложений для использования веб-служб Exchange. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/>Это позволяет определенные приложения для использования веб-служб Exchange. В этом примере любого приложения, которое имеет строка агента пользователя начинается с «OWA /» разрешения на доступ. |
|Разрешить все клиентские приложения для использования веб-служб Exchange, за исключением тех, которые были заблокированы. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/>В этом примере блокирует только приложений с помощью веб-служб Exchange, для которого строка агента пользователя, который начинается с «OWA /». |
|Разрешить все клиентские приложения для использования веб-служб Exchange. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> Так как нет блокировки не указан, то все приложения могут использовать веб-служб Exchange. |
|Блокировка во всей организации с помощью веб-служб Exchange. | `Set-OrganizationConfig -EwsEnabled:$false` |
|Разрешить во всей организации, для использования веб-служб Exchange. | `Set-OrganizationConfig -EwsEnabled:$true`|
|Блокировка отдельных почтовых ящиков с помощью веб-служб Exchange. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|Разрешить отдельным почтовым ящикам для использования веб-служб Exchange. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a>См. также

- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)    
- [Управление доступом к клиентского приложения для веб-служб Exchange в Exchange](controlling-client-application-access-to-ews-in-exchange.md)   
- [Exchange Server PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

