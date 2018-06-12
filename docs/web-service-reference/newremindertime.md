---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: Элемент NewReminderTime Указывает новое время для напоминания.
ms.openlocfilehash: 9f3f509942c673c916cc646cd9519240aef6ea06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834531"
---
# <a name="newremindertime"></a><span data-ttu-id="90d86-103">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="90d86-103">NewReminderTime</span></span>

<span data-ttu-id="90d86-104">Элемент **NewReminderTime** Указывает новое время для напоминания.</span><span class="sxs-lookup"><span data-stu-id="90d86-104">The **NewReminderTime** element specifies a new time for a reminder.</span></span> 
  
```XML
<NewReminderTime/>
```

 <span data-ttu-id="90d86-105">**string**</span><span class="sxs-lookup"><span data-stu-id="90d86-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90d86-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="90d86-106">Attributes and elements</span></span>

<span data-ttu-id="90d86-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="90d86-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90d86-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="90d86-108">Attributes</span></span>

<span data-ttu-id="90d86-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="90d86-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90d86-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="90d86-110">Child elements</span></span>

<span data-ttu-id="90d86-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="90d86-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="90d86-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="90d86-112">Parent elements</span></span>

[<span data-ttu-id="90d86-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="90d86-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="90d86-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="90d86-114">Text value</span></span>

<span data-ttu-id="90d86-115">Текстовое значение элемента **NewReminderTime** — это новое время оповещения.</span><span class="sxs-lookup"><span data-stu-id="90d86-115">The text value of the **NewReminderTime** element is a new time for the reminder.</span></span> <span data-ttu-id="90d86-116">Элемент **NewReminderTime** будет использоваться при элемент [Тип действия](actiontype-reminderactiontype.md) задано значение **отложить**, чтобы задержки напоминания.</span><span class="sxs-lookup"><span data-stu-id="90d86-116">The **NewReminderTime** element is used when the [ActionType](actiontype-reminderactiontype.md) element is set to **Snooze**, in order to delay the reminder.</span></span> <span data-ttu-id="90d86-117">Значение **NewReminderTime** должно быть больше, чем [ReminderTime](remindertime.md) , возвращенные [операцией GetReminders](getreminders-operation.md).</span><span class="sxs-lookup"><span data-stu-id="90d86-117">The value of the **NewReminderTime** must be greater than the [ReminderTime](remindertime.md) returned by the [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="90d86-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="90d86-118">Remarks</span></span>

<span data-ttu-id="90d86-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="90d86-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="90d86-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="90d86-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90d86-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="90d86-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90d86-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="90d86-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90d86-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="90d86-123">Schema Name</span></span>  <br/> |<span data-ttu-id="90d86-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="90d86-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="90d86-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="90d86-125">Validation File</span></span>  <br/> |<span data-ttu-id="90d86-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="90d86-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90d86-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="90d86-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="90d86-128">False</span><span class="sxs-lookup"><span data-stu-id="90d86-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90d86-129">См. также</span><span class="sxs-lookup"><span data-stu-id="90d86-129">See also</span></span>



[<span data-ttu-id="90d86-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="90d86-130">ReminderItemAction</span></span>](reminderitemaction.md)


- [<span data-ttu-id="90d86-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="90d86-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

