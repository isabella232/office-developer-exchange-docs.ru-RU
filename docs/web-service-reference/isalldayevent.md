---
title: IsAllDayEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAllDayEvent
api_type:
- schema
ms.assetid: 29140a64-9d7a-4a14-a10d-c98197c9831b
description: Элемент IsAllDayEvent указывает, представляет ли запрос на собрание или элемент календаря событием на целый день.
ms.openlocfilehash: 81cf1e7d8338275540f264de7cbf194005e7770c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833983"
---
# <a name="isalldayevent"></a><span data-ttu-id="2b367-103">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="2b367-103">IsAllDayEvent</span></span>

<span data-ttu-id="2b367-104">Элемент **IsAllDayEvent** указывает, представляет ли запрос на собрание или элемент календаря событием на целый день.</span><span class="sxs-lookup"><span data-stu-id="2b367-104">The **IsAllDayEvent** element indicates whether a calendar item or meeting request represents an all-day event.</span></span> 
  
```xml
<IsAllDayEvent/>
```

 <span data-ttu-id="2b367-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2b367-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b367-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2b367-106">Attributes and elements</span></span>

<span data-ttu-id="2b367-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2b367-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b367-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2b367-108">Attributes</span></span>

<span data-ttu-id="2b367-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2b367-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b367-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2b367-110">Child elements</span></span>

<span data-ttu-id="2b367-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2b367-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b367-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2b367-112">Parent elements</span></span>

|<span data-ttu-id="2b367-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2b367-113">**Element**</span></span>|<span data-ttu-id="2b367-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2b367-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b367-115">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="2b367-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2b367-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b367-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2b367-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2b367-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2b367-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b367-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2b367-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2b367-119">Text value</span></span>

<span data-ttu-id="2b367-120">Текстовое значение, представляющее логическое значение является обязательным, если данный элемент включен.</span><span class="sxs-lookup"><span data-stu-id="2b367-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="2b367-121">Значение **true** указывает, что элемент представляет событием на целый день.</span><span class="sxs-lookup"><span data-stu-id="2b367-121">A value of **true** indicates that the item represents an all-day event.</span></span> <span data-ttu-id="2b367-122">Значение **false** указывает, что элемент занимает меньше, чем рабочее время пользователя.</span><span class="sxs-lookup"><span data-stu-id="2b367-122">A value of **false** indicates that the item spans less than a user's working hours.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2b367-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="2b367-123">Remarks</span></span>

<span data-ttu-id="2b367-124">Событием на целый день диапазонов продолжительность рабочее время, определенное для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2b367-124">An all-day event spans the duration of working hours that is defined for a mailbox.</span></span>
  
<span data-ttu-id="2b367-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2b367-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b367-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2b367-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b367-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2b367-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b367-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2b367-128">Schema name</span></span>  <br/> |<span data-ttu-id="2b367-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2b367-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b367-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2b367-130">Validation file</span></span>  <br/> |<span data-ttu-id="2b367-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b367-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b367-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2b367-132">Can be empty</span></span>  <br/> |<span data-ttu-id="2b367-133">False</span><span class="sxs-lookup"><span data-stu-id="2b367-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b367-134">См. также</span><span class="sxs-lookup"><span data-stu-id="2b367-134">See also</span></span>



- [<span data-ttu-id="2b367-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2b367-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

