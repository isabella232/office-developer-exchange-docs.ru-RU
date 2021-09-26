---
title: Операция GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: Сведения об операции GetUserPhoto EWS.
ms.openlocfilehash: 6dd1ce73d6291e60ce188b98b917a4c79ce792b5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547486"
---
# <a name="getuserphoto-operation"></a>Операция GetUserPhoto

Сведения об операции **GetUserPhoto** EWS. 
  
Операция **GetUserPhoto** получает фотографию пользователя из служб домена Active Directory (AD DS). 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getuserphoto-operation"></a>Использование операции GetUserPhoto

Операция **RemoveContactFromImList** — это простая операция, которая принимает адрес электронной почты пользователя и запрашиваемую фотографию и возвращает поток фотографий в ответ. 
  
> [!NOTE]
> EWS имеет как SOAP, так и операцию на основе REST для получения фотографий пользователей. Сведения об интерфейсе REST см. в фотоснимки пользователей [с помощью EWS в Exchange.](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx) 
  
### <a name="getuserphoto-operation-soap-headers"></a>Заготавлители мыла для операции GetUserPhoto

В **операции GetUserPhoto** можно использовать заглавные таблицы SOAP, указанные в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Этот заглавный заглавник применим к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Этот заглавный заглавник применим к ответу.  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a>Пример запроса на операцию GetUserPhoto: получить фотографию пользователя

В следующем примере запроса **на операцию GetUserPhoto** показано, как получить фотографию пользователя. В этом примере запрашивается фотография пользователя с размером 48x48 пикселей. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>user1@contoso.com</m:Email>
         <m:SizeRequested>HR48x48</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>
```

В корпусе SOAP запроса используются следующие элементы:
  
- [GetUserPhoto](getuserphoto.md)
    
- [Email (строка)](email-string.md)
    
- [SizeRequested](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a>Успешный ответ на операцию GetUserPhoto

В следующем примере показан успешный ответ на операцию **GetUserPhoto** для получения фотографии пользователя. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

В корпусе SOAP ответа используются следующие элементы:
  
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [HasChanged](haschanged.md)
    
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a>Ответ на ошибку операции GetUserPhoto

Конверт SOAP не возвращает код ошибки, если предпринята попытка получить фотографию пользователя для адреса электронной почты, который не существует в организации. Код состояния HTTP 500 будет возвращен в ответ, чтобы указать, что запрос был неудачным. 
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)   
- [Получение фотографий пользователей с помощью EWS в Exchange](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

