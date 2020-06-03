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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461816"
---
# <a name="getuserphoto-operation"></a><span data-ttu-id="0264b-103">Операция GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="0264b-103">GetUserPhoto operation</span></span>

<span data-ttu-id="0264b-104">Поиск сведений о **GetUserPhotoной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="0264b-104">Find information about the **GetUserPhoto** EWS operation.</span></span> 
  
<span data-ttu-id="0264b-105">Операция **GetUserPhoto** получает фотографию пользователя из доменных служб Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="0264b-105">The **GetUserPhoto** operation gets a user photo from Active Directory Domain Services (AD DS).</span></span> 
  
<span data-ttu-id="0264b-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0264b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getuserphoto-operation"></a><span data-ttu-id="0264b-107">Использование операции GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="0264b-107">Using the GetUserPhoto operation</span></span>

<span data-ttu-id="0264b-108">Операция **RemoveContactFromImList** — это простая операция, которая принимает адрес электронной почты пользователя и запрошенный размер фотографии и возвращает поток фото в ответе.</span><span class="sxs-lookup"><span data-stu-id="0264b-108">The **RemoveContactFromImList** operation is a simple operation that accepts a user's email address and the requested photo size and returns the photo stream in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0264b-109">Для получения фотографий пользователей у веб EWS есть как SOAP, так и операция REST.</span><span class="sxs-lookup"><span data-stu-id="0264b-109">EWS has both a SOAP and a REST-based operation to get user photos.</span></span> <span data-ttu-id="0264b-110">Сведения о интерфейсе REST приведены в статье [Получение фотографий пользователей с помощью EWS в Exchange](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="0264b-110">For information about the REST interface, see [Get user photos by using EWS in Exchange](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx).</span></span> 
  
### <a name="getuserphoto-operation-soap-headers"></a><span data-ttu-id="0264b-111">Заголовки SOAP операции GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="0264b-111">GetUserPhoto operation SOAP headers</span></span>

<span data-ttu-id="0264b-112">Операция **GetUserPhoto** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="0264b-112">The **GetUserPhoto** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0264b-113">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="0264b-113">**Header name**</span></span>|<span data-ttu-id="0264b-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0264b-114">**Element**</span></span>|<span data-ttu-id="0264b-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0264b-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0264b-116">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="0264b-116">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0264b-117">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="0264b-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0264b-118">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="0264b-118">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0264b-119">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="0264b-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0264b-120">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="0264b-120">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0264b-121">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="0264b-121">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0264b-122">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="0264b-122">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0264b-123">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="0264b-123">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a><span data-ttu-id="0264b-124">Пример запроса операции GetUserPhoto: получение фотографии пользователя</span><span class="sxs-lookup"><span data-stu-id="0264b-124">GetUserPhoto operation request example: Get a user's photo</span></span>

<span data-ttu-id="0264b-125">В приведенном ниже примере запроса операции **GetUserPhoto** показано, как получить фотографию пользователя.</span><span class="sxs-lookup"><span data-stu-id="0264b-125">The following example of a **GetUserPhoto** operation request shows how to get a user's photo.</span></span> <span data-ttu-id="0264b-126">В этом примере запрашивается фотография пользователя 48x48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="0264b-126">This example requests a user photo that is 48x48 pixels.</span></span> 
  
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

<span data-ttu-id="0264b-127">В теле SOAP запроса используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0264b-127">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="0264b-128">GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="0264b-128">GetUserPhoto</span></span>](getuserphoto.md)
    
- [<span data-ttu-id="0264b-129">Электронная почта (строка)</span><span class="sxs-lookup"><span data-stu-id="0264b-129">Email (String)</span></span>](email-string.md)
    
- [<span data-ttu-id="0264b-130">сизерекуестед</span><span class="sxs-lookup"><span data-stu-id="0264b-130">SizeRequested</span></span>](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a><span data-ttu-id="0264b-131">Успешный отклик операции GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="0264b-131">Successful GetUserPhoto operation response</span></span>

<span data-ttu-id="0264b-132">В следующем примере показан успешный ответ на операцию **GetUserPhoto** для получения фотографии пользователя.</span><span class="sxs-lookup"><span data-stu-id="0264b-132">The following example shows a successful response to a **GetUserPhoto** operation to get a user's photo.</span></span> 
  
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

<span data-ttu-id="0264b-133">В теле SOAP отклика используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="0264b-133">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="0264b-134">жетусерфотореспонсе</span><span class="sxs-lookup"><span data-stu-id="0264b-134">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
- [<span data-ttu-id="0264b-135">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="0264b-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0264b-136">хасчанжед</span><span class="sxs-lookup"><span data-stu-id="0264b-136">HasChanged</span></span>](haschanged.md)
    
- [<span data-ttu-id="0264b-137">жетусерфотореспонсе</span><span class="sxs-lookup"><span data-stu-id="0264b-137">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a><span data-ttu-id="0264b-138">Ответ об ошибке операции GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="0264b-138">GetUserPhoto operation error response</span></span>

<span data-ttu-id="0264b-139">При попытке получить фотографию пользователя для адреса электронной почты, который не существует в Организации, конверт SOAP не будет возвращать код ошибки.</span><span class="sxs-lookup"><span data-stu-id="0264b-139">The SOAP envelope will not return an error code if an attempt is made to get a user photo for an email address that doesn't exist in the organization.</span></span> <span data-ttu-id="0264b-140">Код состояния HTTP 500 будет возвращен в ответе, чтобы указать, что запрос был выполнен неудачно.</span><span class="sxs-lookup"><span data-stu-id="0264b-140">A 500 HTTP status code will be returned in the response to indicate that the request was unsuccessful.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0264b-141">См. также</span><span class="sxs-lookup"><span data-stu-id="0264b-141">See also</span></span>

- [<span data-ttu-id="0264b-142">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="0264b-142">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="0264b-143">Получение фотографий пользователей с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="0264b-143">Get user photos by using EWS in Exchange</span></span>](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

