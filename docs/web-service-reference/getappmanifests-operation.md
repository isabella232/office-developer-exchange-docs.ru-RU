---
title: Операция GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Поиск сведений о GetAppManifestsной операции EWS.
ms.openlocfilehash: 4d4c1d32f14cf144335ddfdf8c9cd4c88a4421d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463008"
---
# <a name="getappmanifests-operation"></a>Операция GetAppManifests

Поиск сведений о **GetAppManifestsной** операции EWS. 
  
Операция **GetAppManifests** получает манифесты приложений. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getappmanifests-operation"></a>Использование операции GetAppManifests

Операция **GetAppManifests** не имеет аргументов для запроса манифестов приложений для почтового ящика. Ответ будет содержать XML-файлы манифеста в кодировке Base64 для каждого приложения, установленного в почтовом ящике. 
  
### <a name="getappmanifests-operation-soap-headers"></a>Заголовки SOAP операции GetAppManifests

Операция **GetAppManifests** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a>Пример запроса операции GetAppManifests: получение манифестов приложений для почтового ящика

В следующем примере запроса операции **GetAppManifests** показано, как получить манифесты приложения для почтового ящика. Элементы [апиверсионсуппортед](apiversionsupported.md) и [счемаверсионсуппортед](schemaversionsupported.md) являются необязательными. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013_SP1" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:GetAppManifests>
        <m:ApiVersionSupported>1.1</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.1</m:SchemaVersionSupported>
      </m:GetAppManifests>
   </soap:Body>
</soap:Envelope>

```

Текст SOAP запроса содержит следующий элемент:
  
- [GetAppManifests](getappmanifests.md)
    
- [апиверсионсуппортед](apiversionsupported.md)
    
- [счемаверсионсуппортед](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a>Успешный отклик операции GetAppManifests

В следующем примере показан успешный ответ на запрос операции **GetAppManifests** для получения манифестов приложений для почтового ящика. 
  
> [!NOTE]
> Все манифесты приложений Base64 были произвольно усечены, чтобы сохранить удобочитаемость. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [жетаппманифестсреспонсе](getappmanifestsresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [Приложения](apps.md)
    
- [Приложение](app.md)
    
- [Манифест](manifest.md)
    
Тело SOAP отклика также может содержать следующий элемент:
  
- [Манифесты](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a>Ответ об ошибке операции GetAppManifests

Ошибки, возвращаемые для этой операции, связаны с недопустимым форматом входных параметров или общими ошибками EWS. Коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция DisableApp](disableapp-operation.md)
    
- [Операция InstallApp](installapp-operation.md)
    
- [Операция UninstallApp](uninstallapp-operation.md)
    
- [Операция GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)
    

