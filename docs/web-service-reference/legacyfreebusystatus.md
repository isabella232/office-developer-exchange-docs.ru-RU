---
title: LegacyFreeBusyStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LegacyFreeBusyStatus
api_type:
- schema
ms.assetid: ee5f3046-b79f-4f68-9455-1a688cee2745
description: Элемент LegacyFreeBusyStatus представляет состояния занятости элемента календаря.
ms.openlocfilehash: 681d7256dbef09c6c43d33ea1fc92b5d05e73a41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834247"
---
# <a name="legacyfreebusystatus"></a><span data-ttu-id="8e7a0-103">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="8e7a0-103">LegacyFreeBusyStatus</span></span>

<span data-ttu-id="8e7a0-104">Элемент **LegacyFreeBusyStatus** представляет состояния занятости элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-104">The **LegacyFreeBusyStatus** element represents the free/busy status of the calendar item.</span></span> 
  
```xml
<LegacyFreeBusyStatus/>
```

<span data-ttu-id="8e7a0-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="8e7a0-105">**LegacyFreeBusyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8e7a0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8e7a0-106">Attributes and elements</span></span>

<span data-ttu-id="8e7a0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e7a0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8e7a0-108">Attributes</span></span>

<span data-ttu-id="8e7a0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e7a0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8e7a0-110">Child elements</span></span>

<span data-ttu-id="8e7a0-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e7a0-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8e7a0-112">Parent elements</span></span>

|<span data-ttu-id="8e7a0-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8e7a0-113">**Element**</span></span>|<span data-ttu-id="8e7a0-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8e7a0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e7a0-115">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="8e7a0-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8e7a0-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8e7a0-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8e7a0-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8e7a0-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8e7a0-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8e7a0-119">Text value</span></span>

<span data-ttu-id="8e7a0-120">Для этого элемента требуется указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-120">A text value is required for this element.</span></span> <span data-ttu-id="8e7a0-121">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="8e7a0-122">Свободна</span><span class="sxs-lookup"><span data-stu-id="8e7a0-122">Free</span></span> 
- <span data-ttu-id="8e7a0-123">Под вопросом</span><span class="sxs-lookup"><span data-stu-id="8e7a0-123">Tentative</span></span>
- <span data-ttu-id="8e7a0-124">Занята</span><span class="sxs-lookup"><span data-stu-id="8e7a0-124">Busy</span></span>
- <span data-ttu-id="8e7a0-125">ОБ ОТСУТСТВИИ НА РАБОТЕ</span><span class="sxs-lookup"><span data-stu-id="8e7a0-125">OOF</span></span>
- <span data-ttu-id="8e7a0-126">WorkingElsewhere</span><span class="sxs-lookup"><span data-stu-id="8e7a0-126">WorkingElsewhere</span></span>
- <span data-ttu-id="8e7a0-127">NoData</span><span class="sxs-lookup"><span data-stu-id="8e7a0-127">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="8e7a0-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="8e7a0-128">Remarks</span></span>

<span data-ttu-id="8e7a0-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e7a0-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8e7a0-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e7a0-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8e7a0-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e7a0-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8e7a0-132">Schema name</span></span>  <br/> |<span data-ttu-id="8e7a0-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8e7a0-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e7a0-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8e7a0-134">Validation file</span></span>  <br/> |<span data-ttu-id="8e7a0-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8e7a0-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e7a0-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8e7a0-136">Can be empty</span></span>  <br/> |<span data-ttu-id="8e7a0-137">False</span><span class="sxs-lookup"><span data-stu-id="8e7a0-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e7a0-138">См. также</span><span class="sxs-lookup"><span data-stu-id="8e7a0-138">See also</span></span>

- [<span data-ttu-id="8e7a0-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8e7a0-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

