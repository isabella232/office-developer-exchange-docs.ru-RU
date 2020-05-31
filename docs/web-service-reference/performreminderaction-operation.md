---
title: Операция PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Поиск сведений о PerformReminderActionной операции EWS.
ms.openlocfilehash: 778fbb508413721f58cfcf9143a5296874e6cd1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834722"
---
# <a name="performreminderaction-operation"></a>Операция PerformReminderAction

Поиск сведений о **PerformReminderActionной** операции EWS. 
  
Операция **PerformReminderAction** веб-служб Exchange (EWS) запускает действие отклонить или отложить отложить напоминание. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-performreminderaction-operation"></a>Использование операции PerformReminderAction

Вы можете использовать операцию **PerformReminderAction** , чтобы отклонить или отложить напоминания, возвращенные операцией- [напоминаний](getreminders-operation.md) . Чтобы отложить напоминание, установите для [объекта, который следует](actiontype-reminderactiontype.md) **отложить**, и задайте для параметра [Невреминдертиме](newremindertime.md) значение времени позже текущего [ReminderTime](remindertime.md), в противном случае **невреминдертиме** игнорируется сервером. Если напоминание относится к экземпляру повторяющегося собрания, а действие " **отложить** " выполняется в памятке с **невреминдертиме** , которое пройдет за сообщение о следующем повторении, то напоминание отменяется. 
  
Чтобы отклонить напоминание, задайте для **параметра "объект" значение "** **отклонено**". Когда сервер обрабатывает запрос, сервер изменяет значение параметра [напоминания](isreminderset.md) для элемента с **true** на **false**.
  
### <a name="performreminderaction-operation-soap-headers"></a>Заголовки SOAP операции PerformReminderAction

Операция **PerformReminderAction** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a>Пример запроса операции PerformReminderAction

В следующем примере запроса операции **PerformReminderAction** показано, как отложить текущее напоминание и задать новое время оповещения. Обратите внимание, что необходимо включить **чанжекэй** для элемента [ItemId](itemid.md) , а для параметра **невреминдертиме** необходимо задать время позже, чем **ReminderTime** [, возвращенное операцией](getreminders-operation.md) . 
  
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
> Значение **ItemId** было сокращено, чтобы сохранить удобочитаемость. 
  
Текст SOAP Request содержит следующие элементы:
  
- [PerformReminderAction](performreminderaction.md)
    
- [реминдеритемактионс](reminderitemactions.md)
    
- [реминдеритемактион](reminderitemaction.md)
    
- [ActionType](actiontype-reminderactiontype.md)
    
- [Идентификатор](itemid.md)
    
- [невреминдертиме](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a>Успешный отклик операции PerformReminderAction

В следующем примере показан успешный ответ на запрос операции **PerformReminderAction** . Элемент **упдатедитемидс** содержит **итемидс** обновленного элемента календаря. 
  
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

Тело SOAP отклика содержит следующие элементы:
  
- [перформреминдерактионреспонсе](performreminderactionresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [упдатедитемидс](updateditemids.md)
    
- [Идентификатор](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a>Пример ответа на сообщение об ошибке операции PerformReminderAction

В следующем примере показан ответ на запрос операции **PerformReminderAction** , если на сервере не было внесено никаких изменений. Это ответ, в котором был отправлен запрос, но не было возвращено ни одного **упдатедитемидс** , что означает, что напоминания не были изменены. 
  
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

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [перформреминдерактионреспонсе](performreminderactionresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [упдатедитемидс](updateditemids.md)
    
Дополнительные коды ошибок, являющиеся общими для EWS, можно найти в статье [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также


- [Операция GetReminders](getreminders-operation.md)
    

