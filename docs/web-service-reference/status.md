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
# <a name="status"></a><span data-ttu-id="7217e-103">Состояние</span><span class="sxs-lookup"><span data-stu-id="7217e-103">Status</span></span>

<span data-ttu-id="7217e-104">Элемент **Status** представляет состояние элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="7217e-104">The **Status** element represents the status of a task item.</span></span> 
  
```xml
<Status/>
```

 <span data-ttu-id="7217e-105">**TaskStatusType**</span><span class="sxs-lookup"><span data-stu-id="7217e-105">**TaskStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7217e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7217e-106">Attributes and elements</span></span>

<span data-ttu-id="7217e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7217e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7217e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7217e-108">Attributes</span></span>

<span data-ttu-id="7217e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7217e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7217e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7217e-110">Child elements</span></span>

<span data-ttu-id="7217e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7217e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7217e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7217e-112">Parent elements</span></span>

|<span data-ttu-id="7217e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7217e-113">**Element**</span></span>|<span data-ttu-id="7217e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7217e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7217e-115">Задача</span><span class="sxs-lookup"><span data-stu-id="7217e-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="7217e-116">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7217e-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7217e-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7217e-117">Text value</span></span>

<span data-ttu-id="7217e-118">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7217e-118">A text value is required.</span></span> <span data-ttu-id="7217e-119">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="7217e-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="7217e-120">NotStarted</span><span class="sxs-lookup"><span data-stu-id="7217e-120">NotStarted</span></span>
    
- <span data-ttu-id="7217e-121">InProgress</span><span class="sxs-lookup"><span data-stu-id="7217e-121">InProgress</span></span>
    
- <span data-ttu-id="7217e-122">Completed</span><span class="sxs-lookup"><span data-stu-id="7217e-122">Completed</span></span>
    
- <span data-ttu-id="7217e-123">WaitingOnOthers</span><span class="sxs-lookup"><span data-stu-id="7217e-123">WaitingOnOthers</span></span>
    
- <span data-ttu-id="7217e-124">Отложенное</span><span class="sxs-lookup"><span data-stu-id="7217e-124">Deferred</span></span>
    
## <a name="remarks"></a><span data-ttu-id="7217e-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="7217e-125">Remarks</span></span>

<span data-ttu-id="7217e-126">Установка [CompleteDate](completedate.md) имеет тот же эффект, что и установка [PercentComplete](percentcomplete.md) **состояние** значение **завершено**или 100.</span><span class="sxs-lookup"><span data-stu-id="7217e-126">Setting [CompleteDate](completedate.md) has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or **Status** to **Completed**.</span></span> <span data-ttu-id="7217e-127">В запросе, что наборов по крайней мере два из этих свойств, последнего обработанного свойство определяет значение, заданное для этих элементов.</span><span class="sxs-lookup"><span data-stu-id="7217e-127">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="7217e-128">Например, если **PercentComplete** 100, **CompleteDate** — 1/1/2007 и **состояния** NotStarted и свойства, передаваемых в следующем порядке, результат будет присвоено **состояние** задачи NotStarted, **CompleteDate ** **значение null**, а **PercentComplete** 0.</span><span class="sxs-lookup"><span data-stu-id="7217e-128">For example, if **PercentComplete** is 100, **CompleteDate** is 1/1/2007, and **Status** is NotStarted, and the properties are streamed in this order, the effect will be to set the **Status** of the task to NotStarted, the **CompleteDate** to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="7217e-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7217e-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7217e-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7217e-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7217e-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7217e-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7217e-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7217e-132">Schema Name</span></span>  <br/> |<span data-ttu-id="7217e-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7217e-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="7217e-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7217e-134">Validation File</span></span>  <br/> |<span data-ttu-id="7217e-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7217e-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7217e-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7217e-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="7217e-137">False</span><span class="sxs-lookup"><span data-stu-id="7217e-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7217e-138">См. также</span><span class="sxs-lookup"><span data-stu-id="7217e-138">See also</span></span>



- [<span data-ttu-id="7217e-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7217e-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7217e-140">Создание задач</span><span class="sxs-lookup"><span data-stu-id="7217e-140">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="7217e-141">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="7217e-141">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

