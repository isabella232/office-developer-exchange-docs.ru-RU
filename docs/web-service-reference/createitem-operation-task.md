---
title: Операция CreateItem (задача)
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
description: Операция CreateItem создает элементы Task в хранилище Exchange.
ms.openlocfilehash: 502108843193e7ed8377b0fade9e106ef3d1976c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457104"
---
# <a name="createitem-operation-task"></a><span data-ttu-id="f0cf0-103">Операция CreateItem (задача)</span><span class="sxs-lookup"><span data-stu-id="f0cf0-103">CreateItem operation (task)</span></span>

<span data-ttu-id="f0cf0-104">Операция CreateItem создает элементы Task в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-104">The CreateItem operation creates task items in the Exchange store.</span></span>
  
## <a name="task-createitem-request"></a><span data-ttu-id="f0cf0-105">Запрос CreateItem задачи</span><span class="sxs-lookup"><span data-stu-id="f0cf0-105">Task CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="f0cf0-106">Description</span><span class="sxs-lookup"><span data-stu-id="f0cf0-106">Description</span></span>

<span data-ttu-id="f0cf0-107">В приведенном ниже примере запроса CreateItem показано, как создать элемент задачи в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-107">The following example of a CreateItem request shows how to create a task item in a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="f0cf0-108">Код</span><span class="sxs-lookup"><span data-stu-id="f0cf0-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

### <a name="comments"></a><span data-ttu-id="f0cf0-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="f0cf0-109">Comments</span></span>

<span data-ttu-id="f0cf0-110">Запросы на повторяющиеся задачи изменяются при их получении на компьютере под управлением Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-110">Requests for recurring tasks are altered when they are received by the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span> <span data-ttu-id="f0cf0-111">Происходят следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="f0cf0-111">The following changes occur:</span></span>
  
- <span data-ttu-id="f0cf0-112">Только дата сохраняется в свойстве [StartDate (повторение)](startdate-recurrence.md) для интервала повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-112">Only the date is saved for the [StartDate (Recurrence)](startdate-recurrence.md) property of the recurrence range of the task.</span></span> <span data-ttu-id="f0cf0-113">Часть времени усекается.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-113">The time part is truncated.</span></span> 
    
- <span data-ttu-id="f0cf0-114">Свойство [StartDate (повторение)](startdate-recurrence.md) можно изменить в зависимости от расписания повторения.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-114">The [StartDate (Recurrence)](startdate-recurrence.md) property may be adjusted, depending on the recurrence pattern.</span></span> <span data-ttu-id="f0cf0-115">Например, если расписание повторения задано как каждый понедельник, а значение StartDate равно 26 октября 2006 г., то есть четверг, Дата начала StartDate составляет 30 октября 2006, то есть на следующий понедельник.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-115">For example, if the recurrence pattern is specified as every Monday and the StartDate is set to October 26, 2006, which is a Thursday, StartDate is adjusted to October 30, 2006, which is the next Monday.</span></span> 
    
- <span data-ttu-id="f0cf0-116">Если свойство [StartDate](startdate.md) задания задано, оно обновляется в соответствующем поле [StartDate (повторение)](startdate-recurrence.md) диапазона повторения.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-116">If the [StartDate](startdate.md) property of the task is set, it is updated to match the [StartDate (Recurrence)](startdate-recurrence.md) of the recurrence range.</span></span> <span data-ttu-id="f0cf0-117">Свойство [DueDate](duedate.md) задачи также обновляется в соответствии с новым [StartDate](startdate.md).</span><span class="sxs-lookup"><span data-stu-id="f0cf0-117">The [DueDate](duedate.md) property of the task is also updated based on the new [StartDate](startdate.md).</span></span>
    
- <span data-ttu-id="f0cf0-118">Если [StartDate](startdate.md) не задан, обновляется только свойство [DueDate](duedate.md) , которое будет иметь значение [StartDate (повторение)](startdate-recurrence.md) диапазона повторения.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-118">If the [StartDate](startdate.md) is not set, only the [DueDate](duedate.md) property is updated to match the [StartDate (Recurrence)](startdate-recurrence.md) of the recurrence range.</span></span> 
    
<span data-ttu-id="f0cf0-119">В следующей таблице показаны изменения, которые сервер клиентского доступа выполняет с повторяющейся задачей, у которой есть задача. повторять. шаблон каждого понедельника.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-119">The following table shows the changes that the Client Access server makes to a recurring task that has a Task.Recurrence.Pattern of every Monday.</span></span>
  
<span data-ttu-id="f0cf0-120">**Изменение повторяющейся задачи**</span><span class="sxs-lookup"><span data-stu-id="f0cf0-120">**Changes to a recurring task**</span></span>

