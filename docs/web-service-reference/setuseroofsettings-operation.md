---
title: Операция SetUserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettings
api_type:
- schema
ms.assetid: 36277ef0-18ee-4b35-9e6e-8c321d8f5433
description: Веб-метод SetUserOofSettings устанавливает параметры и сообщение "нет на месте" для пользователя почтового ящика.
ms.openlocfilehash: 88b5475dd2f0fe6d334bad51a0fe8d0beb767634
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463155"
---
# <a name="setuseroofsettings-operation"></a>Операция SetUserOofSettings

Веб-метод **SetUserOofSettings** устанавливает параметры и сообщение "нет на месте" для пользователя почтового ящика. 
  
## <a name="soap-headers"></a>Заголовки SOAP

Операция **SetUserOofSettings** может использовать заголовки SOAP, указанные в приведенной ниже таблице и описанные в следующей таблице. 
  
|**Header**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|Олицетворение  <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение.  <br/> |
|серверверсион  <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос.  <br/> |
   
## <a name="setuseroofsettings-request-example"></a>Пример запроса SetUserOofSettings

### <a name="description"></a>Описание

В следующем примере запроса **SetUserOofSettings** задается значение параметра "отсутствие на работе" в течение 10 дней. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>User1</Name>
        <Address>user1@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-10-05T00:00:00</StartTime>
          <EndTime>2006-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [сетусеруфсеттингсрекуест](setuseroofsettingsrequest.md)
    
- [Mailbox (доступность)](mailbox-availability.md)
    
- [Имя (EmailAddress)](name-emailaddress.md)
    
- [Address (строка)](address-string.md)
    
- [Раутингтипе (EmailAddress)](routingtype-emailaddress.md)
    
- [усеруфсеттингс](useroofsettings.md)
    
- [уфстате](oofstate.md)
    
- [екстерналаудиенце](externalaudience.md)
    
- [Продолжительность (Усеруфсеттингс)](duration-useroofsettings.md)
    
- [StartTime](starttime.md)
    
- [EndTime](endtime.md)
    
- [интерналрепли](internalreply.md)
    
- [Сообщение (доступность)](message-availability.md)
    
- [екстерналрепли](externalreply.md)
    
## <a name="successful-setuseroofsettings-response-example"></a>Пример успешного ответа SetUserOofSettings

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос **SetUserOofSettings** . 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" /> 
  </soap:Header>
  <soap:Body>
    <SetUserOofSettingsResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode> 
      </ResponseMessage>
    </SetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [сетусеруфсеттингсреспонсе](setuseroofsettingsresponse.md)
    
- [респонсемессаже](responsemessage.md)
    
- [респонсекоде](responsecode.md)
    
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

