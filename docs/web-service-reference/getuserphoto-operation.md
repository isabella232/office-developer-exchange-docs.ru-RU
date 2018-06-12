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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833694"
---
# <a name="getuserphoto-operation"></a><span data-ttu-id="315b0-103">Операция GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="315b0-103">GetUserPhoto operation</span></span>

<span data-ttu-id="315b0-104">Найдите сведения о **GetUserPhoto** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="315b0-104">Find information about the **GetUserPhoto** EWS operation.</span></span> 
  
<span data-ttu-id="315b0-105">Операция **GetUserPhoto** получает фото пользователя из доменных служб Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="315b0-105">The **GetUserPhoto** operation gets a user photo from Active Directory Domain Services (AD DS).</span></span> 
  
<span data-ttu-id="315b0-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="315b0-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getuserphoto-operation"></a><span data-ttu-id="315b0-107">С помощью операции GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="315b0-107">Using the GetUserPhoto operation</span></span>

<span data-ttu-id="315b0-108">Операция **RemoveContactFromImList** — это простые операции, которая принимает размер запрошенного фотографии и адреса электронной почты пользователя и возвращает поток фотографий в ответе.</span><span class="sxs-lookup"><span data-stu-id="315b0-108">The **RemoveContactFromImList** operation is a simple operation that accepts a user's email address and the requested photo size and returns the photo stream in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="315b0-109">Веб-служб Exchange имеет SOAP и операции на основе REST, для получения фотографии пользователя.</span><span class="sxs-lookup"><span data-stu-id="315b0-109">EWS has both a SOAP and a REST-based operation to get user photos.</span></span> <span data-ttu-id="315b0-110">Сведения об интерфейсе REST [фотографии пользователя с помощью веб-служб Exchange в Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)см.</span><span class="sxs-lookup"><span data-stu-id="315b0-110">For information about the REST interface, see [Get user photos by using EWS in Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx).</span></span> 
  
### <a name="getuserphoto-operation-soap-headers"></a><span data-ttu-id="315b0-111">Заголовки SOAP GetUserPhoto операции</span><span class="sxs-lookup"><span data-stu-id="315b0-111">GetUserPhoto operation SOAP headers</span></span>

<span data-ttu-id="315b0-112">Операция **GetUserPhoto** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="315b0-112">The **GetUserPhoto** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="315b0-113">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="315b0-113">**Header name**</span></span>|<span data-ttu-id="315b0-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="315b0-114">**Element**</span></span>|<span data-ttu-id="315b0-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="315b0-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="315b0-116">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="315b0-116">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="315b0-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="315b0-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="315b0-118">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="315b0-118">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="315b0-119">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="315b0-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="315b0-120">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="315b0-120">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="315b0-121">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="315b0-121">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="315b0-122">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="315b0-122">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="315b0-123">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="315b0-123">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a><span data-ttu-id="315b0-124">Пример запроса GetUserPhoto операции: получение фото пользователя</span><span class="sxs-lookup"><span data-stu-id="315b0-124">GetUserPhoto operation request example: Get a user's photo</span></span>

<span data-ttu-id="315b0-125">В следующем примере запрос операции **GetUserPhoto** показано, как получить фото пользователя.</span><span class="sxs-lookup"><span data-stu-id="315b0-125">The following example of a **GetUserPhoto** operation request shows how to get a user's photo.</span></span> <span data-ttu-id="315b0-126">В этом примере выполняется запрос фотографию пользователя, который является 48 x 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="315b0-126">This example requests a user photo that is 48x48 pixels.</span></span> 
  
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

<span data-ttu-id="315b0-127">В приглашении на SOAP body используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="315b0-127">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="315b0-128">GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="315b0-128">GetUserPhoto</span></span>](getuserphoto.md)
    
- [<span data-ttu-id="315b0-129">Электронной почты (строка)</span><span class="sxs-lookup"><span data-stu-id="315b0-129">Email (String)</span></span>](email-string.md)
    
- [<span data-ttu-id="315b0-130">SizeRequested</span><span class="sxs-lookup"><span data-stu-id="315b0-130">SizeRequested</span></span>](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a><span data-ttu-id="315b0-131">Успешные операции ответа GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="315b0-131">Successful GetUserPhoto operation response</span></span>

<span data-ttu-id="315b0-132">В следующем примере показано успешные ответ на операцию **GetUserPhoto** для получения фото пользователя.</span><span class="sxs-lookup"><span data-stu-id="315b0-132">The following example shows a successful response to a **GetUserPhoto** operation to get a user's photo.</span></span> 
  
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

<span data-ttu-id="315b0-133">В ответе SOAP body используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="315b0-133">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="315b0-134">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="315b0-134">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
- [<span data-ttu-id="315b0-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="315b0-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="315b0-136">HasChanged</span><span class="sxs-lookup"><span data-stu-id="315b0-136">HasChanged</span></span>](haschanged.md)
    
- [<span data-ttu-id="315b0-137">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="315b0-137">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a><span data-ttu-id="315b0-138">Ошибка операции GetUserPhoto ответа</span><span class="sxs-lookup"><span data-stu-id="315b0-138">GetUserPhoto operation error response</span></span>

<span data-ttu-id="315b0-139">Конверт SOAP не возвращает код ошибки при попытке получить фото пользователя адреса электронной почты, который не существует в организации.</span><span class="sxs-lookup"><span data-stu-id="315b0-139">The SOAP envelope will not return an error code if an attempt is made to get a user photo for an email address that doesn't exist in the organization.</span></span> <span data-ttu-id="315b0-140">500 код состояния HTTP будут возвращены в ответ, чтобы указать, что запрос не удалось выполнить.</span><span class="sxs-lookup"><span data-stu-id="315b0-140">A 500 HTTP status code will be returned in the response to indicate that the request was unsuccessful.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="315b0-141">См. также</span><span class="sxs-lookup"><span data-stu-id="315b0-141">See also</span></span>

- [<span data-ttu-id="315b0-142">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="315b0-142">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="315b0-143">Получение фотографий с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="315b0-143">Get user photos by using EWS in Exchange</span></span>](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

