---
title: Операция Жетдомаинсеттингс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a6f4a53d-d7f6-4ad1-8afb-78745c500eaa
description: Операция Жетдомаинсеттингс получает указанные параметры домена для пользователя. Служба автообнаружения возвращает домены, которые должны быть обнаружены, и запрошенные параметры этих доменов.
ms.openlocfilehash: fd655e088b73372bc1dd68a740ebc2b516d1804a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460969"
---
# <a name="getdomainsettings-operation-soap"></a>Операция Жетдомаинсеттингс (SOAP)

Операция **жетдомаинсеттингс** получает указанные параметры домена для пользователя. Служба автообнаружения возвращает домены, которые должны быть обнаружены, и запрошенные параметры этих доменов. 
  
## <a name="getdomainsettings-request-example"></a>Пример запроса Жетдомаинсеттингс

### <a name="description"></a>Описание

В следующем примере запроса **жетдомаинсеттингс** показано, как запросить параметры домена **екстерналевсурл** пользователя. Клиент отправляет этот запрос на сервер. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"> 
    <soap:Header> 
        <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
        <wsa:Action>https://schemas.microsoft.com/exchange/2010/
            Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
        <wsa:To>
            https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc
        </wsa:To>
    </soap:Header> 
    <soap:Body> 
        <a:GetDomainSettingsRequestMessage xmlns:a="https://schemas.microsoft.com
            /exchange/2010/Autodiscover"> 
            <a:Request> 
                <a:Domains> 
                    <a:Domain>contoso.com<</a:Domain> 
                </a:Domains> 
                <a:RequestedSettings> 
                    <a:Setting>ExternalEwsUrl</a:Setting> 
                </a:RequestedSettings> 
            </a:Request> 
        </a:GetDomainSettingsRequestMessage> 
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [Жетдомаинсеттингсрекуестмессаже (SOAP)](getdomainsettingsrequestmessage-soap.md)
    
- [Запрос (SOAP)](request-soap.md)
    
- [Домены (SOAP)](domains-soap.md)
    
- [Домен (SOAP)](domain-soap.md)
    
- [Рекуестедсеттингс (SOAP)](requestedsettings-soap.md)
    
- [Параметр (SOAP)](setting-soap.md)
    
## <a name="getdomainsettings-response-example"></a>Пример отклика Жетдомаинсеттингс

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос **жетдомаинсеттингс** , отправляемый сервером клиенту. 
  
### <a name="code"></a>Код

```XML
//www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/ 
            Autodiscover/Autodiscover/GetDomainSettingsResponse
        </a:Action> 
        <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
            xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
        <h:MajorVersion>14</h:MajorVersion> 
        <h:MinorVersion>0</h:MinorVersion> 
        <h:MajorBuildNumber>639</h:MajorBuildNumber> 
        <h:MinorBuildNumber>20</h:MinorBuildNumber> 
        <h:Version>Exchange2010</h:Version> 
        </h:ServerVersionInfo>
    </s:Header> 
    <s:Body> 
        <GetDomainSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage /> 
                <DomainResponses> 
                    <DomainResponse> 
                        <ErrorCode>NoError</ErrorCode> 
                        <ErrorMessage>No error.</ErrorMessage> 
                        <DomainSettingErrors /> 
                        <DomainSettings> 
                            <DomainSetting i:type="DomainStringSetting"> 
                                <Name>ExternalEwsUrl</Name> 
                                <Value>https://emea.mail.microsoft.com/EWS/Exchange.asmx</Value> 
                            </DomainSetting> 
                        </DomainSettings> 
                        <RedirectTarget i:nil="true" /> 
                    </DomainResponse> 
                </DomainResponses> 
            </Response> 
        </GetDomainSettingsResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a>Элементы Response

В отклике используются следующие элементы:
  
- [Жетдомаинсеттингсреспонсемессаже (SOAP)](getdomainsettingsresponsemessage-soap.md)
    
- [Отклик (SOAP)](response-soap.md)
    
- [ErrorCode (SOAP)](errorcode-soap.md)
    
- [ErrorMessage (SOAP)](errormessage-soap.md)
    
- [Домаинреспонсес (SOAP)](domainresponses-soap.md)
    
- [Домаинреспонсе (SOAP)](domainresponse-soap.md)
    
- [Домаинсеттинжеррорс (SOAP)](domainsettingerrors-soap.md)
    
- [Домаинсеттингс (SOAP)](domainsettings-soap.md)
    
- [Домаинсеттинг (SOAP)](domainsetting-soap.md)
    
- [Имя (SOAP)](name-soap.md)
    
- [Значение (SOAP)](value-soap.md)
    
- [Редиректтаржет (SOAP)](redirecttarget-soap.md)
    
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция Жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)

