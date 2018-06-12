---
title: Операции GetItem (задача)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 8265dd06-1752-4470-8074-5f0e3e970f52
description: Операции GetItem используется для получения задачи из хранилища Exchange.
ms.openlocfilehash: 412710f32ed8702e1a28a596833c3a7e47e3ed76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762840"
---
# <a name="getitem-operation-task"></a><span data-ttu-id="ac3e0-103">Операции GetItem (задача)</span><span class="sxs-lookup"><span data-stu-id="ac3e0-103">GetItem operation (task)</span></span>

<span data-ttu-id="ac3e0-104">Операции GetItem используется для получения задачи из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac3e0-104">The GetItem operation is used to get tasks from the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ac3e0-105">Замечания</span><span class="sxs-lookup"><span data-stu-id="ac3e0-105">Remarks</span></span>

<span data-ttu-id="ac3e0-106">Формат запроса GetItem для задач, совпадает с GetItem для любой другой тип элемента.</span><span class="sxs-lookup"><span data-stu-id="ac3e0-106">The format of the GetItem request for tasks is the same as GetItem for any other item type.</span></span> <span data-ttu-id="ac3e0-107">Единственное отличие заключается в котором можно запросить дополнительные свойства в фигуре ответа.</span><span class="sxs-lookup"><span data-stu-id="ac3e0-107">The only difference is in which additional properties can be requested within the response shape.</span></span> <span data-ttu-id="ac3e0-108">Такие дополнительные свойства должен быть свойства, связанные с задач или расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="ac3e0-108">Such additional properties must either be task-related properties or extended properties.</span></span>
  
## <a name="task-getitem-request-example"></a><span data-ttu-id="ac3e0-109">Пример запроса GetItem задач</span><span class="sxs-lookup"><span data-stu-id="ac3e0-109">Task GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="ac3e0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ac3e0-110">Description</span></span>

<span data-ttu-id="ac3e0-111">Приведенный ниже запрос GetItem показано, как получить элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="ac3e0-111">The following example of a GetItem request shows how to get a task item.</span></span>
  
### <a name="code"></a><span data-ttu-id="ac3e0-112">Программа</span><span class="sxs-lookup"><span data-stu-id="ac3e0-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAEFkb..."/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ac3e0-113">Комментарии</span><span class="sxs-lookup"><span data-stu-id="ac3e0-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="ac3e0-114">Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ac3e0-114">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ac3e0-115">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="ac3e0-115">Request elements</span></span>

<span data-ttu-id="ac3e0-116">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ac3e0-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ac3e0-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="ac3e0-117">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="ac3e0-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="ac3e0-118">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="ac3e0-119">BaseShape</span><span class="sxs-lookup"><span data-stu-id="ac3e0-119">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="ac3e0-120">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="ac3e0-120">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="ac3e0-121">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="ac3e0-121">ItemId</span></span>](itemid.md)
    
## <a name="task-getitem-response-example"></a><span data-ttu-id="ac3e0-122">Пример ответа GetItem задач</span><span class="sxs-lookup"><span data-stu-id="ac3e0-122">Task GetItem response example</span></span>

### <a name="description"></a><span data-ttu-id="ac3e0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ac3e0-123">Description</span></span>

<span data-ttu-id="ac3e0-124">В следующем примере показано успешного ответа на запрос GetItem.</span><span class="sxs-lookup"><span data-stu-id="ac3e0-124">The following example shows a successful response to a GetItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="ac3e0-125">Программа</span><span class="sxs-lookup"><span data-stu-id="ac3e0-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAEA=" ChangeKey="EwAAAB"/>
              <t:ParentFolderId Id="AAAtAEFkbWl=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Task</t:ItemClass>
              <t:Subject>Buy new shoes</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text"/>
              <t:DateTimeReceived>2006-09-15T15:23:08Z</t:DateTimeReceived>
              <t:Size>153</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>true</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-09-15T15:23:08Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-09-15T15:23:08Z</t:DateTimeCreated>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en-US</t:Culture>
              <t:ChangeCount>1</t:ChangeCount>
              <t:IsComplete>false</t:IsComplete>
              <t:IsRecurring>false</t:IsRecurring>
              <t:PercentComplete>0</t:PercentComplete>
              <t:Status>NotStarted</t:Status>
              <t:StatusDescription>Not Started</t:StatusDescription>
            </t:Task>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ac3e0-126">Комментарии</span><span class="sxs-lookup"><span data-stu-id="ac3e0-126">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="ac3e0-127">Идентификаторы элементов и папок и ключей изменения URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ac3e0-127">The item and folder identifiers and change keys have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="ac3e0-128">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="ac3e0-128">Successful response elements</span></span>

