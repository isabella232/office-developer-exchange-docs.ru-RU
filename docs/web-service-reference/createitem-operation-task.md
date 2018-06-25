---
title: Операции CreateItem (задача)
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
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: Операции CreateItem создает элементы задачи в хранилище Exchange.
ms.openlocfilehash: 5a5203202071ae9391faa9348902424317ee96d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761896"
---
# <a name="createitem-operation-task"></a><span data-ttu-id="75a5a-103">Операции CreateItem (задача)</span><span class="sxs-lookup"><span data-stu-id="75a5a-103">CreateItem operation (task)</span></span>

<span data-ttu-id="75a5a-104">Операции CreateItem создает элементы задачи в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="75a5a-104">The CreateItem operation creates task items in the Exchange store.</span></span>
  
## <a name="task-createitem-request"></a><span data-ttu-id="75a5a-105">Запрос CreateItem задачи</span><span class="sxs-lookup"><span data-stu-id="75a5a-105">Task CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="75a5a-106">Описание</span><span class="sxs-lookup"><span data-stu-id="75a5a-106">Description</span></span>

<span data-ttu-id="75a5a-107">В следующем примере запрос CreateItem показано, как создать элемент задачи в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="75a5a-107">The following example of a CreateItem request shows how to create a task item in a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="75a5a-108">Программа</span><span class="sxs-lookup"><span data-stu-id="75a5a-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                MessageDisposition="SaveOnly">
      <Items>
        <t:Task>
          <t:Subject>My task</t:Subject>
          <t:DueDate>2006-10-26T21:32:52</t:DueDate>
          <t:Status>NotStarted</t:Status>
        </t:Task>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="75a5a-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="75a5a-109">Comments</span></span>

<span data-ttu-id="75a5a-110">Запросы для повторяющихся задач, предоставление при получении на компьютере, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="75a5a-110">Requests for recurring tasks are altered when they are received by the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span> <span data-ttu-id="75a5a-111">Происходят следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="75a5a-111">The following changes occur:</span></span>
  
- <span data-ttu-id="75a5a-112">Только дата сохраняется для свойства [StartDate (повторения)](startdate-recurrence.md) диапазона повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="75a5a-112">Only the date is saved for the [StartDate (Recurrence)](startdate-recurrence.md) property of the recurrence range of the task.</span></span> <span data-ttu-id="75a5a-113">Часть времени усекается.</span><span class="sxs-lookup"><span data-stu-id="75a5a-113">The time part is truncated.</span></span> 
    
- <span data-ttu-id="75a5a-114">Свойство [StartDate (повторения)](startdate-recurrence.md) могут быть изменены в зависимости от шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="75a5a-114">The [StartDate (Recurrence)](startdate-recurrence.md) property may be adjusted, depending on the recurrence pattern.</span></span> <span data-ttu-id="75a5a-115">Например, если повторов задается следующим каждый понедельник, StartDate задано значение 26 октября 2006 г., которая Четверг, корректируется StartDate 30 октября 2006 г., которая является следующий понедельник.</span><span class="sxs-lookup"><span data-stu-id="75a5a-115">For example, if the recurrence pattern is specified as every Monday and the StartDate is set to October 26, 2006, which is a Thursday, StartDate is adjusted to October 30, 2006, which is the next Monday.</span></span> 
    
- <span data-ttu-id="75a5a-116">Если значение свойства [StartDate](startdate.md) задачи, он обновляется в соответствии с [StartDate (повторения)](startdate-recurrence.md) диапазона повторения.</span><span class="sxs-lookup"><span data-stu-id="75a5a-116">If the [StartDate](startdate.md) property of the task is set, it is updated to match the [StartDate (Recurrence)](startdate-recurrence.md) of the recurrence range.</span></span> <span data-ttu-id="75a5a-117">Свойство [DueDate](duedate.md) задачи также обновляются на основании нового [StartDate](startdate.md).</span><span class="sxs-lookup"><span data-stu-id="75a5a-117">The [DueDate](duedate.md) property of the task is also updated based on the new [StartDate](startdate.md).</span></span>
    
- <span data-ttu-id="75a5a-118">Если установлено значение [StartDate](startdate.md) , только свойство [DueDate](duedate.md) обновляется в соответствии с [StartDate (повторения)](startdate-recurrence.md) диапазона повторения.</span><span class="sxs-lookup"><span data-stu-id="75a5a-118">If the [StartDate](startdate.md) is not set, only the [DueDate](duedate.md) property is updated to match the [StartDate (Recurrence)](startdate-recurrence.md) of the recurrence range.</span></span> 
    
<span data-ttu-id="75a5a-119">В следующей таблице перечислены необходимые изменения на сервере клиентского доступа вносятся в повторяющейся задачи, имеющей Task.Recurrence.Pattern каждый понедельник.</span><span class="sxs-lookup"><span data-stu-id="75a5a-119">The following table shows the changes that the Client Access server makes to a recurring task that has a Task.Recurrence.Pattern of every Monday.</span></span>
  
<span data-ttu-id="75a5a-120">**Изменения в повторяющейся задачи**</span><span class="sxs-lookup"><span data-stu-id="75a5a-120">**Changes to a recurring task**</span></span>

