---
title: Напоминание
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54dd748a-23a5-4ea2-88f2-b74c68a3c48f
description: Элемент напоминания указывает напоминание для задачи или элемента календаря.
ms.openlocfilehash: 71e54d920a169b8060d22bb7d7d294208c344c2e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457489"
---
# <a name="reminder"></a><span data-ttu-id="73b41-103">Напоминание</span><span class="sxs-lookup"><span data-stu-id="73b41-103">Reminder</span></span>

<span data-ttu-id="73b41-104">Элемент **напоминания** указывает напоминание для задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="73b41-104">The **Reminder** element specifies a reminder for a task or a calendar item.</span></span> 
  
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

 <span data-ttu-id="73b41-105">**реминдертипе**</span><span class="sxs-lookup"><span data-stu-id="73b41-105">**ReminderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73b41-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="73b41-106">Attributes and elements</span></span>

<span data-ttu-id="73b41-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="73b41-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73b41-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="73b41-108">Attributes</span></span>

<span data-ttu-id="73b41-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="73b41-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73b41-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="73b41-110">Child elements</span></span>

<span data-ttu-id="73b41-111">[Subject (тема](subject.md)  |  ) [Location (расположение](location.md)  |  ) [ReminderTime](remindertime.md)  |  [StartDate](startdate.md)  |  [EndDate (реминдертипе)](enddate-remindertype.md)  |  [ItemId](itemid.md)  |  [Рекуррингмастеритемид (итемидтипе)](recurringmasteritemid-itemidtype.md)  |  [Реминдерграуп](remindergroup.md)  |  [UID (UID](uid.md) )</span><span class="sxs-lookup"><span data-stu-id="73b41-111">[Subject](subject.md) | [Location](location.md) | [ReminderTime](remindertime.md) | [StartDate](startdate.md) | [EndDate (ReminderType)](enddate-remindertype.md) | [ItemId](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md) | [ReminderGroup](remindergroup.md) | [UID](uid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73b41-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="73b41-112">Parent elements</span></span>

[<span data-ttu-id="73b41-113">Reminders</span><span class="sxs-lookup"><span data-stu-id="73b41-113">Reminders</span></span>](reminders.md)
  
## <a name="remarks"></a><span data-ttu-id="73b41-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="73b41-114">Remarks</span></span>

<span data-ttu-id="73b41-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="73b41-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="73b41-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="73b41-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73b41-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="73b41-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73b41-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="73b41-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="73b41-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="73b41-119">Schema Name</span></span>  <br/> |<span data-ttu-id="73b41-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="73b41-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="73b41-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="73b41-121">Validation File</span></span>  <br/> |<span data-ttu-id="73b41-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="73b41-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="73b41-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="73b41-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="73b41-124">False</span><span class="sxs-lookup"><span data-stu-id="73b41-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73b41-125">См. также</span><span class="sxs-lookup"><span data-stu-id="73b41-125">See also</span></span>



[<span data-ttu-id="73b41-126">Reminders</span><span class="sxs-lookup"><span data-stu-id="73b41-126">Reminders</span></span>](reminders.md)


- [<span data-ttu-id="73b41-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="73b41-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

