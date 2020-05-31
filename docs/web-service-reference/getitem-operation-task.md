---
title: Операция GetItem (задача)
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
description: Операция GetItem используется для получения задач из хранилища Exchange.
ms.openlocfilehash: 412710f32ed8702e1a28a596833c3a7e47e3ed76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762840"
---
# <a name="getitem-operation-task"></a><span data-ttu-id="9e7cf-103">Операция GetItem (задача)</span><span class="sxs-lookup"><span data-stu-id="9e7cf-103">GetItem operation (task)</span></span>

<span data-ttu-id="9e7cf-104">Операция GetItem используется для получения задач из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e7cf-104">The GetItem operation is used to get tasks from the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e7cf-105">Примечания</span><span class="sxs-lookup"><span data-stu-id="9e7cf-105">Remarks</span></span>

<span data-ttu-id="9e7cf-106">Формат запроса GetItem для задач такой же, что и GetItem для любого другого типа элемента.</span><span class="sxs-lookup"><span data-stu-id="9e7cf-106">The format of the GetItem request for tasks is the same as GetItem for any other item type.</span></span> <span data-ttu-id="9e7cf-107">Единственное отличие заключается в том, что дополнительные свойства можно запросить в фигуре ответа.</span><span class="sxs-lookup"><span data-stu-id="9e7cf-107">The only difference is in which additional properties can be requested within the response shape.</span></span> <span data-ttu-id="9e7cf-108">Такие дополнительные свойства должны быть свойствами или расширенными свойствами, связанными с задачей.</span><span class="sxs-lookup"><span data-stu-id="9e7cf-108">Such additional properties must either be task-related properties or extended properties.</span></span>
  
## <a name="task-getitem-request-example"></a><span data-ttu-id="9e7cf-109">Пример запроса задачи GetItem</span><span class="sxs-lookup"><span data-stu-id="9e7cf-109">Task GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="9e7cf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9e7cf-110">Description</span></span>

<span data-ttu-id="9e7cf-111">В приведенном ниже примере запроса GetItem показано, как получить элемент задачи.</span><span class="sxs-lookup"><span data-stu-id="9e7cf-111">The following example of a GetItem request shows how to get a task item.</span></span>
  
### <a name="code"></a><span data-ttu-id="9e7cf-112">Код</span><span class="sxs-lookup"><span data-stu-id="9e7cf-112">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="9e7cf-113">Comments</span><span class="sxs-lookup"><span data-stu-id="9e7cf-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="9e7cf-114">Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="9e7cf-114">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="9e7cf-115">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="9e7cf-115">Request elements</span></span>

<span data-ttu-id="9e7cf-116">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="9e7cf-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="9e7cf-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="9e7cf-117">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="9e7cf-118">итемшапе</span><span class="sxs-lookup"><span data-stu-id="9e7cf-118">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="9e7cf-119">басешапе</span><span class="sxs-lookup"><span data-stu-id="9e7cf-119">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="9e7cf-120">итемидс</span><span class="sxs-lookup"><span data-stu-id="9e7cf-120">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="9e7cf-121">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="9e7cf-121">ItemId</span></span>](itemid.md)
    
## <a name="task-getitem-response-example"></a><span data-ttu-id="9e7cf-122">Пример отклика "задача GetItem"</span><span class="sxs-lookup"><span data-stu-id="9e7cf-122">Task GetItem response example</span></span>

### <a name="description"></a><span data-ttu-id="9e7cf-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9e7cf-123">Description</span></span>

<span data-ttu-id="9e7cf-124">В следующем примере показан успешный ответ на запрос GetItem.</span><span class="sxs-lookup"><span data-stu-id="9e7cf-124">The following example shows a successful response to a GetItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="9e7cf-125">Код</span><span class="sxs-lookup"><span data-stu-id="9e7cf-125">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="9e7cf-126">Comments</span><span class="sxs-lookup"><span data-stu-id="9e7cf-126">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="9e7cf-127">Идентификаторы элементов и папок, а также ключи изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="9e7cf-127">The item and folder identifiers and change keys have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="9e7cf-128">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="9e7cf-128">Successful response elements</span></span>

