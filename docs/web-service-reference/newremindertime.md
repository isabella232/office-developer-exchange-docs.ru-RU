---
title: невреминдертиме
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: Элемент Невреминдертиме указывает новое время напоминания.
ms.openlocfilehash: a10f7e481b474501f33dba4c09060766568952b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465956"
---
# <a name="newremindertime"></a><span data-ttu-id="9a7f1-103">невреминдертиме</span><span class="sxs-lookup"><span data-stu-id="9a7f1-103">NewReminderTime</span></span>

<span data-ttu-id="9a7f1-104">Элемент **невреминдертиме** указывает новое время напоминания.</span><span class="sxs-lookup"><span data-stu-id="9a7f1-104">The **NewReminderTime** element specifies a new time for a reminder.</span></span> 
  
```XML
<NewReminderTime/>
```

 <span data-ttu-id="9a7f1-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="9a7f1-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a7f1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9a7f1-106">Attributes and elements</span></span>

<span data-ttu-id="9a7f1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9a7f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a7f1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9a7f1-108">Attributes</span></span>

<span data-ttu-id="9a7f1-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9a7f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a7f1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9a7f1-110">Child elements</span></span>

<span data-ttu-id="9a7f1-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9a7f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9a7f1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9a7f1-112">Parent elements</span></span>

[<span data-ttu-id="9a7f1-113">реминдеритемактион</span><span class="sxs-lookup"><span data-stu-id="9a7f1-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="9a7f1-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9a7f1-114">Text value</span></span>

<span data-ttu-id="9a7f1-115">Текстовое значение элемента **невреминдертиме** — новое время напоминания.</span><span class="sxs-lookup"><span data-stu-id="9a7f1-115">The text value of the **NewReminderTime** element is a new time for the reminder.</span></span> <span data-ttu-id="9a7f1-116">Элемент **невреминдертиме** используется, [когда элемент "](actiontype-reminderactiontype.md) элемент" имеет значение **отсрочки**, чтобы отложить напоминание.</span><span class="sxs-lookup"><span data-stu-id="9a7f1-116">The **NewReminderTime** element is used when the [ActionType](actiontype-reminderactiontype.md) element is set to **Snooze**, in order to delay the reminder.</span></span> <span data-ttu-id="9a7f1-117">Значение Невреминдертиме должно быть больше, чем [ReminderTime](remindertime.md) , возвращенное [операцией](getreminders-operation.md) **NewReminderTime** .</span><span class="sxs-lookup"><span data-stu-id="9a7f1-117">The value of the **NewReminderTime** must be greater than the [ReminderTime](remindertime.md) returned by the [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a7f1-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="9a7f1-118">Remarks</span></span>

<span data-ttu-id="9a7f1-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9a7f1-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9a7f1-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9a7f1-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a7f1-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9a7f1-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a7f1-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9a7f1-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9a7f1-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9a7f1-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9a7f1-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9a7f1-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="9a7f1-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9a7f1-125">Validation File</span></span>  <br/> |<span data-ttu-id="9a7f1-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9a7f1-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9a7f1-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9a7f1-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a7f1-128">False</span><span class="sxs-lookup"><span data-stu-id="9a7f1-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a7f1-129">См. также</span><span class="sxs-lookup"><span data-stu-id="9a7f1-129">See also</span></span>



[<span data-ttu-id="9a7f1-130">реминдеритемактион</span><span class="sxs-lookup"><span data-stu-id="9a7f1-130">ReminderItemAction</span></span>](reminderitemaction.md)


- [<span data-ttu-id="9a7f1-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9a7f1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

