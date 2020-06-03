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
ms.openlocfilehash: c0002785fb990a251267218f7a5f232e521db41a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459485"
---
# <a name="textbody"></a><span data-ttu-id="e8b6f-103">текстбоди</span><span class="sxs-lookup"><span data-stu-id="e8b6f-103">TextBody</span></span>

<span data-ttu-id="e8b6f-104">Элемент **текстбоди** указывает текст текста.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-104">The **TextBody** element specifies the text body.</span></span> 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 <span data-ttu-id="e8b6f-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="e8b6f-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8b6f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e8b6f-106">Attributes and elements</span></span>

<span data-ttu-id="e8b6f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8b6f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e8b6f-108">Attributes</span></span>

|<span data-ttu-id="e8b6f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e8b6f-109">**Attribute**</span></span>|<span data-ttu-id="e8b6f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8b6f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e8b6f-111">бодитипетипе</span><span class="sxs-lookup"><span data-stu-id="e8b6f-111">BodyTypeType</span></span>  <br/> |<span data-ttu-id="e8b6f-112">Указывает тип тела.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-112">Indicates the body type.</span></span> <span data-ttu-id="e8b6f-113">Значение **Text** для атрибута **бодитипетипе** указывает на то, что текст отображается в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-113">The value of **Text** for the **BodyTypeType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="e8b6f-114">Значение **HTML** для атрибута **бодитипетипе** указывает на то, что текст находится в HTML-форме.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-114">The value of **HTML** for the **BodyTypeType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="e8b6f-115">Атрибут **бодитипетипе** является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-115">The **BodyTypeType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e8b6f-116">Усечено</span><span class="sxs-lookup"><span data-stu-id="e8b6f-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="e8b6f-117">Указывает, что содержимое тела было усечено.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="e8b6f-118">Текстовое значение **false** для атрибута **Truncate** указывает на то, что содержимое основного текста не было усечено.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="e8b6f-119">Нормализованный текст будет усечен, если длина текста текста превышает значение, заданное в элементе [максимумбодисизе](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="e8b6f-119">The normalized body will be truncated if the text body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e8b6f-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e8b6f-120">Child elements</span></span>

<span data-ttu-id="e8b6f-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8b6f-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e8b6f-122">Parent elements</span></span>

<span data-ttu-id="e8b6f-123">[Элемент](item.md)  |  [Contact (контакт](contact.md)  |  ) [Message (сообщение](message-ex15websvcsotherref.md)  |  ) [Дистрибутионлист](distributionlist.md)  |  [Календаритем](calendaritem.md)  |  [Элемент](postitem.md)  |  i [Task (задача](task.md) )</span><span class="sxs-lookup"><span data-stu-id="e8b6f-123">[Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="e8b6f-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e8b6f-124">Text value</span></span>

<span data-ttu-id="e8b6f-125">Текстовое значение элемента **текстбоди** — основной текст элемента.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-125">The text value of the **TextBody** element is the text body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e8b6f-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="e8b6f-126">Remarks</span></span>

<span data-ttu-id="e8b6f-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e8b6f-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8b6f-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e8b6f-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8b6f-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e8b6f-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8b6f-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e8b6f-131">Schema name</span></span>  <br/> |<span data-ttu-id="e8b6f-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e8b6f-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8b6f-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e8b6f-133">Validation file</span></span>  <br/> |<span data-ttu-id="e8b6f-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e8b6f-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8b6f-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e8b6f-135">Can be empty</span></span>  <br/> ||
   