<span data-ttu-id="9e7cf-129">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="9e7cf-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="9e7cf-130">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="9e7cf-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="9e7cf-131">жетитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="9e7cf-131">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="9e7cf-132">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="9e7cf-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="9e7cf-133">жетитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9e7cf-133">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="9e7cf-134">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="9e7cf-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9e7cf-135">Items</span><span class="sxs-lookup"><span data-stu-id="9e7cf-135">Items</span></span>](items.md)
    
- [<span data-ttu-id="9e7cf-136">Task</span><span class="sxs-lookup"><span data-stu-id="9e7cf-136">Task</span></span>](task.md)
    
- [<span data-ttu-id="9e7cf-137">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="9e7cf-137">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="9e7cf-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9e7cf-138">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="9e7cf-139">ItemClass</span><span class="sxs-lookup"><span data-stu-id="9e7cf-139">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="9e7cf-140">Тема</span><span class="sxs-lookup"><span data-stu-id="9e7cf-140">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="9e7cf-141">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="9e7cf-141">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="9e7cf-142">Основной текст</span><span class="sxs-lookup"><span data-stu-id="9e7cf-142">Body</span></span>](body.md)
    
- [<span data-ttu-id="9e7cf-143">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="9e7cf-143">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="9e7cf-144">Размер</span><span class="sxs-lookup"><span data-stu-id="9e7cf-144">Size</span></span>](size.md)
    
- [<span data-ttu-id="9e7cf-145">Importance</span><span class="sxs-lookup"><span data-stu-id="9e7cf-145">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="9e7cf-146">Отправлено</span><span class="sxs-lookup"><span data-stu-id="9e7cf-146">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="9e7cf-147">Черновик</span><span class="sxs-lookup"><span data-stu-id="9e7cf-147">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="9e7cf-148">исфромме</span><span class="sxs-lookup"><span data-stu-id="9e7cf-148">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="9e7cf-149">исресенд</span><span class="sxs-lookup"><span data-stu-id="9e7cf-149">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="9e7cf-150">исунмодифиед</span><span class="sxs-lookup"><span data-stu-id="9e7cf-150">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="9e7cf-151">датетимесент</span><span class="sxs-lookup"><span data-stu-id="9e7cf-151">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="9e7cf-152">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="9e7cf-152">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="9e7cf-153">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="9e7cf-153">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="9e7cf-154">Culture</span><span class="sxs-lookup"><span data-stu-id="9e7cf-154">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="9e7cf-155">чанжекаунт</span><span class="sxs-lookup"><span data-stu-id="9e7cf-155">ChangeCount</span></span>](changecount.md)
    
- [<span data-ttu-id="9e7cf-156">Выполнение</span><span class="sxs-lookup"><span data-stu-id="9e7cf-156">IsComplete</span></span>](iscomplete.md)
    
- [<span data-ttu-id="9e7cf-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="9e7cf-157">IsRecurring</span></span>](isrecurring.md)
    
- [<span data-ttu-id="9e7cf-158">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="9e7cf-158">PercentComplete</span></span>](percentcomplete.md)
    
- [<span data-ttu-id="9e7cf-159">Состояние</span><span class="sxs-lookup"><span data-stu-id="9e7cf-159">Status</span></span>](status.md)
    
- [<span data-ttu-id="9e7cf-160">статусдескриптион</span><span class="sxs-lookup"><span data-stu-id="9e7cf-160">StatusDescription</span></span>](statusdescription.md)
    
## <a name="see-also"></a><span data-ttu-id="9e7cf-161">См. также</span><span class="sxs-lookup"><span data-stu-id="9e7cf-161">See also</span></span>



[<span data-ttu-id="9e7cf-162">Операция GetItem</span><span class="sxs-lookup"><span data-stu-id="9e7cf-162">GetItem operation</span></span>](getitem-operation.md)


[<span data-ttu-id="9e7cf-163">Создание задач</span><span class="sxs-lookup"><span data-stu-id="9e7cf-163">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="9e7cf-164">Обновление задач</span><span class="sxs-lookup"><span data-stu-id="9e7cf-164">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[<span data-ttu-id="9e7cf-165">Удаление задач</span><span class="sxs-lookup"><span data-stu-id="9e7cf-165">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