<span data-ttu-id="ac3e0-129">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ac3e0-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ac3e0-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ac3e0-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ac3e0-131">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="ac3e0-131">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="ac3e0-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ac3e0-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ac3e0-133">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ac3e0-133">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="ac3e0-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ac3e0-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ac3e0-135">Элементы</span><span class="sxs-lookup"><span data-stu-id="ac3e0-135">Items</span></span>](items.md)
    
- [<span data-ttu-id="ac3e0-136">Задача</span><span class="sxs-lookup"><span data-stu-id="ac3e0-136">Task</span></span>](task.md)
    
- [<span data-ttu-id="ac3e0-137">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="ac3e0-137">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="ac3e0-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ac3e0-138">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="ac3e0-139">ItemClass</span><span class="sxs-lookup"><span data-stu-id="ac3e0-139">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="ac3e0-140">Subject</span><span class="sxs-lookup"><span data-stu-id="ac3e0-140">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="ac3e0-141">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="ac3e0-141">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="ac3e0-142">Body</span><span class="sxs-lookup"><span data-stu-id="ac3e0-142">Body</span></span>](body.md)
    
- [<span data-ttu-id="ac3e0-143">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="ac3e0-143">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="ac3e0-144">Размер</span><span class="sxs-lookup"><span data-stu-id="ac3e0-144">Size</span></span>](size.md)
    
- [<span data-ttu-id="ac3e0-145">Важность</span><span class="sxs-lookup"><span data-stu-id="ac3e0-145">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="ac3e0-146">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="ac3e0-146">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="ac3e0-147">IsDraft</span><span class="sxs-lookup"><span data-stu-id="ac3e0-147">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="ac3e0-148">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="ac3e0-148">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="ac3e0-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="ac3e0-149">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="ac3e0-150">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="ac3e0-150">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="ac3e0-151">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="ac3e0-151">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="ac3e0-152">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="ac3e0-152">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="ac3e0-153">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="ac3e0-153">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="ac3e0-154">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="ac3e0-154">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="ac3e0-155">ChangeCount</span><span class="sxs-lookup"><span data-stu-id="ac3e0-155">ChangeCount</span></span>](changecount.md)
    
- [<span data-ttu-id="ac3e0-156">IsComplete</span><span class="sxs-lookup"><span data-stu-id="ac3e0-156">IsComplete</span></span>](iscomplete.md)
    
- [<span data-ttu-id="ac3e0-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="ac3e0-157">IsRecurring</span></span>](isrecurring.md)
    
- [<span data-ttu-id="ac3e0-158">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="ac3e0-158">PercentComplete</span></span>](percentcomplete.md)
    
- [<span data-ttu-id="ac3e0-159">Состояние</span><span class="sxs-lookup"><span data-stu-id="ac3e0-159">Status</span></span>](status.md)
    
- [<span data-ttu-id="ac3e0-160">StatusDescription</span><span class="sxs-lookup"><span data-stu-id="ac3e0-160">StatusDescription</span></span>](statusdescription.md)
    
## <a name="see-also"></a><span data-ttu-id="ac3e0-161">См. также</span><span class="sxs-lookup"><span data-stu-id="ac3e0-161">See also</span></span>



[<span data-ttu-id="ac3e0-162">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="ac3e0-162">GetItem operation</span></span>](getitem-operation.md)


[<span data-ttu-id="ac3e0-163">Создание задач</span><span class="sxs-lookup"><span data-stu-id="ac3e0-163">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="ac3e0-164">Обновление задач</span><span class="sxs-lookup"><span data-stu-id="ac3e0-164">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[<span data-ttu-id="ac3e0-165">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="ac3e0-165">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