|<span data-ttu-id="75a5a-121">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="75a5a-121">**Property**</span></span>|<span data-ttu-id="75a5a-122">**Исходное значение**</span><span class="sxs-lookup"><span data-stu-id="75a5a-122">**Original Value**</span></span>|<span data-ttu-id="75a5a-123">**Обновленное значение**</span><span class="sxs-lookup"><span data-stu-id="75a5a-123">**Updated Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="75a5a-124">Task.StartDate</span><span class="sxs-lookup"><span data-stu-id="75a5a-124">Task.StartDate</span></span>  <br/> |<span data-ttu-id="75a5a-125">1 января 2006 г.</span><span class="sxs-lookup"><span data-stu-id="75a5a-125">January 1, 2006</span></span>  <br/> |<span data-ttu-id="75a5a-126">30 октября 2006 г.</span><span class="sxs-lookup"><span data-stu-id="75a5a-126">October 30, 2006</span></span>  <br/> |
|<span data-ttu-id="75a5a-127">Task.DueDate</span><span class="sxs-lookup"><span data-stu-id="75a5a-127">Task.DueDate</span></span>  <br/> |<span data-ttu-id="75a5a-128">3 января 2006 г.</span><span class="sxs-lookup"><span data-stu-id="75a5a-128">January 3, 2006</span></span>  <br/> |<span data-ttu-id="75a5a-129">1 ноября 2006 г.</span><span class="sxs-lookup"><span data-stu-id="75a5a-129">November 1, 2006</span></span>  <br/> |
|<span data-ttu-id="75a5a-130">Task.Recurrence.Range.StartDate</span><span class="sxs-lookup"><span data-stu-id="75a5a-130">Task.Recurrence.Range.StartDate</span></span>  <br/> |<span data-ttu-id="75a5a-131">26 октября 2006 г.</span><span class="sxs-lookup"><span data-stu-id="75a5a-131">October 26, 2006</span></span>  <br/> |<span data-ttu-id="75a5a-132">30 октября 2006 г.</span><span class="sxs-lookup"><span data-stu-id="75a5a-132">October 30, 2006</span></span>  <br/> |
   
<span data-ttu-id="75a5a-133">По умолчанию если не указан в целевую папку, элементы задачи создаются в папке задач.</span><span class="sxs-lookup"><span data-stu-id="75a5a-133">By default, if a destination folder is not specified, task items are created in the Tasks folder.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="75a5a-134">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="75a5a-134">Request elements</span></span>

<span data-ttu-id="75a5a-135">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="75a5a-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="75a5a-136">CreateItem</span><span class="sxs-lookup"><span data-stu-id="75a5a-136">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="75a5a-137">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="75a5a-137">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="75a5a-138">Задача</span><span class="sxs-lookup"><span data-stu-id="75a5a-138">Task</span></span>](task.md)
    
- [<span data-ttu-id="75a5a-139">Subject</span><span class="sxs-lookup"><span data-stu-id="75a5a-139">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="75a5a-140">DueDate</span><span class="sxs-lookup"><span data-stu-id="75a5a-140">DueDate</span></span>](duedate.md)
    
- [<span data-ttu-id="75a5a-141">Состояние</span><span class="sxs-lookup"><span data-stu-id="75a5a-141">Status</span></span>](status.md)
    
## <a name="successful-task-createitem-response"></a><span data-ttu-id="75a5a-142">Успешные задачу CreateItem ответа</span><span class="sxs-lookup"><span data-stu-id="75a5a-142">Successful Task CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="75a5a-143">Описание</span><span class="sxs-lookup"><span data-stu-id="75a5a-143">Description</span></span>

<span data-ttu-id="75a5a-144">В следующем примере показано успешного ответа на запрос CreateItem.</span><span class="sxs-lookup"><span data-stu-id="75a5a-144">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="75a5a-145">Программа</span><span class="sxs-lookup"><span data-stu-id="75a5a-145">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAE=" ChangeKey="EwAAABYA"/>
            </t:Task>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="75a5a-146">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="75a5a-146">Successful response elements</span></span>

<span data-ttu-id="75a5a-147">В ответе включены следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="75a5a-147">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="75a5a-148">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="75a5a-148">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="75a5a-149">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="75a5a-149">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="75a5a-150">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="75a5a-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="75a5a-151">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="75a5a-151">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="75a5a-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="75a5a-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="75a5a-153">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="75a5a-153">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="75a5a-154">Задача</span><span class="sxs-lookup"><span data-stu-id="75a5a-154">Task</span></span>](task.md)
    
- [<span data-ttu-id="75a5a-155">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="75a5a-155">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="75a5a-156">См. также</span><span class="sxs-lookup"><span data-stu-id="75a5a-156">See also</span></span>



[<span data-ttu-id="75a5a-157">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="75a5a-157">CreateItem operation</span></span>](createitem-operation.md)


[<span data-ttu-id="75a5a-158">Создание задач</span><span class="sxs-lookup"><span data-stu-id="75a5a-158">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="75a5a-159">Обновление задач</span><span class="sxs-lookup"><span data-stu-id="75a5a-159">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[<span data-ttu-id="75a5a-160">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="75a5a-160">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

