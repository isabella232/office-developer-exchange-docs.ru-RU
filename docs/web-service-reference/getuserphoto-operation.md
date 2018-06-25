---
title: Операция GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: Найдите сведения о веб-служб Exchange GetUserPhoto операции.
ms.openlocfilehash: 4465ac7115d96f5b6ef39e467663c9bf1c70e99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833694"
---
# <a name="getuserphoto-operation"></a>Операция GetUserPhoto

Найдите сведения о **GetUserPhoto** операции веб-служб Exchange. 
  
Операция **GetUserPhoto** получает фото пользователя из доменных служб Active Directory (AD DS). 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getuserphoto-operation"></a>С помощью операции GetUserPhoto

Операция **RemoveContactFromImList** — это простые операции, которая принимает размер запрошенного фотографии и адреса электронной почты пользователя и возвращает поток фотографий в ответе. 
  
> [!NOTE]
> Веб-служб Exchange имеет SOAP и операции на основе REST, для получения фотографии пользователя. Сведения об интерфейсе REST [фотографии пользователя с помощью веб-служб Exchange в Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)см. 
  
### <a name="getuserphoto-operation-soap-headers"></a>Заголовки SOAP GetUserPhoto операции

Операция **GetUserPhoto** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Этот заголовок можно применять к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a>Пример запроса GetUserPhoto операции: получение фото пользователя

В следующем примере запрос операции **GetUserPhoto** показано, как получить фото пользователя. В этом примере выполняется запрос фотографию пользователя, который является 48 x 48 пикселей. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

В приглашении на SOAP body используются следующие элементы:
  
- [GetUserPhoto](getuserphoto.md)
    
- [Электронной почты (строка)](email-string.md)
    
- [SizeRequested](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a>Успешные операции ответа GetUserPhoto

В следующем примере показано успешные ответ на операцию **GetUserPhoto** для получения фото пользователя. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

В ответе SOAP body используются следующие элементы:
  
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [HasChanged](haschanged.md)
    
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a>Ошибка операции GetUserPhoto ответа

Конверт SOAP не возвращает код ошибки при попытке получить фото пользователя адреса электронной почты, который не существует в организации. 500 код состояния HTTP будут возвращены в ответ, чтобы указать, что запрос не удалось выполнить. 
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)   
- [Получение фотографий с помощью веб-служб Exchange в Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

