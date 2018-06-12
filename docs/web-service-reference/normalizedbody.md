---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: Элемент NormalizedBody указывает представлением HTML свойства тела элемента как фрагмент, который можно вставить в другой HTML-текста.
ms.openlocfilehash: 07c2176d2c8a7473c06b7e42f8bcbbe6670581ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834548"
---
# <a name="normalizedbody"></a><span data-ttu-id="97b72-103">NormalizedBody</span><span class="sxs-lookup"><span data-stu-id="97b72-103">NormalizedBody</span></span>

<span data-ttu-id="97b72-104">Элемент **NormalizedBody** указывает представлением HTML свойства **тела** элемента как фрагмент, который можно вставить в другой HTML-текста.</span><span class="sxs-lookup"><span data-stu-id="97b72-104">The **NormalizedBody** element specifies an HTML representation of the **Body** property of an item as a fragment that can be inserted into another HTML body.</span></span> 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 <span data-ttu-id="97b72-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="97b72-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97b72-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="97b72-106">Attributes and elements</span></span>

<span data-ttu-id="97b72-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="97b72-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97b72-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="97b72-108">Attributes</span></span>

|<span data-ttu-id="97b72-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="97b72-109">**Attribute**</span></span>|<span data-ttu-id="97b72-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97b72-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97b72-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="97b72-111">BodyType</span></span>  <br/> |<span data-ttu-id="97b72-112">Указывает тип основного текста.</span><span class="sxs-lookup"><span data-stu-id="97b72-112">Indicates the body type.</span></span> <span data-ttu-id="97b72-113">Значение **текста** в атрибуте **BodyType** указывает текст в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="97b72-113">The value of **Text** for the **BodyType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="97b72-114">Значение **HTML-код** для атрибута **типа текста сообщения** указывает текст в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="97b72-114">The value of **HTML** for the **BodyType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="97b72-115">Атрибут **типа текста сообщения** является обязательным.</span><span class="sxs-lookup"><span data-stu-id="97b72-115">The **BodyType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="97b72-116">IsTruncated</span><span class="sxs-lookup"><span data-stu-id="97b72-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="97b72-117">Указывает, что содержимое текста быть усечен.</span><span class="sxs-lookup"><span data-stu-id="97b72-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="97b72-118">Текстовое значение **false** для атрибута **IsTruncated** указывает, что содержимое текста не были сокращены.</span><span class="sxs-lookup"><span data-stu-id="97b72-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="97b72-119">Нормализованный body усекаются, если длина нормализованный body больше, чем значение, установленное в элементе [MaximumBodySize](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="97b72-119">The normalized body will be truncated if the normalized body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="97b72-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="97b72-120">Child elements</span></span>

<span data-ttu-id="97b72-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="97b72-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="97b72-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="97b72-122">Parent elements</span></span>

<span data-ttu-id="97b72-123">[Элемент](item.md) | [сообщение](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [задачи](task.md) | [PostItem ](postitem.md)  |  [Элемента календаря, имеющего](calendaritem.md) | [контакт](contact.md) | [DistributionList](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="97b72-123">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="97b72-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="97b72-124">Text value</span></span>

<span data-ttu-id="97b72-125">Текстовое значение элемента **NormalizedBody** является нормализованный тело элемента.</span><span class="sxs-lookup"><span data-stu-id="97b72-125">The text value of the **NormalizedBody** element is the normalized body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="97b72-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="97b72-126">Remarks</span></span>

<span data-ttu-id="97b72-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="97b72-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="97b72-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="97b72-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97b72-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="97b72-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97b72-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="97b72-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97b72-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="97b72-131">Schema name</span></span>  <br/> |<span data-ttu-id="97b72-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="97b72-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="97b72-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="97b72-133">Validation file</span></span>  <br/> |<span data-ttu-id="97b72-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="97b72-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97b72-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="97b72-135">Can be empty</span></span>  <br/> ||
   

