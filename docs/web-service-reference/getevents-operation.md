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
description: Операция Events используется клиентами подписки по запросу для запроса уведомлений с сервера клиентского доступа. Ответ операции Events возвращает массив элементов и событий, произошедших в почтовом ящике с момента последнего уведомления.
ms.openlocfilehash: 9258fd003c242911866aa7abbca5eba2b9582223
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462516"
---
# <a name="getevents-operation"></a>Операция GetEvents

Операция **Events** используется клиентами подписки по запросу для запроса уведомлений с сервера клиентского доступа. Ответ операции **Events** возвращает массив элементов и событий, произошедших в почтовом ящике с момента последнего уведомления. 
  
> [!IMPORTANT]
> Операция **DeleteUserConfiguration** инициирует событие Move для системы уведомления о событиях. Объект конфигурации пользователя будет перемещен в корзину. 
  
## <a name="remarks"></a>Примечания

Изменения элементов календаря могут привести к созданию нескольких событий. Эти события являются результатом того, что временные элементы создаются в почтовом ящике, элементы хранения данных о занятости изменяются в рамках обычных операций календаря или и то, и другое. События для класса элемента "IPM. Счедулеплус. FreeBusy. Бинаридата должен игнорироваться клиентами веб-служб. Эти временные элементы удаляются после их создания; Таким образом, при попытке получить эти элементы возвращается ошибка, указывающая на то, что элемент не найден.
  
## <a name="getevents-request-example"></a>Пример запроса на получение событий

### <a name="description"></a>Описание

В приведенном ниже примере показано, как запросить события и элементы, связанные с подпиской, которая определяется идентификатором подписки и водяным знаком.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a>Элементы запроса Events

В запросе используются следующие элементы:
  
- [GetEvents](getevents.md)
    
- [SubscriptionId (Events)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="successful-getevents-response-example"></a>Пример успешных откликов на события

### <a name="description"></a>Описание

В приведенном ниже примере ответа показано уведомление о существовании двух новых почтовых сообщений с момента отправки последнего запроса уведомления на сервер.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
> Идентификаторы элементов и папок были сокращены для сохранения удобочитаемости. 
  
### <a name="getevents-response-elements"></a>Элементы ответа на события

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [жетевентсреспонсе](geteventsresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [жетевентсреспонсемессаже](geteventsresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Уведомление](notification-ex15websvcsotherref.md)
    
- [SubscriptionId (Events)](subscriptionid-getevents.md)
    
- [превиаусватермарк](previouswatermark.md)
    
- [моривентс](moreevents.md)
    
- [невмаилевент](newmailevent.md)
    
- [Watermark](watermark.md)
    
- [Метка времени](timestamp.md)
    
- [Идентификатор](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
Чтобы найти другие параметры ответного сообщения **для операции GetResponse** , изучите иерархию схемы. Начните с элемента [уведомления](notification-ex15websvcsotherref.md) . 
  
## <a name="getevents-error-response-example"></a>Пример ответа на сообщение об ошибке при возникновении событий

### <a name="description"></a>Описание

В приведенном ниже примере показан ответ об ошибке запроса на получение **событий** . 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="remarks"></a>Примечания

При обработке запроса по **событиям** сервер клиентского доступа выполняет следующие действия: 
  
1. Значение SubscriptionID для запроса подтверждено допустимой подпиской, размещенной на сервере клиентского доступа. В противном случае произойдет сбой вызова метода **Events** . 
    
2. SMTP-адрес пользователя, прошедшего проверку подлинности для запроса, сравнивается с SMTP-адресом пользователя, создавшего подписку. Если они не совпадают, происходит сбой запроса **Events** . 
    
3. Очередь подписки запрашивает события, ожидающие отправки клиенту. Если очередь не пустая, первые 50 событий из очереди извлекаются из очереди и кодируются в уведомление.
    
4. Если в очереди не найдено ни одного события, создается Статусевент и кодируется в ответ на уведомление.
    
5. Ответ на уведомление возвращается клиенту.
    
6. События, включенные в уведомление, удаляются из очереди подписки, а последний водяной знак сервера клиентского доступа для подписки задается водяным знаком последнего возвращаемого события.
    
7. Таймер времени ожидания для подписки сбрасывается.
    
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)


[Использование подписок по запросу](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

