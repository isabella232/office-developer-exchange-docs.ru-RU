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
ms.openlocfilehash: cfa1160bd25f5045a3da5a98f081c9dcb3debe7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835056"
---
# <a name="reminder"></a><span data-ttu-id="80e9b-103">Напоминание</span><span class="sxs-lookup"><span data-stu-id="80e9b-103">Reminder</span></span>

<span data-ttu-id="80e9b-104">Элемент **напоминания** указывает напоминание для задачи или элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="80e9b-104">The **Reminder** element specifies a reminder for a task or a calendar item.</span></span> 
  
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

 <span data-ttu-id="80e9b-105">**реминдертипе**</span><span class="sxs-lookup"><span data-stu-id="80e9b-105">**ReminderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80e9b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="80e9b-106">Attributes and elements</span></span>

<span data-ttu-id="80e9b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="80e9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80e9b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="80e9b-108">Attributes</span></span>

<span data-ttu-id="80e9b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="80e9b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80e9b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="80e9b-110">Child elements</span></span>

<span data-ttu-id="80e9b-111">[Subject](subject.md) | [Местонахождение](location.md) | [StartDate](startdate.md) | [ReminderGroup](remindergroup.md) | [UID](uid.md) [ReminderTime](remindertime.md) |  | [ItemId](itemid.md)[EndDate (ReminderType)](enddate-remindertype.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md)субъекта ReminderTime StartDate EndDate (реминдертипе) ItemId рекуррингмастеритемид (итемидтипе) реминдерграуп UID | </span><span class="sxs-lookup"><span data-stu-id="80e9b-111">[Subject](subject.md) | [Location](location.md) | [ReminderTime](remindertime.md) | [StartDate](startdate.md) | [EndDate (ReminderType)](enddate-remindertype.md) | [ItemId](itemid.md) | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md) | [ReminderGroup](remindergroup.md) | [UID](uid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80e9b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="80e9b-112">Parent elements</span></span>

[<span data-ttu-id="80e9b-113">Reminders</span><span class="sxs-lookup"><span data-stu-id="80e9b-113">Reminders</span></span>](reminders.md)
  
## <a name="remarks"></a><span data-ttu-id="80e9b-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="80e9b-114">Remarks</span></span>

<span data-ttu-id="80e9b-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="80e9b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="80e9b-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="80e9b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80e9b-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="80e9b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80e9b-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="80e9b-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80e9b-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="80e9b-119">Schema Name</span></span>  <br/> |<span data-ttu-id="80e9b-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="80e9b-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="80e9b-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="80e9b-121">Validation File</span></span>  <br/> |<span data-ttu-id="80e9b-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="80e9b-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80e9b-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="80e9b-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="80e9b-124">False</span><span class="sxs-lookup"><span data-stu-id="80e9b-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80e9b-125">См. также</span><span class="sxs-lookup"><span data-stu-id="80e9b-125">See also</span></span>



[<span data-ttu-id="80e9b-126">Reminders</span><span class="sxs-lookup"><span data-stu-id="80e9b-126">Reminders</span></span>](reminders.md)


- [<span data-ttu-id="80e9b-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="80e9b-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

