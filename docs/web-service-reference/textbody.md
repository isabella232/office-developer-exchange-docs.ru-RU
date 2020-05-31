---
title: текстбоди
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: Элемент Текстбоди указывает текст текста.
ms.openlocfilehash: 78b18b27891d571605d2eeeeffb5c252cc790c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840152"
---
# <a name="textbody"></a><span data-ttu-id="853b1-103">текстбоди</span><span class="sxs-lookup"><span data-stu-id="853b1-103">TextBody</span></span>

<span data-ttu-id="853b1-104">Элемент **текстбоди** указывает текст текста.</span><span class="sxs-lookup"><span data-stu-id="853b1-104">The **TextBody** element specifies the text body.</span></span> 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 <span data-ttu-id="853b1-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="853b1-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="853b1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="853b1-106">Attributes and elements</span></span>

<span data-ttu-id="853b1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="853b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="853b1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="853b1-108">Attributes</span></span>

|<span data-ttu-id="853b1-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="853b1-109">**Attribute**</span></span>|<span data-ttu-id="853b1-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="853b1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="853b1-111">бодитипетипе</span><span class="sxs-lookup"><span data-stu-id="853b1-111">BodyTypeType</span></span>  <br/> |<span data-ttu-id="853b1-112">Указывает тип тела.</span><span class="sxs-lookup"><span data-stu-id="853b1-112">Indicates the body type.</span></span> <span data-ttu-id="853b1-113">Значение **Text** для атрибута **бодитипетипе** указывает на то, что текст отображается в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="853b1-113">The value of **Text** for the **BodyTypeType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="853b1-114">Значение **HTML** для атрибута **бодитипетипе** указывает на то, что текст находится в HTML-форме.</span><span class="sxs-lookup"><span data-stu-id="853b1-114">The value of **HTML** for the **BodyTypeType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="853b1-115">Атрибут **бодитипетипе** является обязательным.</span><span class="sxs-lookup"><span data-stu-id="853b1-115">The **BodyTypeType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="853b1-116">Усечено</span><span class="sxs-lookup"><span data-stu-id="853b1-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="853b1-117">Указывает, что содержимое тела было усечено.</span><span class="sxs-lookup"><span data-stu-id="853b1-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="853b1-118">Текстовое значение **false** для атрибута **Truncate** указывает на то, что содержимое основного текста не было усечено.</span><span class="sxs-lookup"><span data-stu-id="853b1-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="853b1-119">Нормализованный текст будет усечен, если длина текста текста превышает значение, заданное в элементе [максимумбодисизе](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="853b1-119">The normalized body will be truncated if the text body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="853b1-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="853b1-120">Child elements</span></span>

<span data-ttu-id="853b1-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="853b1-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="853b1-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="853b1-122">Parent elements</span></span>

<span data-ttu-id="853b1-123">[Item](item.md) |  | [Сообщение](message-ex15websvcsotherref.md) | [PostItem](postitem.md) | [Task](task.md) [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md)[Contact](contact.md)с контактами для элемента дистрибутионлист календаритем i i Item Task | </span><span class="sxs-lookup"><span data-stu-id="853b1-123">[Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="853b1-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="853b1-124">Text value</span></span>

<span data-ttu-id="853b1-125">Текстовое значение элемента **текстбоди** — основной текст элемента.</span><span class="sxs-lookup"><span data-stu-id="853b1-125">The text value of the **TextBody** element is the text body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="853b1-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="853b1-126">Remarks</span></span>

<span data-ttu-id="853b1-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="853b1-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="853b1-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="853b1-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="853b1-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="853b1-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="853b1-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="853b1-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="853b1-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="853b1-131">Schema name</span></span>  <br/> |<span data-ttu-id="853b1-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="853b1-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="853b1-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="853b1-133">Validation file</span></span>  <br/> |<span data-ttu-id="853b1-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="853b1-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="853b1-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="853b1-135">Can be empty</span></span>  <br/> ||
   

