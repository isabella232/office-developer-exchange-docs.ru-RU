---
title: MeetingWorkspaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingWorkspaceUrl
api_type:
- schema
ms.assetid: 0ca942fe-8f57-4065-93ad-65790f9a04c3
description: Элемент MeetingWorkspaceUrl содержит URL-адрес, который включен в календаре рабочей области для собраний. Рабочая область для собраний — это общий веб-узел для планирования собраний и отслеживания результатов.
ms.openlocfilehash: 7d84547eafe4e77fb23a792fbf15633dbf93d775
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834436"
---
# <a name="meetingworkspaceurl"></a><span data-ttu-id="64d6c-104">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="64d6c-104">MeetingWorkspaceUrl</span></span>

<span data-ttu-id="64d6c-105">Элемент **MeetingWorkspaceUrl** содержит URL-адрес, который включен в календаре рабочей области для собраний.</span><span class="sxs-lookup"><span data-stu-id="64d6c-105">The **MeetingWorkspaceUrl** element contains the URL for the meeting workspace that is included in the calendar item.</span></span> <span data-ttu-id="64d6c-106">Рабочая область для собраний — это общий веб-узел для планирования собраний и отслеживания результатов.</span><span class="sxs-lookup"><span data-stu-id="64d6c-106">A meeting workspace is a shared Web site for planning the meeting and tracking the results.</span></span> 
  
```xml
<MeetingWorkspaceUrl/>
```

 <span data-ttu-id="64d6c-107">**string**</span><span class="sxs-lookup"><span data-stu-id="64d6c-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64d6c-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="64d6c-108">Attributes and elements</span></span>

<span data-ttu-id="64d6c-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="64d6c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64d6c-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="64d6c-110">Attributes</span></span>

<span data-ttu-id="64d6c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="64d6c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64d6c-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64d6c-112">Child elements</span></span>

<span data-ttu-id="64d6c-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="64d6c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="64d6c-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="64d6c-114">Parent elements</span></span>

|<span data-ttu-id="64d6c-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64d6c-115">**Element**</span></span>|<span data-ttu-id="64d6c-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64d6c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64d6c-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="64d6c-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="64d6c-118">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="64d6c-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64d6c-119">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="64d6c-119">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="64d6c-120">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="64d6c-120">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="64d6c-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="64d6c-121">Text value</span></span>

<span data-ttu-id="64d6c-122">Текстовое значение, представляющее URL-адрес является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="64d6c-122">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="64d6c-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="64d6c-123">Remarks</span></span>

<span data-ttu-id="64d6c-124">Свойство MeetingWorkspaceUrl чтения записи для организатора элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="64d6c-124">The MeetingWorkspaceUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="64d6c-125">Оно доступно только для чтения, для приглашений на собрания и элементы календаря участников.</span><span class="sxs-lookup"><span data-stu-id="64d6c-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="64d6c-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="64d6c-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64d6c-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="64d6c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64d6c-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="64d6c-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64d6c-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="64d6c-129">Schema name</span></span>  <br/> |<span data-ttu-id="64d6c-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="64d6c-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="64d6c-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="64d6c-131">Validation file</span></span>  <br/> |<span data-ttu-id="64d6c-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="64d6c-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64d6c-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="64d6c-133">Can be empty</span></span>  <br/> |<span data-ttu-id="64d6c-134">False</span><span class="sxs-lookup"><span data-stu-id="64d6c-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64d6c-135">См. также</span><span class="sxs-lookup"><span data-stu-id="64d6c-135">See also</span></span>



- [<span data-ttu-id="64d6c-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="64d6c-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

