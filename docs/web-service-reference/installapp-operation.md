---
title: Операция InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: Сведения об операции InstallApp EWS.
ms.openlocfilehash: 87e6f1caddd6949d5dc98edc074acd365de818d9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515581"
---
# <a name="installapp-operation"></a>Операция InstallApp

Сведения об операции **InstallApp** EWS. 
  
Операция **InstallApp** устанавливает почтовое приложение для Outlook в почтовом ящике. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-installapp-operation"></a>Использование операции InstallApp

Операция **InstallApp** использует один аргумент, который идентифицирует почтовое приложение для установки. Аргумент содержит манифест с кодом base64 для почтового приложения. 
  
### <a name="installapp-operation-soap-headers"></a>Заготчики операции InstallApp SOAP

В **операции InstallApp** можно использовать заглавные таблицы SOAP, указанные в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Этот заглавный заглавник применим к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Этот заглавный заглавник применим к ответу.  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a>Пример запроса на операцию InstallApp: Установка почтового приложения в почтовом ящике

В следующем примере запроса на операцию **InstallApp** показано, как установить почтовое приложение для Outlook. Манифест приложения можно найти с помощью [операции GetAppManifests.](getappmanifests-operation.md)
  
> [!NOTE]
> Манифест приложения с кодом base64 был произвольно усечен для сохранения читаемости и не представляет допустимого манифеста. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:InstallApp>
         <m:Manifest>TUwiIC8+CiAgPC9SdWxlPgo8L09mZmljZUFwcD4=</m:Manifest>
      </m:InstallApp>
   </soap:Body>
</soap:Envelope>

```

Тело SOAP запроса содержит следующие элементы:
  
- [InstallApp](installapp.md)
    
- [Манифест](manifest.md)
    
## <a name="successful-installapp-operation-response"></a>Успешный ответ операции InstallApp

В следующем примере показан успешный ответ на запрос на операцию **InstallApp** для установки почтового приложения. 
  
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
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP ответа содержит следующие элементы:
  
- [InstallAppResponse](installappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="installapp-operation-error-response"></a>Ответ на ошибку операции InstallApp

В следующем примере показан ответ на ошибку на запрос **операции InstallApp.** Это ответ на запрос, содержащий недействительный манифест. 
  
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
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

Тело SOAP ответа на ошибку содержит следующие элементы:
  
- [InstallAppResponse](installappresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция DisableApp](disableapp-operation.md)
    
- [Операция UninstallApp](uninstallapp-operation.md)
    
- [GetAppManifests](getappmanifests.md)
    
- [Операция GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)
    

