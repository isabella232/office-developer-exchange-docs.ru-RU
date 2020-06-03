---
title: Операция DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 211731a3-2470-49af-bda3-1ddfc15a8e46
description: Поиск сведений о DisableAppной операции EWS.
ms.openlocfilehash: 8e1f3a257a70c042a01ed70da97cfa0573a2d454
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462068"
---
# <a name="disableapp-operation"></a>Операция DisableApp

Поиск сведений о **DisableAppной** операции EWS. 
  
Операция **DisableApp** отключает почтовое приложение для Outlook. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-disableapp-operation"></a>Использование операции DisableApp

Операция **DisableApp** принимает в запросе два аргумента, которые определяют, что почтовое приложение будет отключено, и причины, по которым оно было отключено. 
  
### <a name="disableapp-operation-soap-headers"></a>Заголовки SOAP операции DisableApp

Операция **DisableApp** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="disableapp-operation-request-example-disable-a-mail-app-installed-in-a-mailbox"></a>Пример запроса операции DisableApp: Отключение почтового приложения, установленного в почтовом ящике

В следующем примере запроса операции **DisableApp** показано, как отключить почтовое приложение. Идентификатор приложения можно найти в манифесте приложения, который возвращается в ответе [операции GetAppManifests](getappmanifests-operation.md) . 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:DisableApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
         <m:DisableReason>NoReason</m:DisableReason>
      </m:DisableApp>
   </soap:Body>
</soap:Envelope>
```

Текст SOAP Request содержит следующие элементы:
  
- [DisableApp](disableapp.md)
    
- [ID (строка)](id-string.md)
    
- [дисаблереасон](disablereason.md)
    
## <a name="successful-disableapp-operation-response"></a>Успешный отклик операции DisableApp

В следующем примере показан успешный ответ на запрос операции **DisableApp** для отключения почтового приложения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [дисаблеаппреспонсе](disableappresponse.md)
    
- [респонсекоде](responsecode.md)
    
## <a name="disableapp-operation-error-response"></a>Ответ об ошибке операции DisableApp

В следующем примере показан ответ об ошибке для запроса операции **DisableApp** . Это ответ на запрос на отключение почтового приложения, которое не установлено в почтовом ящике. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="14" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1C50226D-04B5-4AB2-9FCD-42E236B59E4A can't be found.</MessageText>
         <ResponseCode>ErrorExtensionNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [дисаблеаппреспонсе](disableappresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)   
- [Операция InstallApp](installapp-operation.md)   
- [Операция UninstallApp](uninstallapp-operation.md)   
- [GetAppManifests](getappmanifests.md)   
- [Операция GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)   
- [Надстройки Outlook](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

