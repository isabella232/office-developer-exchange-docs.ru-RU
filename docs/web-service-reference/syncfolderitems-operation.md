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
description: Операция SyncFolderItems синхронизирует элементы между сервером Exchange Server и клиентом.
ms.openlocfilehash: 6b2e4694ac793e17a2b7cb2edb2cb9e6a4a105ea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840128"
---
# <a name="syncfolderitems-operation"></a>Операция SyncFolderItems

Операция SyncFolderItems синхронизирует элементы между сервером Exchange Server и клиентом.
  
## <a name="remarks"></a>Примечания

Для операции SyncFolderItems будет возвращено не более 512 изменений. Для получения дополнительных изменений необходимо выполнить последующие запросы SyncFolderItems. 
  
SyncFolderItems аналогичен операции FindItem, так как она не может возвращать такие свойства, как текст или вложения. Если операция SyncFolderItems не возвращает нужные свойства, можно использовать [операцию GetItem](getitem-operation.md) для получения определенного набора свойств для каждого элемента, возвращенного SyncFolderItems. 
  
## <a name="syncfolderitems-request-example"></a>Пример запроса SyncFolderItems

### <a name="description"></a>Описание

В приведенном ниже примере запроса SyncFolderItems показано, как синхронизировать элементы в папке. В этом примере показана синхронизация элемента папки, которая не является первой синхронизацией, которая возникла для папки "Отправленные". Элемент [синкстате](syncstate-ex15websvcsotherref.md) не включается в запрос первой попытки синхронизации клиента с сервером Exchange. При первой попытке синхронизации элементов в иерархии папок будут возвращены все элементы почтового ящика, кроме элементов, указанных в элементе [Ignore](ignore.md) . Этот запрос SyncFolderItems попытается выполнить синхронизацию всех изменений элементов папки с момента последней синхронизации. Этот запрос будет игнорировать попытку синхронизации одного элемента, указанного в элементе [Ignore](ignore.md) . 
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

Данные элемента [синкстате](syncstate-ex15websvcsotherref.md) с кодировкой base64 и атрибут **идентификатора** элемента [ItemId](itemid.md) были сокращены для сохранения удобочитаемости. 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [SyncFolderItems](syncfolderitems.md)
    
- [итемшапе](itemshape.md)
    
- [басешапе](baseshape.md)
    
- [синкфолдерид](syncfolderid.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
- [синкстате](syncstate-ex15websvcsotherref.md)
    
- [Ignore](ignore.md)
    
- [Идентификатор](itemid.md)
    
- [максчанжесретурнед](maxchangesreturned.md)
    
## <a name="successful-syncfolderitems-response"></a>Успешный ответ SyncFolderItems

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос SyncFolderItems. В этом примере приглашение на собрание синхронизируется из папки "Отправленные".
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

Данные элемента [синкстате](syncstate-ex15websvcsotherref.md) с кодировкой base64 и атрибут **идентификатора** элемента [ItemId](itemid.md) были сокращены для сохранения удобочитаемости. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [синкфолдеритемсреспонсе](syncfolderitemsresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [синкфолдеритемсреспонсемессаже](syncfolderitemsresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [синкстате](syncstate-ex15websvcsotherref.md)
    
- [инклудесластитеминранже](includeslastiteminrange.md)
    
- [Изменения (элементы)](changes-items.md)
    
- [Create (Итемсинк)](create-itemsync.md)
    
- [Свойство meetingrequest](meetingrequest.md)
    
- [Идентификатор](itemid.md)
    
- [Тема](subject.md)
    
- [Sensitivity](sensitivity.md)
    
- [IsOutOfDate](isoutofdate.md)
    
- [хасбинпроцессед](hasbeenprocessed.md)
    
- [ResponseType](responsetype.md)
    
- [интендедфрибусистатус](intendedfreebusystatus.md)
    
- [Начало](start.md)
    
- [Оканчиваться](end-ex15websvcsotherref.md)
    
- [Location](location.md)
    
- [Organizer](organizer.md)
    
- [Mailbox](mailbox.md)
    
- [Имя (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (Нонемптистрингтипе)](emailaddress-nonemptystringtype.md)
    
- [Раутингтипе (EmailAddressType)](routingtype-emailaddresstype.md)
    
## <a name="syncfolderitems-error-response"></a>Ответ об ошибке SyncFolderItems

### <a name="description"></a>Описание

В следующем примере показан ответ об ошибке для запроса SyncFolderItems. Эта ошибка вызвана недопустимым Синкстате.
  
### <a name="code"></a>Код

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

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [синкфолдеритемсреспонсе](syncfolderitemsresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [синкфолдеритемсреспонсемессаже](syncfolderitemsresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [синкстате](syncstate-ex15websvcsotherref.md)
    
- [инклудесластитеминранже](includeslastiteminrange.md)
    
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

