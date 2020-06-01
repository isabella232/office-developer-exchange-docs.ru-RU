---
title: PercentComplete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PercentComplete
api_type:
- schema
ms.assetid: 58a67f8a-c4dc-42dc-97ae-a9e5cc672d2d
description: Элемент PercentComplete описывает состояние выполнения задачи.
ms.openlocfilehash: b7dd2f18bd3ef6addeb6d3a7b004510f35b9cb3d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456887"
---
# <a name="percentcomplete"></a><span data-ttu-id="e4fd3-103">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="e4fd3-103">PercentComplete</span></span>

<span data-ttu-id="e4fd3-104">Элемент **PercentComplete** описывает состояние выполнения задачи.</span><span class="sxs-lookup"><span data-stu-id="e4fd3-104">The **PercentComplete** element describes the completion status of a task.</span></span> 
  
```xml
<PercentComplete/>
```

 <span data-ttu-id="e4fd3-105">**двойной**</span><span class="sxs-lookup"><span data-stu-id="e4fd3-105">**double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4fd3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e4fd3-106">Attributes and elements</span></span>

<span data-ttu-id="e4fd3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e4fd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4fd3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e4fd3-108">Attributes</span></span>

<span data-ttu-id="e4fd3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4fd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4fd3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e4fd3-110">Child elements</span></span>

<span data-ttu-id="e4fd3-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4fd3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4fd3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e4fd3-112">Parent elements</span></span>

|<span data-ttu-id="e4fd3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e4fd3-113">**Element**</span></span>|<span data-ttu-id="e4fd3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4fd3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4fd3-115">Задача</span><span class="sxs-lookup"><span data-stu-id="e4fd3-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="e4fd3-116">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4fd3-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e4fd3-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e4fd3-117">Text value</span></span>

<span data-ttu-id="e4fd3-118">Текстовое значение, представляющее целое число от 0 до 100, обязательно.</span><span class="sxs-lookup"><span data-stu-id="e4fd3-118">A text value that represents an integer between 0 and 100 is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e4fd3-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="e4fd3-119">Remarks</span></span>

<span data-ttu-id="e4fd3-120">Установка **PercentComplete** в 100 имеет то же самое, что и установка элемента [комплетедате](completedate.md) или установка для элемента [Status](status.md) значения **Completed**.</span><span class="sxs-lookup"><span data-stu-id="e4fd3-120">Setting **PercentComplete** to 100 has the same effect as setting the [CompleteDate](completedate.md) element or setting the [Status](status.md) element to **Completed**.</span></span> <span data-ttu-id="e4fd3-121">В запросе, который задает по крайней мере два из этих свойств, Последнее обработанное свойство будет определять значение, заданное для этих элементов.</span><span class="sxs-lookup"><span data-stu-id="e4fd3-121">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="e4fd3-122">Например, если для **PercentComplete** задано значение 100, [Комплетедате](completedate.md) — 1 января 2007, а [состояние](status.md) — NotStarted, а свойства передаются в потоке в этом порядке, то результатом будет установка для задачи [состояния](status.md) NotStarted, [комплетедате](completedate.md) — **null**, а **PercentComplete** — 0.</span><span class="sxs-lookup"><span data-stu-id="e4fd3-122">For example, if **PercentComplete** is 100, [CompleteDate](completedate.md) is January 1, 2007, and [Status](status.md) is NotStarted, and the properties are streamed in this order, the effect will be to set the [Status](status.md) of the task to NotStarted, the [CompleteDate](completedate.md) to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="e4fd3-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e4fd3-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4fd3-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e4fd3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4fd3-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e4fd3-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4fd3-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e4fd3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e4fd3-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e4fd3-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4fd3-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e4fd3-128">Validation File</span></span>  <br/> |<span data-ttu-id="e4fd3-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e4fd3-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4fd3-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e4fd3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4fd3-131">False</span><span class="sxs-lookup"><span data-stu-id="e4fd3-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4fd3-132">См. также</span><span class="sxs-lookup"><span data-stu-id="e4fd3-132">See also</span></span>



- [<span data-ttu-id="e4fd3-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e4fd3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e4fd3-134">Создание задач</span><span class="sxs-lookup"><span data-stu-id="e4fd3-134">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="e4fd3-135">Удаление задач</span><span class="sxs-lookup"><span data-stu-id="e4fd3-135">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

