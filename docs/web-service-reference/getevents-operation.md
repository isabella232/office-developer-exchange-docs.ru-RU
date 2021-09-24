---
title: Операция GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetEvents
api_type:
- schema
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: Операция GetEvents используется клиентами подписки для запроса уведомлений с сервера клиентского доступа. Ответ на операцию GetEvents возвращает массив элементов и событий, произошедших в почтовом ящике с момента последнего уведомления.
ms.openlocfilehash: 72d99a654921794115d56d28327a39a21c9ea378
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511602"
---
# <a name="getevents-operation"></a>Операция GetEvents

Операция **GetEvents** используется клиентами подписки для запроса уведомлений с сервера клиентского доступа. Ответ **на операцию GetEvents** возвращает массив элементов и событий, произошедших в почтовом ящике с момента последнего уведомления. 
  
> [!IMPORTANT]
> Операция **DeleteUserConfiguration** вызовет событие перемещения для системы уведомлений о событиях. Объект конфигурации пользователя будет перемещен в контейнер. 
  
## <a name="notes"></a>Примечания.

Изменения элементов Calendar могут привести к генерации нескольких событий. Эти события являются результатом создания временных элементов в почтовом ящике, изменения элементов хранения данных в режиме свободного или загруженного хранения данных в рамках обычных операций Calendar или обоих. События для класса элементов "IPM. SchedulePlus.FreeBusy.BinaryData" следует игнорировать клиентами веб-службы. Эти временные элементы удаляются после их создания; Поэтому, если будет предпринята попытка получить эти элементы, будет возвращена ошибка, которая заявляет, что элемент не найден.
  
## <a name="getevents-request-example"></a>Пример запроса GetEvents

### <a name="description"></a>Описание

В следующем примере показано, как запрашивать события и элементы, связанные с подпиской, определяемой идентификатором подписки и водяной знак.
  
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

### <a name="getevents-request-elements"></a>Элементы запроса GetEvents

В запросе используются следующие элементы:
  
- [GetEvents](getevents.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="successful-getevents-response-example"></a>Пример успешного ответа GetEvents

### <a name="description"></a>Описание

В следующем примере ответа показано уведомление о наличии двух новых почтовых сообщений с момента последнего запроса уведомления, отправленного на сервер.
  
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
> Идентификаторы элементов и папок были сокращены для сохранения читаемости. 
  
### <a name="getevents-response-elements"></a>Элементы ответа GetEvents

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
    
- [Watermark](watermark.md)
    
- [TimeStamp](timestamp.md)
    
- [ItemId](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
Чтобы найти другие варианты ответного сообщения операции **GetEvents,** ознакомьтесь с иерархией схемы. Начните с элемента [Уведомление.](notification-ex15websvcsotherref.md) 
  
## <a name="getevents-error-response-example"></a>Пример ответа на ошибки GetEvents

### <a name="description"></a>Описание

В следующем примере показан ответ на ошибку на запрос **GetEvents.** 
  
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

## <a name="remarks"></a>Заметки

При обработке **запроса GetEvents** сервер клиентского доступа выполняет следующие действия: 
  
1. Подписка на запрос подтверждается как действительная подписка, которая находится на сервере клиентского доступа. Если это не так, **вызов GetEvents** не удается. 
    
2. SmTP-адрес пользователя с проверкой подлинности для запроса сравнивается с SMTP-адресом пользователя, создавшего подписку. Если они не совпадают, **запрос GetEvents** сбой. 
    
3. Очередь подписки запрашивается для событий, ожидающих их отослать клиенту. Если очередь не пуста, первые 50 событий из очереди будут выдергированы из очереди и закодированы в уведомление.
    
4. Если события в очереди не найдены, создается StatusEvent и закодирован в ответ уведомления.
    
5. Ответ уведомления возвращается клиенту.
    
6. События, включенные в уведомление, удаляются из очереди подписки, а локальный последний водяной знак сервера клиентского доступа для подписки задается водяной знак последнего возвращаемого события.
    
7. Отостановка времени действия подписки.
    
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция Unsubscribe](unsubscribe-operation.md)


[Использование подписки pull](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

