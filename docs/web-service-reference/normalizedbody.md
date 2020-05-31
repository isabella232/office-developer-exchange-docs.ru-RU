---
title: нормализедбоди
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: Элемент Нормализедбоди указывает HTML-представление свойства Body элемента в виде фрагмента, который можно вставить в другой HTML-текст.
ms.openlocfilehash: 07c2176d2c8a7473c06b7e42f8bcbbe6670581ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834548"
---
# <a name="normalizedbody"></a><span data-ttu-id="4c6b8-103">нормализедбоди</span><span class="sxs-lookup"><span data-stu-id="4c6b8-103">NormalizedBody</span></span>

<span data-ttu-id="4c6b8-104">Элемент **нормализедбоди** указывает HTML-представление свойства **Body** элемента в виде фрагмента, который можно вставить в другой HTML-текст.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-104">The **NormalizedBody** element specifies an HTML representation of the **Body** property of an item as a fragment that can be inserted into another HTML body.</span></span> 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 <span data-ttu-id="4c6b8-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="4c6b8-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c6b8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4c6b8-106">Attributes and elements</span></span>

<span data-ttu-id="4c6b8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c6b8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4c6b8-108">Attributes</span></span>

|<span data-ttu-id="4c6b8-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4c6b8-109">**Attribute**</span></span>|<span data-ttu-id="4c6b8-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4c6b8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4c6b8-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="4c6b8-111">BodyType</span></span>  <br/> |<span data-ttu-id="4c6b8-112">Указывает тип тела.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-112">Indicates the body type.</span></span> <span data-ttu-id="4c6b8-113">Значение **Text** для атрибута **BodyType** указывает на то, что текст отображается в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-113">The value of **Text** for the **BodyType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="4c6b8-114">Значение **HTML** для атрибута **BodyType** указывает на то, что текст находится в HTML-форме.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-114">The value of **HTML** for the **BodyType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="4c6b8-115">Атрибут **BodyType** является обязательным.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-115">The **BodyType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="4c6b8-116">Усечено</span><span class="sxs-lookup"><span data-stu-id="4c6b8-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="4c6b8-117">Указывает, что содержимое тела было усечено.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="4c6b8-118">Текстовое значение **false** для атрибута **Truncate** указывает на то, что содержимое основного текста не было усечено.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="4c6b8-119">Нормализованное тело будет усечено, если длина нормализованного текста превышает значение, заданное в элементе [максимумбодисизе](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="4c6b8-119">The normalized body will be truncated if the normalized body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4c6b8-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4c6b8-120">Child elements</span></span>

<span data-ttu-id="4c6b8-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4c6b8-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4c6b8-122">Parent elements</span></span>

<span data-ttu-id="4c6b8-123">[Item](item.md) | [Сообщение](message-ex15websvcsotherref.md) | [MeetingResponse](meetingresponse.md) | [Contact](contact.md)[MeetingMessage](meetingmessage.md) | [MeetingCancellation](meetingcancellation.md)[MeetingRequest](meetingrequest.md) | [DistributionList](distributionlist.md) [Task](task.md)[PostItem](postitem.md)[CalendarItem](calendaritem.md)элемента митингмессаже | свойство meetingrequest митингреспонсе митингканцеллатион | Task | Item | календаритем Contact дистрибутионлист | </span><span class="sxs-lookup"><span data-stu-id="4c6b8-123">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4c6b8-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4c6b8-124">Text value</span></span>

<span data-ttu-id="4c6b8-125">Текстовое значение элемента **нормализедбоди** — это нормализованный текст элемента.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-125">The text value of the **NormalizedBody** element is the normalized body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4c6b8-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="4c6b8-126">Remarks</span></span>

<span data-ttu-id="4c6b8-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4c6b8-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c6b8-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c6b8-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4c6b8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c6b8-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4c6b8-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4c6b8-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4c6b8-131">Schema name</span></span>  <br/> |<span data-ttu-id="4c6b8-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4c6b8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="4c6b8-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4c6b8-133">Validation file</span></span>  <br/> |<span data-ttu-id="4c6b8-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4c6b8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c6b8-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4c6b8-135">Can be empty</span></span>  <br/> ||
   

