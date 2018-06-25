---
title: Операция PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Найдите сведения о веб-служб Exchange PerformReminderAction операции.
ms.openlocfilehash: 778fbb508413721f58cfcf9143a5296874e6cd1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834722"
---
# <a name="performreminderaction-operation"></a>Операция PerformReminderAction

Найдите сведения о **PerformReminderAction** операции веб-служб Exchange. 
  
Операции веб-служб Exchange (EWS) **PerformReminderAction** инициирует действие прекратить или отложить на оповещение. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-performreminderaction-operation"></a>С помощью операции PerformReminderAction

Чтобы закрыть или отложить напоминания (задержка), возвращенные операцией [GetReminders](getreminders-operation.md) можно использовать операцию **PerformReminderAction** . Чтобы отложить напоминание, установите [Тип действия](actiontype-reminderactiontype.md) в **отложить**и задайте [NewReminderTime](newremindertime.md) значение времени в более поздней версии, чем текущий [ReminderTime](remindertime.md)в противном случае **NewReminderTime** игнорируется сервером. Если оповещение — это вхождение повторяющееся собрание и **отложить** действий на напоминание с **NewReminderTime** , находящегося за напоминание следующее вхождение, напоминания эффективно закрывается. 
  
Чтобы отключить напоминание, задайте значение **Прекратить** **Тип действия** . Когда сервер обрабатывает запрос, сервер изменяется значение [IsReminderSet](isreminderset.md) для элемента с **значение True,** значение **False**.
  
### <a name="performreminderaction-operation-soap-headers"></a>Заголовки SOAP PerformReminderAction операции

Операция **PerformReminderAction** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении. Этот заголовок можно применять к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику. Этот заголовок можно применять к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Этот заголовок можно применять к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a>Пример запроса PerformReminderAction операции

В следующем примере запрос операции **PerformReminderAction** показано, как отложить текущего напоминание и задать новый время оповещения. Обратите внимание на то, что вам нужно включить **ChangeKey** для [ItemId](itemid.md) и **NewReminderTime** должен иметь значение времени в более поздней версии, чем **ReminderTime** , возвращенные операцией [GetReminders](getreminders-operation.md) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:PerformReminderAction>
      <m:ReminderItemActions>
        <t:ReminderItemAction>
          <t:ActionType>Snooze</t:ActionType>
          <t:ItemId Id="vwAAAA=="
           ChangeKey="DwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAUDA=="/>
          <t:NewReminderTime>2014-04-16T17:00:00Z</t:NewReminderTime>
        </t:ReminderItemAction>
      </m:ReminderItemActions>
    </m:PerformReminderAction>
  </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> Значение **ItemId** был усечен, чтобы сохранить удобочитаемость. 
  
Запрос SOAP body содержит следующие элементы:
  
- [PerformReminderAction](performreminderaction.md)
    
- [ReminderItemActions](reminderitemactions.md)
    
- [ReminderItemAction](reminderitemaction.md)
    
- [Тип действия](actiontype-reminderactiontype.md)
    
- [Идентификатор элемента](itemid.md)
    
- [NewReminderTime](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a>Успешные операции ответа PerformReminderAction

В следующем примере показано успешного ответа на запрос операции **PerformReminderAction** . Элемент **UpdatedItemIds** содержит **что ItemID** элемента обновленные календаря. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

Ответ SOAP body содержит следующие элементы:
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
- [Идентификатор элемента](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a>Пример ответа об ошибке PerformReminderAction операции

В следующем примере показано ответа на запрос операции **PerformReminderAction** , когда не изменений на сервере. Это ответ был отправлен запрос, но не **UpdatedItemIds** не возвращено, что означает, что нет напоминаний были изменены. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

Ошибка ответ SOAP body содержит следующие элементы:
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
Дополнительные коды ошибок, которые являются общими для веб-служб Exchange в разделе [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>См. также


- [Операция GetReminders](getreminders-operation.md)
    

