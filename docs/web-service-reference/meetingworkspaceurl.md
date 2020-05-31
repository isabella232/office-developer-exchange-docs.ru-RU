---
title: митингворкспацеурл
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
description: Элемент Митингворкспацеурл содержит URL-адрес рабочей области для собраний, включенной в элемент календаря. Рабочая область для собраний — это общедоступный веб-сайт для планирования собраний и отслеживания результатов.
ms.openlocfilehash: 7d84547eafe4e77fb23a792fbf15633dbf93d775
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834436"
---
# <a name="meetingworkspaceurl"></a><span data-ttu-id="079a6-104">митингворкспацеурл</span><span class="sxs-lookup"><span data-stu-id="079a6-104">MeetingWorkspaceUrl</span></span>

<span data-ttu-id="079a6-105">Элемент **митингворкспацеурл** содержит URL-адрес рабочей области для собраний, включенной в элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="079a6-105">The **MeetingWorkspaceUrl** element contains the URL for the meeting workspace that is included in the calendar item.</span></span> <span data-ttu-id="079a6-106">Рабочая область для собраний — это общедоступный веб-сайт для планирования собраний и отслеживания результатов.</span><span class="sxs-lookup"><span data-stu-id="079a6-106">A meeting workspace is a shared Web site for planning the meeting and tracking the results.</span></span> 
  
```xml
<MeetingWorkspaceUrl/>
```

 <span data-ttu-id="079a6-107">**строка**</span><span class="sxs-lookup"><span data-stu-id="079a6-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="079a6-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="079a6-108">Attributes and elements</span></span>

<span data-ttu-id="079a6-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="079a6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="079a6-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="079a6-110">Attributes</span></span>

<span data-ttu-id="079a6-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="079a6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="079a6-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="079a6-112">Child elements</span></span>

<span data-ttu-id="079a6-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="079a6-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="079a6-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="079a6-114">Parent elements</span></span>

|<span data-ttu-id="079a6-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="079a6-115">**Element**</span></span>|<span data-ttu-id="079a6-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="079a6-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="079a6-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="079a6-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="079a6-118">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="079a6-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="079a6-119">календаритем</span><span class="sxs-lookup"><span data-stu-id="079a6-119">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="079a6-120">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="079a6-120">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="079a6-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="079a6-121">Text value</span></span>

<span data-ttu-id="079a6-122">При использовании этого элемента необходимо указать текстовое значение, представляющее URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="079a6-122">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="079a6-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="079a6-123">Remarks</span></span>

<span data-ttu-id="079a6-124">Свойство Митингворкспацеурл доступно для записи в элементе календаря организатора.</span><span class="sxs-lookup"><span data-stu-id="079a6-124">The MeetingWorkspaceUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="079a6-125">Он доступен только для чтения для приглашений на собрания и элементов календаря участников.</span><span class="sxs-lookup"><span data-stu-id="079a6-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="079a6-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="079a6-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="079a6-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="079a6-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="079a6-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="079a6-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="079a6-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="079a6-129">Schema name</span></span>  <br/> |<span data-ttu-id="079a6-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="079a6-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="079a6-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="079a6-131">Validation file</span></span>  <br/> |<span data-ttu-id="079a6-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="079a6-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="079a6-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="079a6-133">Can be empty</span></span>  <br/> |<span data-ttu-id="079a6-134">False</span><span class="sxs-lookup"><span data-stu-id="079a6-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="079a6-135">См. также</span><span class="sxs-lookup"><span data-stu-id="079a6-135">See also</span></span>



- [<span data-ttu-id="079a6-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="079a6-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

