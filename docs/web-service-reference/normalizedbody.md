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
ms.openlocfilehash: fb249794bccfeed198e7a3230ab53c66893dcf96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462670"
---
# <a name="normalizedbody"></a><span data-ttu-id="f35d2-103">нормализедбоди</span><span class="sxs-lookup"><span data-stu-id="f35d2-103">NormalizedBody</span></span>

<span data-ttu-id="f35d2-104">Элемент **нормализедбоди** указывает HTML-представление свойства **Body** элемента в виде фрагмента, который можно вставить в другой HTML-текст.</span><span class="sxs-lookup"><span data-stu-id="f35d2-104">The **NormalizedBody** element specifies an HTML representation of the **Body** property of an item as a fragment that can be inserted into another HTML body.</span></span> 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 <span data-ttu-id="f35d2-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="f35d2-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f35d2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f35d2-106">Attributes and elements</span></span>

<span data-ttu-id="f35d2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f35d2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f35d2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f35d2-108">Attributes</span></span>

|<span data-ttu-id="f35d2-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f35d2-109">**Attribute**</span></span>|<span data-ttu-id="f35d2-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f35d2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f35d2-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="f35d2-111">BodyType</span></span>  <br/> |<span data-ttu-id="f35d2-112">Указывает тип тела.</span><span class="sxs-lookup"><span data-stu-id="f35d2-112">Indicates the body type.</span></span> <span data-ttu-id="f35d2-113">Значение **Text** для атрибута **BodyType** указывает на то, что текст отображается в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="f35d2-113">The value of **Text** for the **BodyType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="f35d2-114">Значение **HTML** для атрибута **BodyType** указывает на то, что текст находится в HTML-форме.</span><span class="sxs-lookup"><span data-stu-id="f35d2-114">The value of **HTML** for the **BodyType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="f35d2-115">Атрибут **BodyType** является обязательным.</span><span class="sxs-lookup"><span data-stu-id="f35d2-115">The **BodyType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="f35d2-116">Усечено</span><span class="sxs-lookup"><span data-stu-id="f35d2-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="f35d2-117">Указывает, что содержимое тела было усечено.</span><span class="sxs-lookup"><span data-stu-id="f35d2-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="f35d2-118">Текстовое значение **false** для атрибута **Truncate** указывает на то, что содержимое основного текста не было усечено.</span><span class="sxs-lookup"><span data-stu-id="f35d2-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="f35d2-119">Нормализованное тело будет усечено, если длина нормализованного текста превышает значение, заданное в элементе [максимумбодисизе](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="f35d2-119">The normalized body will be truncated if the normalized body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f35d2-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f35d2-120">Child elements</span></span>

<span data-ttu-id="f35d2-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f35d2-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f35d2-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f35d2-122">Parent elements</span></span>

<span data-ttu-id="f35d2-123">[Элемент](item.md)  |  [Message (сообщение](message-ex15websvcsotherref.md)  |  ) [Митингмессаже](meetingmessage.md)  |  [Свойство meetingrequest](meetingrequest.md)  |  [Митингреспонсе](meetingresponse.md)  |  [Митингканцеллатион](meetingcancellation.md)  |  [Task (задача](task.md)  |  ) [Элемент](postitem.md)  |  i [Календаритем](calendaritem.md)  |  [Contact (контакт](contact.md)  |  ) [Дистрибутионлист](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="f35d2-123">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f35d2-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f35d2-124">Text value</span></span>

<span data-ttu-id="f35d2-125">Текстовое значение элемента **нормализедбоди** — это нормализованный текст элемента.</span><span class="sxs-lookup"><span data-stu-id="f35d2-125">The text value of the **NormalizedBody** element is the normalized body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f35d2-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="f35d2-126">Remarks</span></span>

<span data-ttu-id="f35d2-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f35d2-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f35d2-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f35d2-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f35d2-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f35d2-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f35d2-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f35d2-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f35d2-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f35d2-131">Schema name</span></span>  <br/> |<span data-ttu-id="f35d2-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f35d2-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="f35d2-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f35d2-133">Validation file</span></span>  <br/> |<span data-ttu-id="f35d2-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f35d2-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f35d2-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f35d2-135">Can be empty</span></span>  <br/> ||
   

