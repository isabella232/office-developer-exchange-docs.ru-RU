---
title: Операция SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 7f0de089-8876-47ec-a871-df118ceae75d
description: Операция SyncFolderItems синхронизирует элементов между сервером Exchange и клиентом.
ms.openlocfilehash: 6b2e4694ac793e17a2b7cb2edb2cb9e6a4a105ea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840128"
---
# <a name="syncfolderitems-operation"></a>Операция SyncFolderItems

Операция SyncFolderItems синхронизирует элементов между сервером Exchange и клиентом.
  
## <a name="remarks"></a>Замечания

Операция SyncFolderItems возвращает не более 512 изменения. Последующие запросы SyncFolderItems необходимо выполнить, чтобы получить дополнительные изменения. 
  
SyncFolderItems аналогично операции FindItem в том, что оно не может возвратить свойства, такие как текст или вложения. Если операция SyncFolderItems не возвращает свойства, которые требуется, можно с помощью [операции GetItem](getitem-operation.md) получить определенный набор свойств для каждого элемента, возвращаемых с SyncFolderItems. 
  
## <a name="syncfolderitems-request-example"></a>Пример запроса SyncFolderItems

### <a name="description"></a>Описание

В следующем примере запрос SyncFolderItems показано, как синхронизировать элементы в папке. В этом примере показано, синхронизация элемента папки, который не является первой синхронизации для происходили для этой папке. Элемент [состояние](syncstate-ex15websvcsotherref.md) не входит в запросе для первой попытке синхронизации клиента с сервером Exchange. Первая попытка синхронизировать элементы в иерархии папок возвращает все элементы в почтовом ящике, кроме элементов, которые определяются в элементе [Игнорировать](ignore.md) . Этот запрос SyncFolderItems попытается синхронизировать все изменения элементов папки с момента последней синхронизации. Этот запрос будет игнорировать попытке синхронизации одного элемента, который идентифицируется в элементе [Игнорировать](ignore.md) . 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderItems xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
      </ItemShape>
      <SyncFolderId>
        <t:DistinguishedFolderId Id="sentitems"/>
      </SyncFolderId>
      <SyncState>AEbJ94eMOAAA=</SyncState>
      <Ignore>
        <t:ItemId Id="AQApAHRAA==" ChangeKey="CQAAABY"/>
      </Ignore>
      <MaxChangesReturned>100</MaxChangesReturned>
    </SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Данные элемента кодировки Base64 [состояние](syncstate-ex15websvcsotherref.md) и атрибута **Id** элемента [ItemId](itemid.md) URL были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [SyncFolderItems](syncfolderitems.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [SyncFolderId](syncfolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Состояние](syncstate-ex15websvcsotherref.md)
    
- [Пропуск](ignore.md)
    
- [Идентификатор элемента](itemid.md)
    
- [MaxChangesReturned](maxchangesreturned.md)
    
## <a name="successful-syncfolderitems-response"></a>Успешного ответа SyncFolderItems

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос SyncFolderItems. В этом примере синхронизируется приглашения на собрание, из папки «Отправленные».
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAA=</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:MeetingRequest>
                <t:ItemId Id="AQApAHRwA==" ChangeKey="CwAAABYA" />
                <t:Subject>Budget Q3</t:Subject>
                <t:Sensitivity>Normal</t:Sensitivity>
                <t:IsOutOfDate>false</t:IsOutOfDate>
                <t:HasBeenProcessed>true</t:HasBeenProcessed>
                <t:ResponseType>NoResponseReceived</t:ResponseType>
                <t:IntendedFreeBusyStatus>Busy</t:IntendedFreeBusyStatus>
                <t:Start>2006-08-02T17:30:00Z</t:Start>
                <t:End>2006-08-02T19:30:00Z</t:End>
                <t:Location>Conference Room 2</t:Location>
                <t:Organizer>
                  <t:Mailbox>
                    <t:Name>Dan Park</t:Name>
                    <t:EmailAddress>dpark@example.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                </t:Organizer>
              </t:MeetingRequest>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Данные элемента кодировки Base64 [состояние](syncstate-ex15websvcsotherref.md) и атрибута **Id** элемента [ItemId](itemid.md) URL были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Состояние](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastItemInRange](includeslastiteminrange.md)
    
- [Изменения (элементы)](changes-items.md)
    
- [Создание (ItemSync)](create-itemsync.md)
    
- [MeetingRequest](meetingrequest.md)
    
- [Идентификатор элемента](itemid.md)
    
- [Subject](subject.md)
    
- [Уровень конфиденциальности сообщения](sensitivity.md)
    
- [IsOutOfDate](isoutofdate.md)
    
- [HasBeenProcessed](hasbeenprocessed.md)
    
- [ResponseType](responsetype.md)
    
- [IntendedFreeBusyStatus](intendedfreebusystatus.md)
    
- [Start](start.md)
    
- [End](end-ex15websvcsotherref.md)
    
- [Location](location.md)
    
- [Организатор](organizer.md)
    
- [Mailbox](mailbox.md)
    
- [Имя (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
## <a name="syncfolderitems-error-response"></a>Ошибка SyncFolderItems ответа

### <a name="description"></a>Описание

В следующем примере показано ошибочный ответ на запрос SyncFolderItems. Эта ошибка была вызвана недопустимое состояние.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupt or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ответа об ошибках

В ответ на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Состояние](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastItemInRange](includeslastiteminrange.md)
    
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

