---
title: Памятки
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54dd748a-23a5-4ea2-88f2-b74c68a3c48f
description: Элемент напоминание указывает напоминания для задачи или элемента календаря.
ms.openlocfilehash: cfa1160bd25f5045a3da5a98f081c9dcb3debe7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835056"
---
# <a name="reminder"></a><span data-ttu-id="fd240-103">Памятки</span><span class="sxs-lookup"><span data-stu-id="fd240-103">Reminder</span></span>

<span data-ttu-id="fd240-104">Элемент **напоминание** указывает напоминания для задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="fd240-104">The **Reminder** element specifies a reminder for a task or a calendar item.</span></span> 
  
```XML
<Reminder>
   <Subject></Subject>
   <Location></Location>
   <ReminderTime></ReminderTime>
   <StartDate></StartDate>
   <EndDate></EndDate>
   <ItemId></ItemId>
   <RecurringMasterItemId></RecurringMasterItemId>
   <ReminderGroup></ReminderGroup>
   <UID></UID>
</Reminder>

```

 <span data-ttu-id="fd240-105">**ReminderType**</span><span class="sxs-lookup"><span data-stu-id="fd240-105">**ReminderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd240-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fd240-106">Attributes and elements</span></span>

<span data-ttu-id="fd240-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fd240-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd240-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fd240-108">Attributes</span></span>

<span data-ttu-id="fd240-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fd240-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd240-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fd240-110">Child elements</span></span>

<span data-ttu-id="fd240-111">[Тема](subject.md) | [расположение](location.md) | [ReminderTime](remindertime.md) | [StartDate](startdate.md) | [EndDate (ReminderType)](enddate-remindertype.md) | [ItemId](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md)  |  [ReminderGroup](remindergroup.md) | [ИД пользователя](uid.md)</span><span class="sxs-lookup"><span data-stu-id="fd240-111">[Subject](subject.md) | [Location](location.md) | [ReminderTime](remindertime.md) | [StartDate](startdate.md) | [EndDate (ReminderType)](enddate-remindertype.md) | [ItemId](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md) | [ReminderGroup](remindergroup.md) | [UID](uid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd240-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fd240-112">Parent elements</span></span>

[<span data-ttu-id="fd240-113">Напоминания</span><span class="sxs-lookup"><span data-stu-id="fd240-113">Reminders</span></span>](reminders.md)
  
## <a name="remarks"></a><span data-ttu-id="fd240-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="fd240-114">Remarks</span></span>

<span data-ttu-id="fd240-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fd240-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fd240-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd240-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd240-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fd240-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd240-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fd240-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd240-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fd240-119">Schema Name</span></span>  <br/> |<span data-ttu-id="fd240-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fd240-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd240-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fd240-121">Validation File</span></span>  <br/> |<span data-ttu-id="fd240-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fd240-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd240-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fd240-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd240-124">False</span><span class="sxs-lookup"><span data-stu-id="fd240-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd240-125">См. также</span><span class="sxs-lookup"><span data-stu-id="fd240-125">See also</span></span>



[<span data-ttu-id="fd240-126">Напоминания</span><span class="sxs-lookup"><span data-stu-id="fd240-126">Reminders</span></span>](reminders.md)


- [<span data-ttu-id="fd240-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fd240-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

