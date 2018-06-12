---
title: ConflictingMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: Элемент ConflictingMeetingCount представляет число собраний, конфликтующие с элемента календаря.
ms.openlocfilehash: ace800982c284cf65ff22d92c711197ee5ee1d06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761710"
---
# <a name="conflictingmeetingcount"></a><span data-ttu-id="a7298-103">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="a7298-103">ConflictingMeetingCount</span></span>

<span data-ttu-id="a7298-104">Элемент **ConflictingMeetingCount** представляет число собраний, конфликтующие с элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="a7298-104">The **ConflictingMeetingCount** element represents the number of meetings that conflict with the calendar item.</span></span> 
  
```xml
<ConflictingMeetingCount/>
```

 <span data-ttu-id="a7298-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a7298-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7298-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a7298-106">Attributes and elements</span></span>

<span data-ttu-id="a7298-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a7298-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7298-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a7298-108">Attributes</span></span>

<span data-ttu-id="a7298-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a7298-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7298-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a7298-110">Child elements</span></span>

<span data-ttu-id="a7298-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a7298-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7298-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a7298-112">Parent elements</span></span>

|<span data-ttu-id="a7298-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a7298-113">**Element**</span></span>|<span data-ttu-id="a7298-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7298-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7298-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a7298-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a7298-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7298-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a7298-117">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="a7298-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a7298-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7298-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a7298-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a7298-119">Text value</span></span>

<span data-ttu-id="a7298-120">Текстовое значение представляет собой целое число.</span><span class="sxs-lookup"><span data-stu-id="a7298-120">The text value represents an integer.</span></span> <span data-ttu-id="a7298-121">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7298-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a7298-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="a7298-122">Remarks</span></span>

<span data-ttu-id="a7298-123">Элемент календаря считается конфликтующие, если она происходит, по крайней мере в части, в то же время, что и другой элемент календаря в той же папке календаря.</span><span class="sxs-lookup"><span data-stu-id="a7298-123">A calendar item is considered conflicting if it occurs, at least in part, at the same time as another calendar item in the same calendar folder.</span></span> <span data-ttu-id="a7298-124">Если элемент календаря в папке noncalendar, — это по сравнению с элементами календаря в папке календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a7298-124">If a calendar item is in a noncalendar folder, it is compared with calendar items in the default calendar folder.</span></span> <span data-ttu-id="a7298-125">Приглашения на собрания, сравниваются с элементами календаря в папке календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a7298-125">Meeting requests are compared with calendar items in the default calendar folder.</span></span>
  
<span data-ttu-id="a7298-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a7298-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7298-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a7298-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7298-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a7298-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7298-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a7298-129">Schema name</span></span>  <br/> |<span data-ttu-id="a7298-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a7298-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7298-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a7298-131">Validation file</span></span>  <br/> |<span data-ttu-id="a7298-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7298-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7298-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a7298-133">Can be empty</span></span>  <br/> |<span data-ttu-id="a7298-134">False</span><span class="sxs-lookup"><span data-stu-id="a7298-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7298-135">См. также</span><span class="sxs-lookup"><span data-stu-id="a7298-135">See also</span></span>



- [<span data-ttu-id="a7298-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a7298-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

