---
title: Операция GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: Поиск сведений о GetUserPhotoной операции EWS.
ms.openlocfilehash: 6769842d31519f0aac2cf9bda10c1cab70558301
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461816"
---
# <a name="getuserphoto-operation"></a>Операция GetUserPhoto

Поиск сведений о **GetUserPhotoной** операции EWS. 
  
Операция **GetUserPhoto** получает фотографию пользователя из доменных служб Active Directory (AD DS). 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getuserphoto-operation"></a>Использование операции GetUserPhoto

Операция **RemoveContactFromImList** — это простая операция, которая принимает адрес электронной почты пользователя и запрошенный размер фотографии и возвращает поток фото в ответе. 
  
> [!NOTE]
> Для получения фотографий пользователей у веб EWS есть как SOAP, так и операция REST. Сведения о интерфейсе REST приведены в статье [Получение фотографий пользователей с помощью EWS в Exchange](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx). 
  
### <a name="getuserphoto-operation-soap-headers"></a>Заголовки SOAP операции GetUserPhoto

Операция **GetUserPhoto** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a>Пример запроса операции GetUserPhoto: получение фотографии пользователя

В приведенном ниже примере запроса операции **GetUserPhoto** показано, как получить фотографию пользователя. В этом примере запрашивается фотография пользователя 48x48 пикселей. 
  
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

В теле SOAP запроса используются следующие элементы:
  
- [GetUserPhoto](getuserphoto.md)
    
- [Электронная почта (строка)](email-string.md)
    
- [сизерекуестед](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a>Успешный отклик операции GetUserPhoto

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

В теле SOAP отклика используются следующие элементы:
  
- [жетусерфотореспонсе](getuserphotoresponse.md)
    
- [респонсекоде](responsecode.md)
    
- [хасчанжед](haschanged.md)
    
- [жетусерфотореспонсе](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a>Ответ об ошибке операции GetUserPhoto

При попытке получить фотографию пользователя для адреса электронной почты, который не существует в Организации, конверт SOAP не будет возвращать код ошибки. Код состояния HTTP 500 будет возвращен в ответе, чтобы указать, что запрос был выполнен неудачно. 
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)   
- [Получение фотографий пользователей с помощью EWS в Exchange](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

