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
description: Операция DeleteItem удаляет элементы из хранилища Exchange.
ms.openlocfilehash: 87d7853daa5db0cd87b3f6469c228a584b4d9caf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762043"
---
# <a name="deleteitem-operation"></a><span data-ttu-id="fef96-103">Операция DeleteItem</span><span class="sxs-lookup"><span data-stu-id="fef96-103">DeleteItem operation</span></span>

<span data-ttu-id="fef96-104">Операция **DeleteItem** удаляет элементы из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="fef96-104">The **DeleteItem** operation deletes items in the Exchange store.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fef96-105">Если делегат пытается удалить элемент в почтовом ящике участника, задав для Диспосалтипе значение MoveToDeletedItems, возвращается сообщение об ошибке, которое включает код ошибки Еррорканнотделетеобжект для операции **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="fef96-105">An error response that includes the ErrorCannotDeleteObject error code will be returned for a **DeleteItem** operation when a delegate tries to delete an item in the principal's mailbox by setting the DisposalType to MoveToDeletedItems.</span></span> <span data-ttu-id="fef96-106">Чтобы удалить элемент, переместив его в папку "Удаленные", делегат должен использовать [операцию MoveItem](moveitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="fef96-106">To delete an item by moving it to the Deleted Items folder, a delegate must use the [MoveItem operation](moveitem-operation.md).</span></span> 
  
## <a name="deleteitem-request-example"></a><span data-ttu-id="fef96-107">Пример запроса DeleteItem</span><span class="sxs-lookup"><span data-stu-id="fef96-107">DeleteItem request example</span></span>

### <a name="description"></a><span data-ttu-id="fef96-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fef96-108">Description</span></span>

<span data-ttu-id="fef96-109">В приведенном ниже примере запроса **DeleteItem** показано, как выполнить окончательное удаление элемента из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="fef96-109">The following example of a **DeleteItem** request shows how to perform a hard delete of an item from a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fef96-110">Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="fef96-110">The item ID has been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fef96-111">Код</span><span class="sxs-lookup"><span data-stu-id="fef96-111">Code</span></span>

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

### <a name="request-elements"></a><span data-ttu-id="fef96-112">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="fef96-112">Request elements</span></span>

<span data-ttu-id="fef96-113">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fef96-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="fef96-114">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="fef96-114">DeleteItem</span></span>](deleteitem.md)
    
- [<span data-ttu-id="fef96-115">итемидс</span><span class="sxs-lookup"><span data-stu-id="fef96-115">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="fef96-116">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="fef96-116">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="fef96-117">Чтобы найти другие параметры сообщения Request операции **DeleteItem** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="fef96-117">To find other options for the request message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="fef96-118">Начните с элемента [DeleteItem](deleteitem.md) .</span><span class="sxs-lookup"><span data-stu-id="fef96-118">Start at the [DeleteItem](deleteitem.md) element.</span></span> 
  
## <a name="successful-deleteitem-response"></a><span data-ttu-id="fef96-119">Успешный ответ DeleteItem</span><span class="sxs-lookup"><span data-stu-id="fef96-119">Successful DeleteItem response</span></span>

### <a name="description"></a><span data-ttu-id="fef96-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fef96-120">Description</span></span>

<span data-ttu-id="fef96-121">В следующем примере показан успешный ответ на запрос **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="fef96-121">The following example shows a successful response to the **DeleteItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fef96-122">Код</span><span class="sxs-lookup"><span data-stu-id="fef96-122">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="fef96-123">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="fef96-123">Successful response elements</span></span>

<span data-ttu-id="fef96-124">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fef96-124">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="fef96-125">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="fef96-125">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fef96-126">делетеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="fef96-126">DeleteItemResponse</span></span>](deleteitemresponse.md)
    
- [<span data-ttu-id="fef96-127">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fef96-127">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fef96-128">делетеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fef96-128">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
    
- [<span data-ttu-id="fef96-129">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fef96-129">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="fef96-130">Чтобы найти другие параметры для ответного сообщения операции **DeleteItem** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="fef96-130">To find other options for the response message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="fef96-131">Начните с элемента [делетеитемреспонсе](deleteitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="fef96-131">Start at the [DeleteItemResponse](deleteitemresponse.md) element.</span></span> 
  
## <a name="deleteitem-error-response"></a><span data-ttu-id="fef96-132">Ответ об ошибке DeleteItem</span><span class="sxs-lookup"><span data-stu-id="fef96-132">DeleteItem error response</span></span>

### <a name="description"></a><span data-ttu-id="fef96-133">Описание</span><span class="sxs-lookup"><span data-stu-id="fef96-133">Description</span></span>

<span data-ttu-id="fef96-134">В следующем примере показан ответ об ошибке для запроса **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="fef96-134">The following example shows an error response to a **DeleteItem** request.</span></span> <span data-ttu-id="fef96-135">Ошибка была создана, так как Операция попыталась удалить элемент, который не был найден в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fef96-135">The error was created because the operation tried to delete an item that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fef96-136">Код</span><span class="sxs-lookup"><span data-stu-id="fef96-136">Code</span></span>

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

### <a name="error-response-elements"></a><span data-ttu-id="fef96-137">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="fef96-137">Error response elements</span></span>

<span data-ttu-id="fef96-138">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fef96-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="fef96-139">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="fef96-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fef96-140">делетеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="fef96-140">DeleteItemResponse</span></span>](deleteitemresponse.md)
    
- [<span data-ttu-id="fef96-141">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fef96-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fef96-142">делетеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fef96-142">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
    
- [<span data-ttu-id="fef96-143">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="fef96-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="fef96-144">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fef96-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fef96-145">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="fef96-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="fef96-146">Чтобы найти другие параметры сообщения об ошибке при выполнении операции **DeleteItem** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="fef96-146">To find other options for the error response message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="fef96-147">Начните с элемента [делетеитемреспонсе](deleteitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="fef96-147">Start at the [DeleteItemResponse](deleteitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fef96-148">См. также</span><span class="sxs-lookup"><span data-stu-id="fef96-148">See also</span></span>

- [<span data-ttu-id="fef96-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fef96-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="fef96-150">Удаление контактов</span><span class="sxs-lookup"><span data-stu-id="fef96-150">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)  
- [<span data-ttu-id="fef96-151">Удаление сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="fef96-151">Deleting E-mail Messages</span></span>](http://msdn.microsoft.com/library/c40f2f0b-dae0-412f-b716-727e8c0949b4%28Office.15%29.aspx) 
- [<span data-ttu-id="fef96-152">Удаление задач</span><span class="sxs-lookup"><span data-stu-id="fef96-152">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

