---
title: Операция GetUserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettings
api_type:
- schema
ms.assetid: 153e4440-495b-4972-9811-2fbea740142a
description: Операция GetUserOofSettings получает параметры об отсутствии на работе Office (OOF) и сообщения пользователя почтового ящика.
ms.openlocfilehash: 75a734999842cc33c213e02dc114f23372ae51fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833691"
---
# <a name="getuseroofsettings-operation"></a>Операция GetUserOofSettings

Операция **GetUserOofSettings** получает параметры об отсутствии на работе Office (OOF) и сообщения пользователя почтового ящика. 
  
## <a name="soap-headers"></a>Заголовки SOAP

Операция **GetUserOofSettings** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|Олицетворение  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос.  <br/> |
   
## <a name="using-the-getuseroofsettings-operation"></a>С помощью операции GetUserOofSettings

Операция **GetUserOofSettings** предоставляет доступ к параметрам пользователя об отсутствии на работе. Пользователь идентифицируется адрес электронной почты пользователя. Если сообщение об отсутствии на работе имеет значение null и об отсутствии на работе этот параметр включен, сообщения об отсутствии на работе не отправляются. 
  
> [!IMPORTANT]
> Если сообщений об отсутствии на работе с MicrosoftOfficeOutlook, эта операция возвращает сообщения об отсутствии на работе в формате HTML. 
  
## <a name="getuseroofsettings-request-example"></a>Пример запроса GetUserOofSettings

### <a name="description"></a>Описание

В следующем примере показано **GetUserOofSettings** запрос, который получает сведения об отсутствии на работе одного пользователя. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns ="http://schemas.microsoft.com/exchange/services/2006/types">
        <Address>User1@example.com</Address>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [GetUserOofSettingsRequest](getuseroofsettingsrequest.md)
    
- [Почтовый ящик (доступность)](mailbox-availability.md)
    
- [Адрес (строка)](address-string.md)
    
## <a name="successful-getuseroofsettings-response-example"></a>Пример успешного ответа GetUserOofSettings

### <a name="description"></a>Описание

В следующем примере показано отключенном состоянии об отсутствии на работе с сообщениями об отсутствии на работе.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserOofSettingsResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode>
      </ResponseMessage>
      <OofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Disabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-11-03T23:00:00</StartTime>
          <EndTime>2006-11-04T23:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office. This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </OofSettings>
      <AllowExternalOof>All</AllowExternalOof>
    </GetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-getuseroofsettings-response-elements"></a>Элементы ответов успешно GetUserOofSettings

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
    
- [ResponseMessage](responsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [OofSettings](oofsettings.md)
    
- [OofState](oofstate.md)
    
- [ExternalAudience](externalaudience.md)
    
- [Продолжительность (UserOofSettings)](duration-useroofsettings.md)
    
- [Время начала](starttime.md)
    
- [Время окончания](endtime.md)
    
- [InternalReply](internalreply.md)
    
- [ExternalReply](externalreply.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [AllowExternalOof](allowexternaloof.md)
    
## <a name="getuseroofsettings-error-response-example"></a>Пример ответа об ошибке GetUserOofSettings

### <a name="description"></a>Описание

В следующем примере показано возврату ошибки, возникающие при попытке обращения к другому пользователю сведения об отсутствии на работе.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <faultcode>soap:Client</faultcode>
      <faultstring>Microsoft.Exchange.Data.Storage.AccessDeniedException: User is not mailbox owner. User = S-1-5-21-3642464542-282065186-3871681729-1155, MailboxGuid = S-1-5-21-3642464542-282065186-3871681729-1156 ---> User is not mailbox owner. </faultstring>
      <faultactor>https://CAS01.example.com/EWS/Exchange.asmx</faultactor>
      <detail>
        <ErrorCode xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">-2146233088</ErrorCode>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

