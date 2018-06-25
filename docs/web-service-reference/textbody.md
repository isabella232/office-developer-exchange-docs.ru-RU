---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: Элемент TextBody указывает body текст.
ms.openlocfilehash: 78b18b27891d571605d2eeeeffb5c252cc790c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840152"
---
# <a name="textbody"></a><span data-ttu-id="c3966-103">TextBody</span><span class="sxs-lookup"><span data-stu-id="c3966-103">TextBody</span></span>

<span data-ttu-id="c3966-104">Элемент **TextBody** указывает body текст.</span><span class="sxs-lookup"><span data-stu-id="c3966-104">The **TextBody** element specifies the text body.</span></span> 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 <span data-ttu-id="c3966-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="c3966-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c3966-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c3966-106">Attributes and elements</span></span>

<span data-ttu-id="c3966-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c3966-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c3966-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c3966-108">Attributes</span></span>

|<span data-ttu-id="c3966-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="c3966-109">**Attribute**</span></span>|<span data-ttu-id="c3966-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c3966-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c3966-111">BodyTypeType</span><span class="sxs-lookup"><span data-stu-id="c3966-111">BodyTypeType</span></span>  <br/> |<span data-ttu-id="c3966-112">Указывает тип основного текста.</span><span class="sxs-lookup"><span data-stu-id="c3966-112">Indicates the body type.</span></span> <span data-ttu-id="c3966-113">Значение **текста** в атрибуте **BodyTypeType** указывает текст в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="c3966-113">The value of **Text** for the **BodyTypeType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="c3966-114">Значение **HTML-код** для атрибута **BodyTypeType** указывает текст в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="c3966-114">The value of **HTML** for the **BodyTypeType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="c3966-115">Атрибут **BodyTypeType** является обязательным.</span><span class="sxs-lookup"><span data-stu-id="c3966-115">The **BodyTypeType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="c3966-116">IsTruncated</span><span class="sxs-lookup"><span data-stu-id="c3966-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="c3966-117">Указывает, что содержимое текста быть усечен.</span><span class="sxs-lookup"><span data-stu-id="c3966-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="c3966-118">Текстовое значение **false** для атрибута **IsTruncated** указывает, что содержимое текста не были сокращены.</span><span class="sxs-lookup"><span data-stu-id="c3966-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="c3966-119">Нормализованный body усекаются, если длина body текст больше, чем значение, установленное в элементе [MaximumBodySize](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="c3966-119">The normalized body will be truncated if the text body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c3966-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c3966-120">Child elements</span></span>

<span data-ttu-id="c3966-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="c3966-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c3966-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c3966-122">Parent elements</span></span>

<span data-ttu-id="c3966-123">[Элемент](item.md) | [контакт](contact.md) | [сообщение](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [элемента календаря, имеющего](calendaritem.md) | [PostItem](postitem.md) | [задач](task.md)</span><span class="sxs-lookup"><span data-stu-id="c3966-123">[Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c3966-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c3966-124">Text value</span></span>

<span data-ttu-id="c3966-125">Текстовое значение элемента **TextBody** является текста элемента.</span><span class="sxs-lookup"><span data-stu-id="c3966-125">The text value of the **TextBody** element is the text body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c3966-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="c3966-126">Remarks</span></span>

<span data-ttu-id="c3966-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c3966-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c3966-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3966-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c3966-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c3966-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c3966-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c3966-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c3966-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c3966-131">Schema name</span></span>  <br/> |<span data-ttu-id="c3966-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c3966-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="c3966-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c3966-133">Validation file</span></span>  <br/> |<span data-ttu-id="c3966-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c3966-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c3966-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c3966-135">Can be empty</span></span>  <br/> ||
   