|<span data-ttu-id="f0cf0-121">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="f0cf0-121">**Property**</span></span>|<span data-ttu-id="f0cf0-122">**Исходное значение**</span><span class="sxs-lookup"><span data-stu-id="f0cf0-122">**Original Value**</span></span>|<span data-ttu-id="f0cf0-123">**Обновленное значение**</span><span class="sxs-lookup"><span data-stu-id="f0cf0-123">**Updated Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f0cf0-124">Task. StartDate</span><span class="sxs-lookup"><span data-stu-id="f0cf0-124">Task.StartDate</span></span>  <br/> |<span data-ttu-id="f0cf0-125">1 января 2006 г.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-125">January 1, 2006</span></span>  <br/> |<span data-ttu-id="f0cf0-126">30 октября 2006 г.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-126">October 30, 2006</span></span>  <br/> |
|<span data-ttu-id="f0cf0-127">Task. DueDate</span><span class="sxs-lookup"><span data-stu-id="f0cf0-127">Task.DueDate</span></span>  <br/> |<span data-ttu-id="f0cf0-128">3 января 2006 г.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-128">January 3, 2006</span></span>  <br/> |<span data-ttu-id="f0cf0-129">1 ноября 2006 г.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-129">November 1, 2006</span></span>  <br/> |
|<span data-ttu-id="f0cf0-130">Task. повторяющуюся. Range. StartDate</span><span class="sxs-lookup"><span data-stu-id="f0cf0-130">Task.Recurrence.Range.StartDate</span></span>  <br/> |<span data-ttu-id="f0cf0-131">26 октября 2006 г.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-131">October 26, 2006</span></span>  <br/> |<span data-ttu-id="f0cf0-132">30 октября 2006 г.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-132">October 30, 2006</span></span>  <br/> |
   
<span data-ttu-id="f0cf0-133">По умолчанию, если папка назначения не указана, элементы задач создаются в папке "задачи".</span><span class="sxs-lookup"><span data-stu-id="f0cf0-133">By default, if a destination folder is not specified, task items are created in the Tasks folder.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="f0cf0-134">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="f0cf0-134">Request elements</span></span>

<span data-ttu-id="f0cf0-135">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="f0cf0-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f0cf0-136">CreateItem</span><span class="sxs-lookup"><span data-stu-id="f0cf0-136">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="f0cf0-137">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="f0cf0-137">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="f0cf0-138">Task</span><span class="sxs-lookup"><span data-stu-id="f0cf0-138">Task</span></span>](task.md)
    
- [<span data-ttu-id="f0cf0-139">Тема</span><span class="sxs-lookup"><span data-stu-id="f0cf0-139">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="f0cf0-140">DueDate</span><span class="sxs-lookup"><span data-stu-id="f0cf0-140">DueDate</span></span>](duedate.md)
    
- [<span data-ttu-id="f0cf0-141">Status</span><span class="sxs-lookup"><span data-stu-id="f0cf0-141">Status</span></span>](status.md)
    
## <a name="successful-task-createitem-response"></a><span data-ttu-id="f0cf0-142">Отклик об успешном выполнении операции CreateItem</span><span class="sxs-lookup"><span data-stu-id="f0cf0-142">Successful Task CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="f0cf0-143">Description</span><span class="sxs-lookup"><span data-stu-id="f0cf0-143">Description</span></span>

<span data-ttu-id="f0cf0-144">В следующем примере показан успешный ответ на запрос CreateItem.</span><span class="sxs-lookup"><span data-stu-id="f0cf0-144">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="f0cf0-145">Код</span><span class="sxs-lookup"><span data-stu-id="f0cf0-145">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="f0cf0-146">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="f0cf0-146">Successful response elements</span></span>

<span data-ttu-id="f0cf0-147">В ответ включаются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="f0cf0-147">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="f0cf0-148">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="f0cf0-148">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f0cf0-149">креатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="f0cf0-149">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="f0cf0-150">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f0cf0-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f0cf0-151">креатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f0cf0-151">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="f0cf0-152">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="f0cf0-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f0cf0-153">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="f0cf0-153">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="f0cf0-154">Task</span><span class="sxs-lookup"><span data-stu-id="f0cf0-154">Task</span></span>](task.md)
    
- [<span data-ttu-id="f0cf0-155">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="f0cf0-155">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="f0cf0-156">См. также</span><span class="sxs-lookup"><span data-stu-id="f0cf0-156">See also</span></span>



[<span data-ttu-id="f0cf0-157">Операция CreateItem</span><span class="sxs-lookup"><span data-stu-id="f0cf0-157">CreateItem operation</span></span>](createitem-operation.md)


[<span data-ttu-id="f0cf0-158">Создание задач</span><span class="sxs-lookup"><span data-stu-id="f0cf0-158">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="f0cf0-159">Обновление задач</span><span class="sxs-lookup"><span data-stu-id="f0cf0-159">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[<span data-ttu-id="f0cf0-160">Удаление задач</span><span class="sxs-lookup"><span data-stu-id="f0cf0-160">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

