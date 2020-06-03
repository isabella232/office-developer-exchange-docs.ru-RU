---
title: Операция GetAppMarketplaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2c016fc3-0e13-4624-9a5b-d3e84577a860
description: Поиск сведений о GetAppMarketplaceUrlной операции EWS.
ms.openlocfilehash: 6797af44c3aaa6653c440b3d53a282d8c90a4381
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459527"
---
# <a name="getappmarketplaceurl-operation"></a>Операция GetAppMarketplaceUrl

Поиск сведений о **GetAppMarketplaceUrlной** операции EWS. 
  
Операция **GetAppMarketplaceUrl** извлекает URL-адрес магазина приложений, который клиент может посетить для получения приложений для установки в почтовом ящике. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getappmarketplaceurl-operation"></a>Использование операции GetAppMarketplaceUrl

Операция **GetAppMarketplaceUrl** не имеет аргументов для запроса URL-адреса Marketplace, с которого клиент может устанавливать приложения. Ответ будет содержать URL-адрес Marketplace для приложения. 
  
### <a name="getappmarketplaceurl-operation-soap-headers"></a>Заголовки SOAP операции GetAppMarketplaceUrl

Операция **GetAppMarketplaceUrl** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="getappmarketplaceurl-operation-request-example-get-the-app-marketplace-url-for-a-mailbox"></a>Пример запроса операции GetAppMarketplaceUrl: получение URL-адреса магазина приложений для почтового ящика

В следующем примере запроса операции **GetAppMarketplaceUrl** показано, как получить URL-адрес рынка приложений для почтового ящика. 
  
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
      <m:GetAppMarketplaceUrl>
        <m:ApiVersionSupported>1.0</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.0</m:SchemaVersionSupported>
      </m:GetAppMarketplaceUrl>
   </soap:Body>
</soap:Envelope>

```

Текст SOAP Request содержит следующие элементы:
  
- [GetAppMarketplaceUrl](getappmarketplaceurl.md)
    
- [апиверсионсуппортед](apiversionsupported.md)
    
- [счемаверсионсуппортед](schemaversionsupported.md)
    
## <a name="successful-getappmarketplaceurl-operation-response"></a>Успешный отклик операции GetAppMarketplaceUrl

В следующем примере показан успешный ответ на запрос операции **GetAppMarketplaceUrl** для получения URL-адреса рынка приложений для почтового ящика. 
  
> [!NOTE]
> URL-адрес магазина приложений изменен в целях сохранения читаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Success" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <AppMarketplaceUrl>http://marketplace.contoso.com</AppMarketplaceUrl>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>

```

Тело SOAP отклика содержит следующие элементы:
  
- [жетаппмаркетплацеурлреспонсе](getappmarketplaceurlresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [аппмаркетплацеурл](appmarketplaceurl.md)
    
## <a name="getappmarketplaceurl-operation-error-response"></a>Ответ об ошибке операции GetAppMarketPlaceUrl

Ошибки, возвращаемые для этой операции, связаны с неправильной конфигурацией службы или общими ошибками EWS. Коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md). 
  
В следующем примере показан ответ об ошибке, который возвращается, если внешняя панель управления Exchange (ECP) не настроена.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Error" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot get external ECP URL. This might happen if external ECP URL isn't configured.</MessageText>
         <ResponseCode>ErrorCannotGetExternalEcpUrl</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>
```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [жетаппмаркетплацеурлреспонсе](getappmarketplaceurlresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция DisableApp](disableapp-operation.md)
    
- [Операция InstallApp](installapp-operation.md)
    
- [Операция UninstallApp](uninstallapp-operation.md)
    
- [Операция GetAppManifests](getappmanifests-operation.md)
    

