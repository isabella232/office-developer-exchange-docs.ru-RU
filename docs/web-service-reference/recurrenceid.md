---
title: RecurrenceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: Элемент RecurrenceId используется для идентификации определенный экземпляр повторяющегося элемента календаря.
ms.openlocfilehash: 078bec85e1ca1530137f9935365d7dd3e530ea34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835005"
---
# <a name="recurrenceid"></a><span data-ttu-id="250a3-103">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="250a3-103">RecurrenceId</span></span>

<span data-ttu-id="250a3-104">Элемент **RecurrenceId** используется для идентификации определенный экземпляр повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="250a3-104">The **RecurrenceId** element is used to identify a specific instance of a recurring calendar item.</span></span> 
  
```xml
<RecurrenceId/>
```

 <span data-ttu-id="250a3-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="250a3-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="250a3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="250a3-106">Attributes and elements</span></span>

<span data-ttu-id="250a3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="250a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="250a3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="250a3-108">Attributes</span></span>

<span data-ttu-id="250a3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="250a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="250a3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="250a3-110">Child elements</span></span>

<span data-ttu-id="250a3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="250a3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="250a3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="250a3-112">Parent elements</span></span>

|<span data-ttu-id="250a3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="250a3-113">**Element**</span></span>|<span data-ttu-id="250a3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="250a3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="250a3-115">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="250a3-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="250a3-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="250a3-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="250a3-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="250a3-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="250a3-118">Представляет сообщение собрания.</span><span class="sxs-lookup"><span data-stu-id="250a3-118">Represents a meeting message.</span></span>  <br/> |
|[<span data-ttu-id="250a3-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="250a3-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="250a3-120">Представляет приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="250a3-120">Represents a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="250a3-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="250a3-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="250a3-122">Представляет ответ на приглашение.</span><span class="sxs-lookup"><span data-stu-id="250a3-122">Represents a meeting response.</span></span>  <br/> |
|[<span data-ttu-id="250a3-123">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="250a3-123">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="250a3-124">Представляет отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="250a3-124">Represents a meeting cancellation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="250a3-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="250a3-125">Text value</span></span>

<span data-ttu-id="250a3-126">Текстовое значение представляет значение даты и времени, которое идентифицирует вхождение календаря.</span><span class="sxs-lookup"><span data-stu-id="250a3-126">The text value represents a date/time value that identifies a calendar occurrence.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="250a3-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="250a3-127">Remarks</span></span>

<span data-ttu-id="250a3-128">Это свойство используется со свойством [Уникальный идентификатор](uid.md) для идентификации определенный экземпляр повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="250a3-128">This property is used with the [UID](uid.md) property to identify a specific instance of a recurring calendar item.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="250a3-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="250a3-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="250a3-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="250a3-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="250a3-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="250a3-131">Schema Name</span></span>  <br/> |<span data-ttu-id="250a3-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="250a3-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="250a3-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="250a3-133">Validation File</span></span>  <br/> |<span data-ttu-id="250a3-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="250a3-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="250a3-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="250a3-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="250a3-136">False</span><span class="sxs-lookup"><span data-stu-id="250a3-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="250a3-137">См. также</span><span class="sxs-lookup"><span data-stu-id="250a3-137">See also</span></span>



- [<span data-ttu-id="250a3-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="250a3-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

