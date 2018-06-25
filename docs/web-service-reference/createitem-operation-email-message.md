---
title: Операции CreateItem (сообщение электронной почты)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1
description: Операции CreateItem используется для создания сообщений электронной почты.
ms.openlocfilehash: 591209165cfbafc2d5f4036dd8fab6659523a044
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761893"
---
# <a name="createitem-operation-email-message"></a><span data-ttu-id="8c762-103">Операции CreateItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="8c762-103">CreateItem operation (email message)</span></span>

<span data-ttu-id="8c762-104">Операции CreateItem используется для создания сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8c762-104">The CreateItem operation is used to create e-mail messages.</span></span>
  
## <a name="createitem-request-example"></a><span data-ttu-id="8c762-105">Пример запроса CreateItem</span><span class="sxs-lookup"><span data-stu-id="8c762-105">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="8c762-106">Описание</span><span class="sxs-lookup"><span data-stu-id="8c762-106">Description</span></span>

<span data-ttu-id="8c762-107">Запрос CreateItem в следующем примере показано, как создать новое сообщение электронной почты, отправлять сообщения и сохраните его в папке "Черновики".</span><span class="sxs-lookup"><span data-stu-id="8c762-107">The following example of a CreateItem request shows how to create a new e-mail message, send the message, and save a copy of it in the drafts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="8c762-108">Программа</span><span class="sxs-lookup"><span data-stu-id="8c762-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem MessageDisposition="SendAndSaveCopy" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </SavedItemFolderId>
      <Items>
        <t:Message>
          <t:ItemClass>IPM.Note</t:ItemClass>
          <t:Subject>Project Action</t:Subject>
          <t:Body BodyType="Text">Priority - Update specification</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sschmidt@example.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
          <t:IsRead>false</t:IsRead>
        </t:Message>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="8c762-109">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="8c762-109">Request elements</span></span>

<span data-ttu-id="8c762-110">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="8c762-110">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="8c762-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="8c762-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="8c762-112">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="8c762-112">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="8c762-113">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="8c762-113">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="8c762-114">Message</span><span class="sxs-lookup"><span data-stu-id="8c762-114">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="8c762-115">ItemClass</span><span class="sxs-lookup"><span data-stu-id="8c762-115">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="8c762-116">Subject</span><span class="sxs-lookup"><span data-stu-id="8c762-116">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="8c762-117">Body</span><span class="sxs-lookup"><span data-stu-id="8c762-117">Body</span></span>](body.md)
    
- [<span data-ttu-id="8c762-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="8c762-118">ToRecipients</span></span>](torecipients.md)
    
- [<span data-ttu-id="8c762-119">Mailbox</span><span class="sxs-lookup"><span data-stu-id="8c762-119">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="8c762-120">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="8c762-120">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="8c762-121">IsRead</span><span class="sxs-lookup"><span data-stu-id="8c762-121">IsRead</span></span>](isread.md)
    
<span data-ttu-id="8c762-122">Чтобы найти другие параметры для сообщения запроса на выполнение операции CreateItem, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="8c762-122">To find other options for the request message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="8c762-123">Начать с [CreateItem](createitem.md) элемента.</span><span class="sxs-lookup"><span data-stu-id="8c762-123">Start at the [CreateItem](createitem.md) element.</span></span> 
  
## <a name="successful-createitem-response"></a><span data-ttu-id="8c762-124">Успешные CreateItem ответа</span><span class="sxs-lookup"><span data-stu-id="8c762-124">Successful CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="8c762-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8c762-125">Description</span></span>

<span data-ttu-id="8c762-126">В следующем примере показано успешного ответа на запрос CreateItem.</span><span class="sxs-lookup"><span data-stu-id="8c762-126">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="8c762-127">Программа</span><span class="sxs-lookup"><span data-stu-id="8c762-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="8c762-128">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="8c762-128">Successful response elements</span></span>

<span data-ttu-id="8c762-129">В ответе включены следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="8c762-129">The following elements are included in the response:</span></span> 
  
- [<span data-ttu-id="8c762-130">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="8c762-130">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="8c762-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8c762-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8c762-132">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8c762-132">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="8c762-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8c762-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8c762-134">Элементы</span><span class="sxs-lookup"><span data-stu-id="8c762-134">Items</span></span>](items.md)
    
<span data-ttu-id="8c762-135">Чтобы найти другие параметры в сообщении ответа операции CreateItem, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="8c762-135">To find other options for the response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="8c762-136">Запустите в элементе [CreateItemResponse](createitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="8c762-136">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="error-createitem-response"></a><span data-ttu-id="8c762-137">Ошибка CreateItem ответа</span><span class="sxs-lookup"><span data-stu-id="8c762-137">Error CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="8c762-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8c762-138">Description</span></span>

<span data-ttu-id="8c762-139">В следующем примере показано ошибочный ответ на запрос CreateItem.</span><span class="sxs-lookup"><span data-stu-id="8c762-139">The following example shows an error response to a CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="8c762-140">Программа</span><span class="sxs-lookup"><span data-stu-id="8c762-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account.</m:MessageText>
          <m:ResponseCode>ErrorSendAsDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="8c762-141">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="8c762-141">Error response elements</span></span>

<span data-ttu-id="8c762-142">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="8c762-142">The following elements are used in the error response:</span></span> 
  
- [<span data-ttu-id="8c762-143">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="8c762-143">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="8c762-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8c762-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8c762-145">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8c762-145">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="8c762-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="8c762-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="8c762-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8c762-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8c762-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8c762-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="8c762-149">Элементы</span><span class="sxs-lookup"><span data-stu-id="8c762-149">Items</span></span>](items.md)
    
<span data-ttu-id="8c762-150">Чтобы найти другие параметры в сообщении об ошибке ответа операции CreateItem, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="8c762-150">To find other options for the error response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="8c762-151">Запустите в элементе [CreateItemResponse](createitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="8c762-151">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8c762-152">См. также</span><span class="sxs-lookup"><span data-stu-id="8c762-152">See also</span></span>



[<span data-ttu-id="8c762-153">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="8c762-153">CreateItem operation</span></span>](createitem-operation.md)

