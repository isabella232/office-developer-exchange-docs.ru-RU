---
title: Состояние
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 80121e41-291b-4fc0-a55e-6f677d4b5fb5
description: Элемент Status представляет состояние элемента задачи.
ms.openlocfilehash: 224b61913a5ae8e5b4aa0d756a9f2488df2741bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835584"
---
# <a name="status"></a><span data-ttu-id="6d9d9-103">Состояние</span><span class="sxs-lookup"><span data-stu-id="6d9d9-103">Status</span></span>

<span data-ttu-id="6d9d9-104">Элемент **Status** представляет состояние элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="6d9d9-104">The **Status** element represents the status of a task item.</span></span> 
  
```xml
<Status/>
```

 <span data-ttu-id="6d9d9-105">**таскстатустипе**</span><span class="sxs-lookup"><span data-stu-id="6d9d9-105">**TaskStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d9d9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6d9d9-106">Attributes and elements</span></span>

<span data-ttu-id="6d9d9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6d9d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d9d9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6d9d9-108">Attributes</span></span>

<span data-ttu-id="6d9d9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6d9d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d9d9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6d9d9-110">Child elements</span></span>

<span data-ttu-id="6d9d9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6d9d9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d9d9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6d9d9-112">Parent elements</span></span>

|<span data-ttu-id="6d9d9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6d9d9-113">**Element**</span></span>|<span data-ttu-id="6d9d9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6d9d9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d9d9-115">Задача</span><span class="sxs-lookup"><span data-stu-id="6d9d9-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="6d9d9-116">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d9d9-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6d9d9-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6d9d9-117">Text value</span></span>

<span data-ttu-id="6d9d9-118">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="6d9d9-118">A text value is required.</span></span> <span data-ttu-id="6d9d9-119">Ниже приведены возможные текстовые значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="6d9d9-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="6d9d9-120">NotStarted</span><span class="sxs-lookup"><span data-stu-id="6d9d9-120">NotStarted</span></span>
    
- <span data-ttu-id="6d9d9-121">InProgress</span><span class="sxs-lookup"><span data-stu-id="6d9d9-121">InProgress</span></span>
    
- <span data-ttu-id="6d9d9-122">Completed</span><span class="sxs-lookup"><span data-stu-id="6d9d9-122">Completed</span></span>
    
- <span data-ttu-id="6d9d9-123">ваитингоносерс</span><span class="sxs-lookup"><span data-stu-id="6d9d9-123">WaitingOnOthers</span></span>
    
- <span data-ttu-id="6d9d9-124">Deferred</span><span class="sxs-lookup"><span data-stu-id="6d9d9-124">Deferred</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6d9d9-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="6d9d9-125">Remarks</span></span>

<span data-ttu-id="6d9d9-126">Установка [комплетедате](completedate.md) имеет тот же последствия, что и установка [PercentComplete](percentcomplete.md) в 100 или **состояние** на " **завершено**".</span><span class="sxs-lookup"><span data-stu-id="6d9d9-126">Setting [CompleteDate](completedate.md) has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or **Status** to **Completed**.</span></span> <span data-ttu-id="6d9d9-127">В запросе, который задает по крайней мере два из этих свойств, Последнее обработанное свойство будет определять значение, заданное для этих элементов.</span><span class="sxs-lookup"><span data-stu-id="6d9d9-127">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="6d9d9-128">Например, если для параметра **PercentComplete** задано значение 100, **комплетедате** — 1/1/2007, а **состояние** — NotStarted, а свойства передаются в потоке в этом порядке, то результатом будет установка для задачи **состояния** NotStarted, **комплетедате** — **null**, а **PercentComplete** — 0.</span><span class="sxs-lookup"><span data-stu-id="6d9d9-128">For example, if **PercentComplete** is 100, **CompleteDate** is 1/1/2007, and **Status** is NotStarted, and the properties are streamed in this order, the effect will be to set the **Status** of the task to NotStarted, the **CompleteDate** to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="6d9d9-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6d9d9-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d9d9-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6d9d9-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d9d9-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6d9d9-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d9d9-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6d9d9-132">Schema Name</span></span>  <br/> |<span data-ttu-id="6d9d9-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6d9d9-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="6d9d9-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6d9d9-134">Validation File</span></span>  <br/> |<span data-ttu-id="6d9d9-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6d9d9-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d9d9-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6d9d9-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d9d9-137">False</span><span class="sxs-lookup"><span data-stu-id="6d9d9-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d9d9-138">См. также</span><span class="sxs-lookup"><span data-stu-id="6d9d9-138">See also</span></span>



- [<span data-ttu-id="6d9d9-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6d9d9-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6d9d9-140">Создание задач</span><span class="sxs-lookup"><span data-stu-id="6d9d9-140">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="6d9d9-141">Удаление задач</span><span class="sxs-lookup"><span data-stu-id="6d9d9-141">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

