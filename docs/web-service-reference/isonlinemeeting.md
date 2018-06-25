---
title: IsOnlineMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOnlineMeeting
api_type:
- schema
ms.assetid: c29df676-0f3a-4694-a42f-522c6d16872f
description: Элемент IsOnlineMeeting указывает, является ли online собрания.
ms.openlocfilehash: 5a56b0b9828d6f6bec83fc0ad0f8f9579b471a72
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834061"
---
# <a name="isonlinemeeting"></a><span data-ttu-id="6ce51-103">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6ce51-103">IsOnlineMeeting</span></span>

<span data-ttu-id="6ce51-104">Элемент **IsOnlineMeeting** указывает, является ли online собрания.</span><span class="sxs-lookup"><span data-stu-id="6ce51-104">The **IsOnlineMeeting** element indicates whether the meeting is online.</span></span> 
  
```xml
<IsOnlineMeeting/>
```

 <span data-ttu-id="6ce51-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6ce51-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ce51-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6ce51-106">Attributes and elements</span></span>

<span data-ttu-id="6ce51-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6ce51-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ce51-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6ce51-108">Attributes</span></span>

<span data-ttu-id="6ce51-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6ce51-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ce51-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6ce51-110">Child elements</span></span>

<span data-ttu-id="6ce51-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6ce51-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6ce51-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6ce51-112">Parent elements</span></span>

|<span data-ttu-id="6ce51-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6ce51-113">**Element**</span></span>|<span data-ttu-id="6ce51-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6ce51-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ce51-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="6ce51-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="6ce51-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ce51-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6ce51-117">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="6ce51-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="6ce51-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ce51-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6ce51-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6ce51-119">Text value</span></span>

<span data-ttu-id="6ce51-120">Текстовое значение, представляющее логическое значение является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="6ce51-120">A text value that represents a Boolean value is required if this element is used.</span></span> <span data-ttu-id="6ce51-121">Значение **true** указывает, что собрания находится в сети.</span><span class="sxs-lookup"><span data-stu-id="6ce51-121">A value of **true** indicates that the meeting is online.</span></span> <span data-ttu-id="6ce51-122">Значение **false** указывает, что приглашение на собрание не является online.</span><span class="sxs-lookup"><span data-stu-id="6ce51-122">A value of **false** indicates that the meeting is not online.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6ce51-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="6ce51-123">Remarks</span></span>

<span data-ttu-id="6ce51-124">Свойство IsOnlineMeeting чтения записи для организатора элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="6ce51-124">The IsOnlineMeeting property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="6ce51-125">Оно доступно только для чтения, для приглашений на собрания и элементы календаря участников.</span><span class="sxs-lookup"><span data-stu-id="6ce51-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="6ce51-126">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает MicrosoftExchange 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6ce51-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ce51-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6ce51-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ce51-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6ce51-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6ce51-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6ce51-129">Schema name</span></span>  <br/> |<span data-ttu-id="6ce51-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6ce51-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="6ce51-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6ce51-131">Validation file</span></span>  <br/> |<span data-ttu-id="6ce51-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6ce51-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6ce51-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6ce51-133">Can be empty</span></span>  <br/> |<span data-ttu-id="6ce51-134">False</span><span class="sxs-lookup"><span data-stu-id="6ce51-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ce51-135">См. также</span><span class="sxs-lookup"><span data-stu-id="6ce51-135">See also</span></span>



- [<span data-ttu-id="6ce51-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6ce51-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

