---
title: POX ответа службы автообнаружения для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 08c6c5a2-a67a-4141-a8bd-1b5d560b90a7
description: Ответ на запрос службы автообнаружения, которая содержит список URL-адресов, которые используются для установления привязки с помощью веб-служб Exchange (EWS) содержит ответ службы автообнаружения.
ms.openlocfilehash: d9f8a5cc86efaa4dceda7385164872ecc5409252
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834863"
---
# <a name="pox-autodiscover-response-for-exchange"></a>POX ответа службы автообнаружения для Exchange

Ответ на запрос службы автообнаружения, которая содержит список URL-адресов, которые используются для установления привязки с помощью веб-служб Exchange (EWS) содержит ответ службы автообнаружения.
  
## <a name="autodiscover-response-example"></a>Пример ответа службы автообнаружения

### <a name="description"></a>Описание

В следующем примере показано успешного ответа службы автообнаружения.
  
### <a name="code"></a>Программа

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <User>
      <DisplayName>First Last</DisplayName>
      <LegacyDN>/o=contoso/ou=First Administrative Group/cn=Recipients/cn=iuser885646</LegacyDN>
      <DeploymentId>644560b8-a1ce-429c-8ace-23395843f701</DeploymentId>
    </User>
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>MBX-SERVER.mail.internal.contoso.com</Server>
        <ServerDN>/o=contoso/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=MBX-SERVER</ServerDN>
        <ServerVersion>72008287</ServerVersion>
        <MdbDN>/o=contoso/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=MBX-SERVER/cn=Microsoft Private MDB</MdbDN>
        <ASUrl>https://mail.contoso.com/ews/exchange.asmx</ASUrl>
        <OOFUrl>https://mail.contoso.com/ews/exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/unifiedmessaging/service.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/d29844a9-724e-468c-8820-0f7b345b767b/</OABUrl>
      </Protocol>
      <Protocol>
        <Type>EXPR</Type>
        <Server>Exchange.contoso.com</Server>
        <ASUrl>https://mail.contoso.com/ews/exchange.asmx</ASUrl>
        <OOFUrl>https://mail.contoso.com/ews/exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/unifiedmessaging/service.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/d29844a9-724e-468c-8820-0f7b345b767b/</OABUrl>
      </Protocol>
      <Protocol>
        <Type>WEB</Type>
        <Internal>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-01-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-02-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Basic">https://cas-04-server.mail.internal.contoso.com/owa</OWAUrl>
          <OWAUrl AuthenticationMethod="Ntlm, WindowsIntegrated">https://cas-05-server.mail.internal.contoso.com/owa</OWAUrl>
        </Internal>
      </Protocol>
    </Account>
  </Response>
</Autodiscover>
```

### <a name="comments"></a>Комментарии

Чтобы привязать к веб-служб Exchange, используйте URL-адрес, обнаруженных в элементе [ASUrl (POX)](asurl-pox.md) . 
  
### <a name="response-element"></a>Элемент Response

В теле ответа используются следующие элементы:
  
- [Автообнаружение (POX)](autodiscover-pox.md)
    
- [Ответ (POX)](response-pox.md)
    
- [Пользователь (POX)](user-pox.md)
    
- [DisplayName (POX)](displayname-pox.md)
    
- [LegacyDN (POX)](legacydn-pox.md)
    
- [DeploymentId (POX)](deploymentid-pox.md)
    
- [Учетная запись (POX)](account-pox.md)
    
- [AccountType (POX)](accounttype-pox.md)
    
- [Действие (POX)](action-pox.md)
    
- [Протокол (POX)](protocol-pox.md)
    
- [Тип (POX)](type-pox.md)
    
- [Сервер (POX)](server-pox.md)
    
- [ServerDN (POX)](serverdn-pox.md)
    
- [ServerVersion (POX)](serverversion-pox.md)
    
- [MdbDN (POX)](mdbdn-pox.md)
    
- [ASUrl (POX)](asurl-pox.md)
    
- [OOFUrl (POX)](oofurl-pox.md)
    
- [UMUrl (POX)](umurl-pox.md)
    
- [OABUrl (POX)](oaburl-pox.md)
    
- [Внутренний (POX)](internal-pox.md)
    
- [OWAUrl (POX)](owaurl-pox.md)
    
## <a name="autodiscover-error-response-example"></a>Пример ответа об ошибке автообнаружения

### <a name="description"></a>Описание

В следующем примере показано возврату ошибки службы автообнаружения.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
    <Error Time="21:25:04.8897083" Id="4130155072">
      <ErrorCode>600</ErrorCode>
      <Message>Invalid Request</Message>
      <DebugData />
    </Error>
  </Response>
</Autodiscover>
```

### <a name="error-response-element"></a>Элемент ответа об ошибках

В теле ответа используются следующие элементы:
  
- [Автообнаружение (POX)](autodiscover-pox.md)
    
- [Ответ (POX)](response-pox.md)
    
- [Ошибка (POX)](error-pox.md)
    
- [Код ошибки (POX)](errorcode-pox.md)
    
- [Сообщение (POX)](message-pox.md)
    
- [DebugData (POX)](debugdata-pox.md)
    
## <a name="see-also"></a>См. также

- [Запрос автообнаружения POX для Exchange](pox-autodiscover-request-for-exchange.md)
- [Служба POX автоматического обнаружения веб-ссылки для Exchange](pox-autodiscover-web-service-reference-for-exchange.md) 
- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

