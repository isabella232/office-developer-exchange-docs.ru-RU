---
title: ReminderGroup
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: Элемент ReminderGroup указывает, является ли напоминания для элемента календаря или задачи.
ms.openlocfilehash: d9d31cdab482d04149428021ad44cc742108053a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835060"
---
# <a name="remindergroup"></a><span data-ttu-id="56b0a-103">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="56b0a-103">ReminderGroup</span></span>

<span data-ttu-id="56b0a-104">Элемент **ReminderGroup** указывает, является ли напоминания для элемента календаря или задачи.</span><span class="sxs-lookup"><span data-stu-id="56b0a-104">The **ReminderGroup** element specifies whether the reminder is for a calendar item or a task.</span></span> 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 <span data-ttu-id="56b0a-105">**ReminderGroupType**</span><span class="sxs-lookup"><span data-stu-id="56b0a-105">**ReminderGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56b0a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="56b0a-106">Attributes and elements</span></span>

<span data-ttu-id="56b0a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="56b0a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56b0a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="56b0a-108">Attributes</span></span>

<span data-ttu-id="56b0a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="56b0a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56b0a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="56b0a-110">Child elements</span></span>

<span data-ttu-id="56b0a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="56b0a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="56b0a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="56b0a-112">Parent elements</span></span>

[<span data-ttu-id="56b0a-113">Памятки</span><span class="sxs-lookup"><span data-stu-id="56b0a-113">Reminder</span></span>](reminder.md)
  
## <a name="text-value"></a><span data-ttu-id="56b0a-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="56b0a-114">Text value</span></span>

<span data-ttu-id="56b0a-115">Текстовое значение элемента **ReminderGroup** — это тип группы памятки.</span><span class="sxs-lookup"><span data-stu-id="56b0a-115">The text value of the **ReminderGroup** element is the group type of the reminder.</span></span> <span data-ttu-id="56b0a-116">Текстовое значение **календаря** указывается напоминания для элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="56b0a-116">The text value of **Calendar** specifies that the reminder is for a calendar item.</span></span> <span data-ttu-id="56b0a-117">Текстовое значение **задач** указывается напоминания для элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="56b0a-117">The text value of **Task** specifies that the reminder is for a task item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="56b0a-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="56b0a-118">Remarks</span></span>

<span data-ttu-id="56b0a-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="56b0a-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="56b0a-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="56b0a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56b0a-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="56b0a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56b0a-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="56b0a-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56b0a-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="56b0a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="56b0a-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="56b0a-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="56b0a-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="56b0a-125">Validation File</span></span>  <br/> |<span data-ttu-id="56b0a-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="56b0a-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56b0a-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="56b0a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="56b0a-128">False</span><span class="sxs-lookup"><span data-stu-id="56b0a-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56b0a-129">См. также</span><span class="sxs-lookup"><span data-stu-id="56b0a-129">See also</span></span>



[<span data-ttu-id="56b0a-130">Памятки</span><span class="sxs-lookup"><span data-stu-id="56b0a-130">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="56b0a-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="56b0a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

