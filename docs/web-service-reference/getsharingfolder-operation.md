---
title: Операция GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: 75fee92a-a7f8-4a62-ad2b-17acbaada186
description: Операция GetSharingFolder Получает идентификатор локальной папки указанной общей папке.
ms.openlocfilehash: 23adb10b22623fcbc1dd6b33bd674afafdaa8b19
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833670"
---
# <a name="getsharingfolder-operation"></a>Операция GetSharingFolder

Операция **GetSharingFolder** Получает идентификатор локальной папки указанной общей папке. 
  
## <a name="soap-headers"></a>Заголовки SOAP

Операция **GetSharingFolder** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос.  <br/> |
   
## <a name="getsharingfolder-request-example"></a>Пример запроса GetSharingFolder

### <a name="getting-the-local-folder-identifier-by-specifying-the-sharedfolderid-element-of-the-folder-being-shared"></a>Получение идентификатора локальную папку путем указания элемент SharedFolderId общей папке

В следующем примере кода показано, как для формирования запроса, чтобы получить идентификатор локальной папки, соответствующее к папке, где находится в совместном. К папке, где находится в совместном идентифицируется по SMTP-адрес почтового ящика, содержащем папку общий и по [SharedFolderId](sharedfolderid.md) элемент, представляющий идентификатор этой папке. В этом примере к папке, где находится в совместном владельцем user1@contoso.com. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:SharedFolderId>AAMkA=</m:SharedFolderId>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="getting-the-local-folder-identifier-by-specifying-the-datatype-element-of-the-folder-being-shared"></a>Начало идентификатор локальной папки, указав тип данных элемента общей папке

В следующем примере кода показано, как для формирования запроса, чтобы получить идентификатор локальной папки, соответствующее к папке, где находится в совместном. К папке, где находится в совместном определяется путем SMTP-адрес почтового ящика, содержащем папку общий и элемент [тип данных](datatype.md) , представляющий тип данных в этой папке. В этом примере выполняется общей папки — это папка Контакты, владельцем которого является user1@contoso.com. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:DataType>Contacts</m:DataType>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Сведения о возможных значений элемента **типа данных** содержатся в разделе [тип данных](datatype.md).
  
## <a name="successful-getsharingfolder-response"></a>Успешного ответа GetSharingFolder

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **GetSharingFolder** . Атрибут **Id** элемента [SharingFolderId](sharingfolderid.md) представляет идентификатор локальной папки в отношении общего доступа. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="getsharingfolder-error-response"></a>Ошибка GetSharingFolder ответа

### <a name="description"></a>Описание

В следующем примере показано ошибочный ответ на запрос **GetSharingFolder** . В этом примере произошла ошибка, так как запрос определенных элементов и [SharingFolderId](sharingfolderid.md) и [типа данных](datatype.md) . Обратите внимание на то, что только тот или иной этих двух элементов можно указать, но не оба. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Error" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Either DataType or SharedFolderId must be specified, but not both.</m:MessageText>
      <m:ResponseCode>ErrorInvalidGetSharingFolderRequest</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



[GetSharingFolder](getsharingfolder.md)
  
[GetSharingFolderType](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderType.aspx)
  
[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md)
  
[GetSharingFolderResponseMessageType](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderResponseMessageType.aspx)


[Операции EWS в Exchange](ews-operations-in-exchange.md)
  
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

