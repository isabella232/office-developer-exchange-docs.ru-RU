---
title: Операция DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 3e26c416-fa12-476e-bfd2-5c1f4bb7b348
description: Операция DeleteItem удаляет элементы в хранилище Exchange.
ms.openlocfilehash: 87d7853daa5db0cd87b3f6469c228a584b4d9caf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762043"
---
# <a name="deleteitem-operation"></a><span data-ttu-id="bf1ff-103">Операция DeleteItem</span><span class="sxs-lookup"><span data-stu-id="bf1ff-103">DeleteItem operation</span></span>

<span data-ttu-id="bf1ff-104">Операция **DeleteItem** удаляет элементы в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf1ff-104">The **DeleteItem** operation deletes items in the Exchange store.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bf1ff-105">Ответ на ошибку, которая включает в себя код ошибки ErrorCannotDeleteObject будут возвращены для выполнения операции **DeleteItem** при попытке удалить элемент в почтовом ящике участника путем установки для параметра MoveToDeletedItems DisposalType делегата.</span><span class="sxs-lookup"><span data-stu-id="bf1ff-105">An error response that includes the ErrorCannotDeleteObject error code will be returned for a **DeleteItem** operation when a delegate tries to delete an item in the principal's mailbox by setting the DisposalType to MoveToDeletedItems.</span></span> <span data-ttu-id="bf1ff-106">Чтобы удалить элемент путем перемещения в папку «Удаленные», делегата необходимо использовать [MoveItem операции](moveitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="bf1ff-106">To delete an item by moving it to the Deleted Items folder, a delegate must use the [MoveItem operation](moveitem-operation.md).</span></span> 
  
## <a name="deleteitem-request-example"></a><span data-ttu-id="bf1ff-107">Пример запроса DeleteItem</span><span class="sxs-lookup"><span data-stu-id="bf1ff-107">DeleteItem request example</span></span>

### <a name="description"></a><span data-ttu-id="bf1ff-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bf1ff-108">Description</span></span>

<span data-ttu-id="bf1ff-109">В следующем примере запрос **DeleteItem** показано, как выполнить окончательного удаления элемента из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bf1ff-109">The following example of a **DeleteItem** request shows how to perform a hard delete of an item from a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bf1ff-110">Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="bf1ff-110">The item ID has been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bf1ff-111">Программа</span><span class="sxs-lookup"><span data-stu-id="bf1ff-111">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteItem DeleteType="HardDelete" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemIds>
        <t:ItemId Id="AS4AUn=="/>
      </ItemIds>
    </DeleteItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="bf1ff-112">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="bf1ff-112">Request elements</span></span>

<span data-ttu-id="bf1ff-113">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bf1ff-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="bf1ff-114">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="bf1ff-114">DeleteItem</span></span>](deleteitem.md)
    
- [<span data-ttu-id="bf1ff-115">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="bf1ff-115">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="bf1ff-116">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="bf1ff-116">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="bf1ff-117">Чтобы найти другие параметры для запроса **DeleteItem** операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="bf1ff-117">To find other options for the request message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="bf1ff-118">Начать с [DeleteItem](deleteitem.md) элемента.</span><span class="sxs-lookup"><span data-stu-id="bf1ff-118">Start at the [DeleteItem](deleteitem.md) element.</span></span> 
  
## <a name="successful-deleteitem-response"></a><span data-ttu-id="bf1ff-119">Успешные DeleteItem ответа</span><span class="sxs-lookup"><span data-stu-id="bf1ff-119">Successful DeleteItem response</span></span>

### <a name="description"></a><span data-ttu-id="bf1ff-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bf1ff-120">Description</span></span>

<span data-ttu-id="bf1ff-121">В следующем примере показано успешного ответа на запрос **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="bf1ff-121">The following example shows a successful response to the **DeleteItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bf1ff-122">Программа</span><span class="sxs-lookup"><span data-stu-id="bf1ff-122">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="bf1ff-123">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="bf1ff-123">Successful response elements</span></span>

<span data-ttu-id="bf1ff-124">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bf1ff-124">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="bf1ff-125">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bf1ff-125">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="bf1ff-126">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="bf1ff-126">DeleteItemResponse</span></span>](deleteitemresponse.md)
    
- [<span data-ttu-id="bf1ff-127">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bf1ff-127">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bf1ff-128">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bf1ff-128">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
    
- [<span data-ttu-id="bf1ff-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bf1ff-129">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="bf1ff-130">Чтобы найти другие параметры в сообщении ответа **DeleteItem** операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="bf1ff-130">To find other options for the response message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="bf1ff-131">Запустите в элементе [DeleteItemResponse](deleteitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="bf1ff-131">Start at the [DeleteItemResponse](deleteitemresponse.md) element.</span></span> 
  
## <a name="deleteitem-error-response"></a><span data-ttu-id="bf1ff-132">Ошибка DeleteItem ответа</span><span class="sxs-lookup"><span data-stu-id="bf1ff-132">DeleteItem error response</span></span>

### <a name="description"></a><span data-ttu-id="bf1ff-133">Описание</span><span class="sxs-lookup"><span data-stu-id="bf1ff-133">Description</span></span>

<span data-ttu-id="bf1ff-134">В следующем примере показано возврату ошибки **DeleteItem** запрос.</span><span class="sxs-lookup"><span data-stu-id="bf1ff-134">The following example shows an error response to a **DeleteItem** request.</span></span> <span data-ttu-id="bf1ff-135">Ошибка была создана, поскольку операции пытались удалить элемент, который не найден в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf1ff-135">The error was created because the operation tried to delete an item that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bf1ff-136">Программа</span><span class="sxs-lookup"><span data-stu-id="bf1ff-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="bf1ff-137">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="bf1ff-137">Error response elements</span></span>

<span data-ttu-id="bf1ff-138">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bf1ff-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="bf1ff-139">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bf1ff-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="bf1ff-140">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="bf1ff-140">DeleteItemResponse</span></span>](deleteitemresponse.md)
    
- [<span data-ttu-id="bf1ff-141">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bf1ff-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bf1ff-142">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bf1ff-142">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
    
- [<span data-ttu-id="bf1ff-143">MessageText</span><span class="sxs-lookup"><span data-stu-id="bf1ff-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="bf1ff-144">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bf1ff-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bf1ff-145">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bf1ff-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="bf1ff-146">Чтобы найти другие параметры в сообщении об ошибке ответа **DeleteItem** операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="bf1ff-146">To find other options for the error response message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="bf1ff-147">Запустите в элементе [DeleteItemResponse](deleteitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="bf1ff-147">Start at the [DeleteItemResponse](deleteitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="bf1ff-148">См. также</span><span class="sxs-lookup"><span data-stu-id="bf1ff-148">See also</span></span>

- [<span data-ttu-id="bf1ff-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bf1ff-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="bf1ff-150">Удаление контактов</span><span class="sxs-lookup"><span data-stu-id="bf1ff-150">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)  
- [<span data-ttu-id="bf1ff-151">Удаление сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="bf1ff-151">Deleting E-mail Messages</span></span>](http://msdn.microsoft.com/library/c40f2f0b-dae0-412f-b716-727e8c0949b4%28Office.15%29.aspx) 
- [<span data-ttu-id="bf1ff-152">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="bf1ff-152">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

