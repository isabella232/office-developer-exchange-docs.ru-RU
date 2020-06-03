---
title: Операция GetUserSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 758d965c-ef63-4de4-9120-e293abf14ff8
description: Операция GetUserSettings содержит запрос для настройки клиентского доступа пользователей.
ms.openlocfilehash: e274fd4e1ca954ea25ea91a52e363c9a434b290a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466145"
---
# <a name="getusersettings-operation-soap"></a>Операция GetUserSettings (SOAP)

Операция **GetUserSettings** содержит запрос для настройки клиентского доступа пользователей. 
  
## <a name="getusersettings-request-example"></a>Пример запроса GetUserSettings

### <a name="description"></a>Description

В приведенном ниже примере XML-кода показан основной текст запроса автообнаружения, который запрашивает отображаемое имя пользователя, различающееся имя, идентификатор развертывания, сервер почтовых ящиков, различающееся имя почтового ящика, сервер Active Directory, версию сервера клиентского доступа и поддерживаемые схемы веб-служб Exchange.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover"      
               xmlns:wsa="http://www.w3.org/2005/08/addressing" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"      
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://myserver.contoso.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>UserName@domain.contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>UserDisplayName</a:Setting>
          <a:Setting>UserDN</a:Setting>
          <a:Setting>UserDeploymentId</a:Setting>
          <a:Setting>InternalMailboxServer</a:Setting>
          <a:Setting>MailboxDN</a:Setting>
          <a:Setting>ActiveDirectoryServer</a:Setting>
          <a:Setting>CasVersion</a:Setting>
          <a:Setting>EwsSupportedSchemas</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a>Элементы Request

В тексте запроса используются следующие элементы:
  
- [Жетусерсеттингсрекуестмессаже (SOAP)](getusersettingsrequestmessage-soap.md)
    
- [Почтовый ящик (SOAP)](mailbox-soap.md)
    
- [Запрос (SOAP)](request-soap.md)
    
- [Рекуестедсерверверсион (SOAP)](requestedserverversion-soap.md)
    
- [Рекуестедсеттингс (SOAP)](requestedsettings-soap.md)
    
- [Параметр (SOAP)](setting-soap.md)
    
- [Пользователь (SOAP)](user-soap.md)
    
- [Пользователи (SOAP)](users-soap.md)
    
## <a name="getusersettings-response-example"></a>Пример отклика GetUserSettings

### <a name="description"></a>Description

В следующем примере показан успешный ответ **GetUserSettings** . 
  
### <a name="code"></a>Код

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
  </s:Header>
  <s:Body>
  <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>UserDisplayName</Name>
                <Value>UserDisplayName</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDN</Name>
                <Value>/o=First Organization/ou=Exchange Administrative Group (SDASDASDJ)/cn=Recipients/cn=UserDisplayName</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDeploymentId</Name>
                <Value>a40E2742-21c6-4050-8Ed2-d41f100c22b8</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>CasVersion</Name>
                <Value>14.00.0478.000</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EwsSupportedSchemas</Name>
                <Value>Exchange2007,  Exchange2010</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>InternalMailboxServer</Name>
                <Value>machinename.domain.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ActiveDirectoryServer</Name>
                <Value>machinename.domain.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>MailboxDN</Name>
                <Value>/o=First Organization/ou=Exchange Administrative Group (SDASDASDJ)/cn=Configuration/cn=Servers/cn=server/cn=Contoso Pri MDB</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

### <a name="response-elements"></a>Элементы Response

В тексте отклика используются следующие элементы:
  
- [ErrorCode (SOAP)](errorcode-soap.md)
    
- [ErrorMessage (SOAP)](errormessage-soap.md)
    
- [Жетусерсеттингсреспонсемессаже (SOAP)](getusersettingsresponsemessage-soap.md)
    
- [Имя (SOAP)](name-soap.md)
    
- [Редиректтаржет (SOAP)](redirecttarget-soap.md)
    
- [Отклик (SOAP)](response-soap.md)
    
- [Усерреспонсе (SOAP)](userresponse-soap.md)
    
- [Усерреспонсес (SOAP)](userresponses-soap.md)
    
- [Усерсеттинг (SOAP)](usersetting-soap.md)
    
- [Усерсеттинжеррорс (SOAP)](usersettingerrors-soap.md)
    
- [Усерсеттингс (SOAP)](usersettings-soap.md)
    
- [Значение (SOAP)](value-soap.md)
    
## <a name="see-also"></a>См. также



[Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)
  
[Операция Жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)


[XML-элементы автообнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

