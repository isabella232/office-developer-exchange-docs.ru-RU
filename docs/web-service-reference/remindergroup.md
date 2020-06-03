---
title: реминдерграуп
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: Элемент Реминдерграуп указывает, относится ли напоминание к элементу календаря или к задаче.
ms.openlocfilehash: be6f4a7d7e9d495ed7b42ed40c60f016468e8c2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529870"
---
# <a name="remindergroup"></a><span data-ttu-id="aee3f-103">реминдерграуп</span><span class="sxs-lookup"><span data-stu-id="aee3f-103">ReminderGroup</span></span>

<span data-ttu-id="aee3f-104">Элемент **реминдерграуп** указывает, относится ли напоминание к элементу календаря или к задаче.</span><span class="sxs-lookup"><span data-stu-id="aee3f-104">The **ReminderGroup** element specifies whether the reminder is for a calendar item or a task.</span></span> 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 <span data-ttu-id="aee3f-105">**реминдерграуптипе**</span><span class="sxs-lookup"><span data-stu-id="aee3f-105">**ReminderGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aee3f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aee3f-106">Attributes and elements</span></span>

<span data-ttu-id="aee3f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="aee3f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aee3f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aee3f-108">Attributes</span></span>

<span data-ttu-id="aee3f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aee3f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aee3f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aee3f-110">Child elements</span></span>

<span data-ttu-id="aee3f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aee3f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aee3f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aee3f-112">Parent elements</span></span>

[<span data-ttu-id="aee3f-113">Reminder</span><span class="sxs-lookup"><span data-stu-id="aee3f-113">Reminder</span></span>](reminder.md)
  
## <a name="text-value"></a><span data-ttu-id="aee3f-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="aee3f-114">Text value</span></span>

<span data-ttu-id="aee3f-115">Текстовое значение элемента **реминдерграуп** — тип группы напоминания.</span><span class="sxs-lookup"><span data-stu-id="aee3f-115">The text value of the **ReminderGroup** element is the group type of the reminder.</span></span> <span data-ttu-id="aee3f-116">Текстовое значение **Calendar** указывает, что напоминание предназначено для элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="aee3f-116">The text value of **Calendar** specifies that the reminder is for a calendar item.</span></span> <span data-ttu-id="aee3f-117">Текстовое значение **Task** указывает, что напоминание относится к элементу задачи.</span><span class="sxs-lookup"><span data-stu-id="aee3f-117">The text value of **Task** specifies that the reminder is for a task item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="aee3f-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="aee3f-118">Remarks</span></span>

<span data-ttu-id="aee3f-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="aee3f-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aee3f-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="aee3f-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aee3f-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aee3f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aee3f-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aee3f-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aee3f-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aee3f-123">Schema Name</span></span>  <br/> |<span data-ttu-id="aee3f-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="aee3f-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="aee3f-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aee3f-125">Validation File</span></span>  <br/> |<span data-ttu-id="aee3f-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="aee3f-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aee3f-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aee3f-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="aee3f-128">False</span><span class="sxs-lookup"><span data-stu-id="aee3f-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aee3f-129">См. также</span><span class="sxs-lookup"><span data-stu-id="aee3f-129">See also</span></span>



[<span data-ttu-id="aee3f-130">Reminder</span><span class="sxs-lookup"><span data-stu-id="aee3f-130">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="aee3f-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aee3f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

