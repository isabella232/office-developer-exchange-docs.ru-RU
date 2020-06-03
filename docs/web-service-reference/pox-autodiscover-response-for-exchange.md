---
title: Отклик автообнаружения POX для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 08c6c5a2-a67a-4141-a8bd-1b5d560b90a7
description: Ответ автообнаружения содержит ответ на запрос автообнаружения, включающий список URL-адресов, которые используются для установки привязки с помощью веб-служб Exchange (EWS).
ms.openlocfilehash: 0d903d9829fa6dc1273d8b25a1eeb0b68700d5da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462285"
---
# <a name="pox-autodiscover-response-for-exchange"></a>Отклик автообнаружения POX для Exchange

Ответ автообнаружения содержит ответ на запрос автообнаружения, включающий список URL-адресов, которые используются для установки привязки с помощью веб-служб Exchange (EWS).
  
## <a name="autodiscover-response-example"></a>Пример отклика автообнаружения

### <a name="description"></a>Description

В следующем примере показан успешный ответ автообнаружения.
  
### <a name="code"></a>Код

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
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

Чтобы выполнить присоединение к веб-службам Exchange, используйте URL-адрес, указанный в элементе [асурл (POX)](asurl-pox.md) . 
  
### <a name="response-element"></a>Элемент Response

В тексте отклика используются следующие элементы:
  
- [Служба автообнаружения (POX)](autodiscover-pox.md)
    
- [Ответ (POX)](response-pox.md)
    
- [Пользователь (POX)](user-pox.md)
    
- [DisplayName (POX)](displayname-pox.md)
    
- [LegacyDN (POX)](legacydn-pox.md)
    
- [Деплойментид (POX)](deploymentid-pox.md)
    
- [Учетная запись (POX)](account-pox.md)
    
- [AccountType (POX)](accounttype-pox.md)
    
- [Action (POX)](action-pox.md)
    
- [Протокол (POX)](protocol-pox.md)
    
- [Тип (POX)](type-pox.md)
    
- [Сервер (POX)](server-pox.md)
    
- [Сервердн (POX)](serverdn-pox.md)
    
- [Серверверсион (POX)](serverversion-pox.md)
    
- [Мдбдн (POX)](mdbdn-pox.md)
    
- [Асурл (POX)](asurl-pox.md)
    
- [Уфурл (POX)](oofurl-pox.md)
    
- [Умурл (POX)](umurl-pox.md)
    
- [Оабурл (POX)](oaburl-pox.md)
    
- [Internal (POX)](internal-pox.md)
    
- [Оваурл (POX)](owaurl-pox.md)
    
## <a name="autodiscover-error-response-example"></a>Пример ответа на сообщение об ошибке автообнаружения

### <a name="description"></a>Description

В следующем примере показан ответ об ошибке автообнаружения.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
    <Error Time="21:25:04.8897083" Id="4130155072">
      <ErrorCode>600</ErrorCode>
      <Message>Invalid Request</Message>
      <DebugData />
    </Error>
  </Response>
</Autodiscover>
```

### <a name="error-response-element"></a>Элемент Response Error

В тексте отклика используются следующие элементы:
  
- [Служба автообнаружения (POX)](autodiscover-pox.md)
    
- [Ответ (POX)](response-pox.md)
    
- [Ошибка (POX)](error-pox.md)
    
- [ErrorCode (POX)](errorcode-pox.md)
    
- [Сообщение (POX)](message-pox.md)
    
- [Дебугдата (POX)](debugdata-pox.md)
    
## <a name="see-also"></a>См. также

- [Запрос автообнаружения POX для Exchange](pox-autodiscover-request-for-exchange.md)
- [Справочник по веб-службе автообнаружения POX для Exchange](pox-autodiscover-web-service-reference-for-exchange.md) 
- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

