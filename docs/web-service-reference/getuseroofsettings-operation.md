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
description: Операция GetUserOofSettings Возвращает параметры и сообщения пользователя почтового ящика "нет на месте" (отсутствие на работе).
ms.openlocfilehash: 622faa622b0ea231a6331ff62631885d4252c1f5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457699"
---
# <a name="getuseroofsettings-operation"></a>Операция GetUserOofSettings

Операция **GetUserOofSettings** Возвращает параметры и сообщения пользователя почтового ящика "нет на месте" (отсутствие на работе). 
  
## <a name="soap-headers"></a>Заголовки SOAP

Операция **GetUserOofSettings** может использовать заголовки SOAP, указанные в приведенной ниже таблице и описанные в следующей таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|Олицетворение  <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение.  <br/> |
|серверверсион  <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос.  <br/> |
   
## <a name="using-the-getuseroofsettings-operation"></a>Использование операции GetUserOofSettings

Операция **GetUserOofSettings** предоставляет доступ к параметрам отсутствия на работе пользователя. Пользователь идентифицируется по адресу электронной почты пользователя. Если сообщение об отсутствии на работе имеет значение NULL и включено отсутствие на работе, сообщение об отсутствии на месте не отправляется. 
  
> [!IMPORTANT]
> Если сообщения об отсутствии на работе задаются Майкрософтofficeoutlook, эта операция возвратит сообщения об отсутствии на работе в формате HTML. 
  
## <a name="getuseroofsettings-request-example"></a>Пример запроса GetUserOofSettings

### <a name="description"></a>Description

В приведенном ниже примере показан запрос **GetUserOofSettings** , который получает сведения об отсутствии на работе отдельных пользователей. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns ="https://schemas.microsoft.com/exchange/services/2006/types">
        <Address>User1@example.com</Address>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [жетусеруфсеттингсрекуест](getuseroofsettingsrequest.md)
    
- [Mailbox (доступность)](mailbox-availability.md)
    
- [Address (строка)](address-string.md)
    
## <a name="successful-getuseroofsettings-response-example"></a>Пример успешного ответа GetUserOofSettings

### <a name="description"></a>Description

В следующем примере показано отключенное состояние отсутствия на работе с сообщениями об отсутствии на работе.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserOofSettingsResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode>
      </ResponseMessage>
      <OofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="successful-getuseroofsettings-response-elements"></a>Успешные элементы ответа GetUserOofSettings

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [жетусеруфсеттингсреспонсе](getuseroofsettingsresponse.md)
    
- [респонсемессаже](responsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [уфсеттингс](oofsettings.md)
    
- [уфстате](oofstate.md)
    
- [екстерналаудиенце](externalaudience.md)
    
- [Продолжительность (Усеруфсеттингс)](duration-useroofsettings.md)
    
- [StartTime](starttime.md)
    
- [EndTime](endtime.md)
    
- [интерналрепли](internalreply.md)
    
- [екстерналрепли](externalreply.md)
    
- [Сообщение](message-ex15websvcsotherref.md)
    
- [алловекстерналуф](allowexternaloof.md)
    
## <a name="getuseroofsettings-error-response-example"></a>Пример ответа на сообщение об ошибке GetUserOofSettings

### <a name="description"></a>Description

В следующем примере показан ответ об ошибке, вызванный попыткой доступа к сведениям об отсутствии на работе другого пользователя.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <faultcode>soap:Client</faultcode>
      <faultstring>Microsoft.Exchange.Data.Storage.AccessDeniedException: User is not mailbox owner. User = S-1-5-21-3642464542-282065186-3871681729-1155, MailboxGuid = S-1-5-21-3642464542-282065186-3871681729-1156 ---> User is not mailbox owner. </faultstring>
      <faultactor>https://CAS01.example.com/EWS/Exchange.asmx</faultactor>
      <detail>
        <ErrorCode xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">-2146233088</ErrorCode>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

