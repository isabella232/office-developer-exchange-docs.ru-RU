---
title: Операция GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: Операция GetEvents используется клиентами подписки пула для запроса уведомлений с сервера клиентского доступа. Ответ GetEvents операция возвращает массив элементов и события, которые происходили в почтовом ящике с момента последнего уведомления.
ms.openlocfilehash: 1a23a9d570a4554e54becb7927f25dff89888c74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762763"
---
# <a name="getevents-operation"></a>Операция GetEvents

Операция **GetEvents** используется клиентами подписки пула для запроса уведомлений с сервера клиентского доступа. Ответ **GetEvents** операция возвращает массив элементов и события, которые происходили в почтовом ящике с момента последнего уведомления. 
  
> [!IMPORTANT]
> Операция **DeleteUserConfiguration** , будет вызвано событие перемещения по системе события уведомления. Объект конфигурации пользователя перемещается в корзину. 
  
## <a name="remarks"></a>Замечания

Изменения элементов календаря может привести к созданию несколько событий. Эти события основаны на результатах временные элементов, создаются в почтовом ящике изменяемый как часть обычных операций календаря или оба элементов хранения данных о доступности. События для элемента класса «IPM. SchedulePlus.FreeBusy.BinaryData» должны пропускаться клиентов веб-служб. Эти временные элементы удаляются после их создания; Таким образом при попытке извлечь эти элементы ошибка будут возвращены, о том, что элемент не найден.
  
## <a name="getevents-request-example"></a>Пример запроса GetEvents

### <a name="description"></a>Описание

Следующем примере показано, как запросить событий и элементы, связанные с подпиской, который идентифицируется средством идентификатор подписки и водяного знака.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a>Элементы запроса GetEvents

В запросе используются следующие элементы:
  
- [GetEvents](getevents.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Водяной знак](watermark.md)
    
## <a name="successful-getevents-response-example"></a>Пример успешного ответа GetEvents

### <a name="description"></a>Описание

В следующем примере ответа показано уведомление об существование двух новых почтовых сообщений с момента последнего уведомления запрос был отправлен на сервер.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:PreviousWatermark>AAAAAMAGAAAAAAAAAQ==</t:PreviousWatermark>
            <t:MoreEvents>false</t:MoreEvents>
            <t:NewMailEvent>
              <t:Watermark>AAAAAM4GAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T00:36:29Z</t:TimeStamp>
              <t:ItemId Id="AQApAHR" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:NewMailEvent>
              <t:Watermark>AAAAAOQGAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T01:00:50Z</t:TimeStamp>
              <t:ItemId Id="AQApAHRw" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
          </m:Notification>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

> [!NOTE]
> Идентификаторы элементов и папок URL-были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="getevents-response-elements"></a>Элементы GetEvents ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetEventsResponse](geteventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetEventsResponseMessage](geteventsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Уведомление](notification-ex15websvcsotherref.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [PreviousWatermark](previouswatermark.md)
    
- [MoreEvents](moreevents.md)
    
- [NewMailEvent](newmailevent.md)
    
- [Водяной знак](watermark.md)
    
- [Метка времени](timestamp.md)
    
- [Идентификатор элемента](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
Чтобы найти другие параметры в сообщении ответа **GetEvents** операции, изучите иерархия схемы. Запустите на элементе [уведомлений](notification-ex15websvcsotherref.md) . 
  
## <a name="getevents-error-response-example"></a>Пример ответа об ошибке GetEvents

### <a name="description"></a>Описание

В следующем примере показано возврату ошибки **GetEvents** запрос. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Error">
          <m:MessageText>Access is denied. Only the subscription owner may access the subscription.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionAccessDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a>Замечания

При обработке запроса **GetEvents** сервера клиентского доступа необходимо выполнить следующие действия: 
  
1. SubscriptionID запрос подтверждения действительную подписку, размещенного на сервере клиентского доступа. Если он не установлен, **GetEvents** завершается неудачно. 
    
2. SMTP-адрес пользователя, прошедшего проверку подлинности для запроса сравнивается с SMTP-адрес пользователя, создавшего подписку. Если они не совпадают, происходит сбой запроса **GetEvents** . 
    
3. Очередь подписки будет опрошен на наличие событий, ожидающих отправляются клиенту. Если очередь не является пустым, первые 50 события из очереди, которые извлекаются из очереди и кодируются в уведомление.
    
4. Если события не обнаружены в очереди, StatusEvent создан и кодируются в ответ уведомлений.
    
5. Уведомление ответ возвращается клиенту.
    
6. События, включенные в уведомлении, удаляются из очереди подписки, клиентского доступа сервера локальной последний водяной знак для подписки на задано значение водяной знак последнего события, который возвращается.
    
7. Сброс таймера времени ожидания для подписки.
    
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Отписаться операции](unsubscribe-operation.md)


[С помощью подписки по запросу](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

