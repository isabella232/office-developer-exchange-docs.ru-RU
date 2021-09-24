---
title: Операция UninstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: Сведения об операции UninstallApp EWS.
ms.openlocfilehash: 8a301360b2b4c38d85e8c5be2e80c79378d0fd97
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527148"
---
# <a name="uninstallapp-operation"></a>Операция UninstallApp

Сведения об операции **UninstallApp** EWS. 
  
Операция **UninstallApp** анинсталирует почтовое приложение для Outlook. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-uninstallapp-operation"></a>Использование операции UninstallApp

Операция **UninstallApp** принимает один аргумент в запросе, который идентифицирует почтовое приложение, чтобы удалить. 
  
### <a name="uninstallapp-operation-soap-headers"></a>Заглавы операции UninstallApp

Операция **UninstallApp** может использовать заглавные таблицы SOAP, перечисленные в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Этот заглавный заглавник применим к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Этот заглавный заглавник применим к ответу.  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a>Пример запроса на операцию UninstallApp: удалить почтовое приложение в почтовом ящике

В следующем примере запроса операции **UninstallApp** показано, как удалить почтовое приложение с помощью идентификатора приложения. Идентификатор приложения можно найти в манифесте приложения, возвращаемом операцией [GetAppManifests.](getappmanifests-operation.md)
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:UninstallApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
      </m:UninstallApp>
   </soap:Body>
</soap:Envelope>
```

Тело SOAP запроса содержит следующие элементы:
  
- [UninstallApp](uninstallapp.md)
    
- [ID (строка)](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a>Успешный ответ на операцию UninstallApp

В следующем примере показан успешный ответ на запрос операции **UninstallApp,** чтобы удалить почтовое приложение. 
  
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
      <UninstallAppResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP ответа содержит следующие элементы:
  
- [UninstallAppResponse](uninstallappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a>Ответ на ошибку операции UninstallApp

В следующем примере показан ответ на ошибку на запрос операции **UninstallApp.** Это ответ на запрос о том, чтобы удалить почтовое приложение, которое уже было неустановлено. 
  
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
      <UninstallAppResponse ResponseClass="Error" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1c50226d-04b5-4ab2-9fcd-42e236b59e4b can't be found.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP ответа на ошибку содержит следующие элементы:
  
- [UninstallAppResponse](uninstallappresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Дополнительные коды ошибок, общие для EWS и специфические для этой операции, см. [в ответе.](responsecode.md)
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция InstallApp](installapp-operation.md)
    
- [Операция DisableApp](disableapp-operation.md)
    
- [GetAppManifests](getappmanifests.md)
    
- [Операция GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)
    

