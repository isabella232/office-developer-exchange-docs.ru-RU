---
title: Тип действия (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: Тип действия элемент указывает действие, которое выполняется на оповещение.
ms.openlocfilehash: 361259f733756995fae2c2c2390013a728e475a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761327"
---
# <a name="actiontype-reminderactiontype"></a><span data-ttu-id="60cc6-103">Тип действия (ReminderActionType)</span><span class="sxs-lookup"><span data-stu-id="60cc6-103">ActionType (ReminderActionType)</span></span>

<span data-ttu-id="60cc6-104">**Тип действия** элемент указывает действие, которое выполняется на оповещение.</span><span class="sxs-lookup"><span data-stu-id="60cc6-104">The **ActionType** element specifies the action to take on the reminder.</span></span> 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 <span data-ttu-id="60cc6-105">**ReminderActionType**</span><span class="sxs-lookup"><span data-stu-id="60cc6-105">**ReminderActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60cc6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="60cc6-106">Attributes and elements</span></span>

<span data-ttu-id="60cc6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="60cc6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60cc6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="60cc6-108">Attributes</span></span>

<span data-ttu-id="60cc6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="60cc6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60cc6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="60cc6-110">Child elements</span></span>

<span data-ttu-id="60cc6-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="60cc6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="60cc6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="60cc6-112">Parent elements</span></span>

[<span data-ttu-id="60cc6-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="60cc6-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="60cc6-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="60cc6-114">Text value</span></span>

<span data-ttu-id="60cc6-115">Текстовое значение элемента **Тип действия** указывает действие, которое выполняется на оповещение.</span><span class="sxs-lookup"><span data-stu-id="60cc6-115">The text value of the **ActionType** element specifies the action to take on the reminder.</span></span> <span data-ttu-id="60cc6-116">Текстовое значение **Прекратить** указывает, что должны быть закрыты напоминания.</span><span class="sxs-lookup"><span data-stu-id="60cc6-116">The text value of **Dismiss** indicates the reminder should be dismissed.</span></span> <span data-ttu-id="60cc6-117">Текстовое значение **отложить** указывает, что напоминания следует вводить до времени, указанного в элементе [NewReminderTime](newremindertime.md) .</span><span class="sxs-lookup"><span data-stu-id="60cc6-117">The text value of **Snooze** indicates that the reminder should be delayed until the time specified by the [NewReminderTime](newremindertime.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="60cc6-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="60cc6-118">Remarks</span></span>

<span data-ttu-id="60cc6-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="60cc6-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="60cc6-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="60cc6-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60cc6-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="60cc6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60cc6-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="60cc6-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="60cc6-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="60cc6-123">Schema Name</span></span>  <br/> |<span data-ttu-id="60cc6-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="60cc6-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="60cc6-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="60cc6-125">Validation File</span></span>  <br/> |<span data-ttu-id="60cc6-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="60cc6-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="60cc6-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="60cc6-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="60cc6-128">False</span><span class="sxs-lookup"><span data-stu-id="60cc6-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60cc6-129">См. также</span><span class="sxs-lookup"><span data-stu-id="60cc6-129">See also</span></span>

- [<span data-ttu-id="60cc6-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="60cc6-130">ReminderItemAction</span></span>](reminderitemaction.md)
- [<span data-ttu-id="60cc6-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="60cc6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

