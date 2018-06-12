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
description: Элемент PercentComplete описывает состояние завершения задачи.
ms.openlocfilehash: 18e53221ecdf60df195445ed7692c03795bdcc1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834717"
---
# <a name="percentcomplete"></a><span data-ttu-id="0bcb7-103">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="0bcb7-103">PercentComplete</span></span>

<span data-ttu-id="0bcb7-104">Элемент **PercentComplete** описывает состояние завершения задачи.</span><span class="sxs-lookup"><span data-stu-id="0bcb7-104">The **PercentComplete** element describes the completion status of a task.</span></span> 
  
```xml
<PercentComplete/>
```

 <span data-ttu-id="0bcb7-105">**Двойная**</span><span class="sxs-lookup"><span data-stu-id="0bcb7-105">**double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bcb7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0bcb7-106">Attributes and elements</span></span>

<span data-ttu-id="0bcb7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0bcb7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bcb7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0bcb7-108">Attributes</span></span>

<span data-ttu-id="0bcb7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0bcb7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bcb7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0bcb7-110">Child elements</span></span>

<span data-ttu-id="0bcb7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="0bcb7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0bcb7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0bcb7-112">Parent elements</span></span>

|<span data-ttu-id="0bcb7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0bcb7-113">**Element**</span></span>|<span data-ttu-id="0bcb7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0bcb7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bcb7-115">Задача</span><span class="sxs-lookup"><span data-stu-id="0bcb7-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="0bcb7-116">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bcb7-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0bcb7-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0bcb7-117">Text value</span></span>

<span data-ttu-id="0bcb7-118">Текстовое значение, которое представляет собой целое число между 0 и 100 является обязательным.</span><span class="sxs-lookup"><span data-stu-id="0bcb7-118">A text value that represents an integer between 0 and 100 is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0bcb7-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="0bcb7-119">Remarks</span></span>

<span data-ttu-id="0bcb7-120">Установка **PercentComplete** 100 имеет тот же эффект, как установка элемент [CompleteDate](completedate.md) или установка элемент [состояние](status.md) значение **завершено**.</span><span class="sxs-lookup"><span data-stu-id="0bcb7-120">Setting **PercentComplete** to 100 has the same effect as setting the [CompleteDate](completedate.md) element or setting the [Status](status.md) element to **Completed**.</span></span> <span data-ttu-id="0bcb7-121">В запросе, что наборов по крайней мере два из этих свойств, последнего обработанного свойство определяет значение, заданное для этих элементов.</span><span class="sxs-lookup"><span data-stu-id="0bcb7-121">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="0bcb7-122">К примеру Если **PercentComplete** равно 100, [CompleteDate](completedate.md) — 1 января 2007 г и имеет [состояние](status.md) NotStarted и свойства, передаваемых в следующем порядке, влияние будет присвоено [состояние](status.md) задачи NotStarted, [ CompleteDate](completedate.md) **значение null**, а **PercentComplete** 0.</span><span class="sxs-lookup"><span data-stu-id="0bcb7-122">For example, if **PercentComplete** is 100, [CompleteDate](completedate.md) is January 1, 2007, and [Status](status.md) is NotStarted, and the properties are streamed in this order, the effect will be to set the [Status](status.md) of the task to NotStarted, the [CompleteDate](completedate.md) to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="0bcb7-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0bcb7-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bcb7-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0bcb7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bcb7-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0bcb7-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0bcb7-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0bcb7-126">Schema Name</span></span>  <br/> |<span data-ttu-id="0bcb7-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0bcb7-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="0bcb7-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0bcb7-128">Validation File</span></span>  <br/> |<span data-ttu-id="0bcb7-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0bcb7-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0bcb7-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0bcb7-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="0bcb7-131">False</span><span class="sxs-lookup"><span data-stu-id="0bcb7-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bcb7-132">См. также</span><span class="sxs-lookup"><span data-stu-id="0bcb7-132">See also</span></span>



- [<span data-ttu-id="0bcb7-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0bcb7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0bcb7-134">Создание задач</span><span class="sxs-lookup"><span data-stu-id="0bcb7-134">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="0bcb7-135">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="0bcb7-135">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

