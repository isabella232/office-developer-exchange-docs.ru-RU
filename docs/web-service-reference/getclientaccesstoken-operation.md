---
title: Операция GetClientAccessToken
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: Найдите сведения о веб-служб Exchange GetClientAccessToken операции.
ms.openlocfilehash: afa9a315a8421f31c345c9547a5d80bed41e9fbc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762713"
---
# <a name="getclientaccesstoken-operation"></a>Операция GetClientAccessToken

Найдите сведения о **GetClientAccessToken** операции веб-служб Exchange. 
  
Операция **GetClientAccessToken** получает клиентского доступа маркер для почтового приложения для Outlook. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getclientaccesstoken-operation"></a>С помощью операции GetClientAccessToken

Запрос операции **GetClientAccessToken** использует два обязательных аргумента: идентификатор приложения и тип маркера. [Операция GetAppManifests](getappmanifests-operation.md) можно использовать для запроса идентификатор приложения. 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a>Заголовки SOAP GetClientAccessToken операции

Операция **GetClientAccessToken** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Этот заголовок можно применять к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a>Пример запроса GetClientAccessToken операции: получение маркера удостоверения вызывающей стороны

Приведенный ниже запрос операции **GetClientAccessToken** показано, как получить маркер удостоверения вызывающей стороны для приложения. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetClientAccessToken>
         <m:TokenRequests>
            <t:TokenRequest>
               <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
               <t:TokenType>CallerIdentity</t:TokenType>
            </t:TokenRequest>
         </m:TokenRequests>
      </m:GetClientAccessToken>
   </soap:Body>
</soap:Envelope>

```

Запрос SOAP body содержит следующие элементы:
  
- [GetClientAccessToken](getclientaccesstoken.md)
    
- [TokenRequests](tokenrequests.md)
    
- [TokenRequest](tokenrequest.md)
    
- [Идентификатор (строка)](id-string.md)
    
- [TokenType](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a>Успешные операции ответа GetClientAccessToken

В следующем примере показано успешного ответа на запрос операции **GetClientAccessToken** для получения маркера удостоверения вызывающей стороны для приложения. 
  
> [!NOTE]
> Для сохранения удобочитаемость URL были сокращены значения маркера в этой статье. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Token>
                  <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
                  <t:TokenType>CallerIdentity</t:TokenType>
                  <t:TokenValue>eyJ0eXAmv0QitaJg</t:TokenValue>
                  <t:TTL>479</t:TTL>
               </m:Token>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>

```

Ответ SOAP body содержит следующие элементы:
  
- [GetClientAccessTokenResponse](getclientaccesstokenresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetClientAccessTokenResponseMessage](getclientaccesstokenresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Маркер (ClientAccessTokenType)](token-clientaccesstokentype.md)
    
- [Идентификатор (строка)](id-string.md)
    
- [TokenType (ClientAccessTokenType)](tokentype-clientaccesstokentype.md)
    
- [TokenValue](tokenvalue.md)
    
- [TTL (ClientAccessTokenTypeType)](ttl-clientaccesstokentypetype.md)
    
## <a name="getclientaccesstoken-operation-error-response"></a>Ошибка операции GetClientAccessToken ответа

В следующем примере показано ошибочный ответ на запрос операции **GetClientAccessToken** . Это ответ на запрос для получения обратного вызова расширение маркеров без соответствующих разрешений. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Error">
               <m:MessageText>The caller does not have enough permission for this token request.</m:MessageText>
               <m:ResponseCode>ErrorInvalidClientAccessTokenRequest</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>
```

Ошибка ответ SOAP body содержит следующие элементы:
  
- [GetClientAccessTokenResponse](getclientaccesstokenresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetClientAccessTokenResponseMessage](getclientaccesstokenresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetAppManifests](getappmanifests-operation.md)
    
- [Надстройки Outlook](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

