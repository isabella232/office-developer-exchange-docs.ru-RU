---
title: OptionalAttendees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OptionalAttendees
api_type:
- schema
ms.assetid: e7c80c4d-3794-45e9-986f-6a8a687df0a4
description: Элемент OptionalAttendees представляет участников, которые не требуется на участие в собрании.
ms.openlocfilehash: d5d994f7e85a47b14ab47f58fb73533cf961f7e6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834658"
---
# <a name="optionalattendees"></a><span data-ttu-id="aab03-103">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="aab03-103">OptionalAttendees</span></span>

<span data-ttu-id="aab03-104">Элемент **OptionalAttendees** представляет участников, которые не требуется на участие в собрании.</span><span class="sxs-lookup"><span data-stu-id="aab03-104">The **OptionalAttendees** element represents attendees who are not required to attend a meeting.</span></span> 
  
```xml
<OptionalAttendees>
   <Attendee/>
</OptionalAttendees>
```

 <span data-ttu-id="aab03-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="aab03-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aab03-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aab03-106">Attributes and elements</span></span>

<span data-ttu-id="aab03-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="aab03-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aab03-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aab03-108">Attributes</span></span>

<span data-ttu-id="aab03-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="aab03-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aab03-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aab03-110">Child elements</span></span>

|<span data-ttu-id="aab03-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aab03-111">**Element**</span></span>|<span data-ttu-id="aab03-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aab03-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aab03-113">Attendee</span><span class="sxs-lookup"><span data-stu-id="aab03-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="aab03-114">Представляет участников и ресурсы, необходимые для собрания.</span><span class="sxs-lookup"><span data-stu-id="aab03-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aab03-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aab03-115">Parent elements</span></span>

|<span data-ttu-id="aab03-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aab03-116">**Element**</span></span>|<span data-ttu-id="aab03-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aab03-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aab03-118">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="aab03-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="aab03-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="aab03-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="aab03-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="aab03-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="aab03-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="aab03-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aab03-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="aab03-122">Remarks</span></span>

<span data-ttu-id="aab03-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="aab03-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aab03-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aab03-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aab03-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aab03-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aab03-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aab03-126">Schema name</span></span>  <br/> |<span data-ttu-id="aab03-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="aab03-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="aab03-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aab03-128">Validation file</span></span>  <br/> |<span data-ttu-id="aab03-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aab03-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aab03-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aab03-130">Can be empty</span></span>  <br/> |<span data-ttu-id="aab03-131">False</span><span class="sxs-lookup"><span data-stu-id="aab03-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aab03-132">См. также</span><span class="sxs-lookup"><span data-stu-id="aab03-132">See also</span></span>



- [<span data-ttu-id="aab03-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aab03-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

