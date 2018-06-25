---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: Элемент MimeContent содержит ASCII MIME-поток объекта, который представлен в формате base64Binary и поддерживает [RFC2045].
ms.openlocfilehash: 60f2d42f09347611559137c494d93036f1192829
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834465"
---
# <a name="mimecontent"></a><span data-ttu-id="013b9-103">MimeContent</span><span class="sxs-lookup"><span data-stu-id="013b9-103">MimeContent</span></span>

<span data-ttu-id="013b9-104">Элемент **MimeContent** содержит ASCII MIME-поток объекта, который представлен в формате base64Binary и поддерживает [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span><span class="sxs-lookup"><span data-stu-id="013b9-104">The **MimeContent** element contains the ASCII MIME stream of an object that is represented in base64Binary format and supports [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span></span>
  
```xml
<MimeContent CharacterSet="" />
```

 <span data-ttu-id="013b9-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="013b9-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="013b9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="013b9-106">Attributes and elements</span></span>

<span data-ttu-id="013b9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="013b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="013b9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="013b9-108">Attributes</span></span>

|<span data-ttu-id="013b9-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="013b9-109">**Attribute**</span></span>|<span data-ttu-id="013b9-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="013b9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="013b9-111">**CharacterSet**</span><span class="sxs-lookup"><span data-stu-id="013b9-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="013b9-112">Если задано, значение этого атрибута игнорируется сервером.</span><span class="sxs-lookup"><span data-stu-id="013b9-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="013b9-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="013b9-113">Child elements</span></span>

<span data-ttu-id="013b9-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="013b9-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="013b9-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="013b9-115">Parent elements</span></span>

<span data-ttu-id="013b9-116">[Элемента календаря, имеющего](calendaritem.md) | [контакт](contact.md) | [DistributionList](distributionlist.md) | [элемента](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [ MeetingResponse](meetingresponse.md) | [сообщение](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [задач](task.md)</span><span class="sxs-lookup"><span data-stu-id="013b9-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="013b9-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="013b9-117">Text value</span></span>

<span data-ttu-id="013b9-118">Текстовое значение, представляющее потока MIME base64Binary является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="013b9-118">A text value that represents a base64Binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="013b9-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="013b9-119">Remarks</span></span>

<span data-ttu-id="013b9-120">Содержимое сообщения проходит через кодировки перед сохранением в значении **MimeContent** трех уровней:</span><span class="sxs-lookup"><span data-stu-id="013b9-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContent** value:</span></span> 
  
1. <span data-ttu-id="013b9-121">Текст сообщения — это тело кодирования, такие как iso-2022-jp для японского языка символов.</span><span class="sxs-lookup"><span data-stu-id="013b9-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="013b9-122">Поток MIME — это ASCII кодирования текста сообщения для элемента **MimeContent** или кодировки UTF8 текста сообщения для элемента [MimeContentUTF8](mimecontentutf8.md) .</span><span class="sxs-lookup"><span data-stu-id="013b9-122">MIME stream — This is the ASCII encoding of the message text for the **MimeContent** element, or the UTF8 encoding of the message text for the [MimeContentUTF8](mimecontentutf8.md) element.</span></span> 
    
3. <span data-ttu-id="013b9-123">XML-документ — это всегда в кодировке base64 поток ASCII потока MIME, где символы, такие как "\<", значимых XML, скрыты от анализаторы XML.</span><span class="sxs-lookup"><span data-stu-id="013b9-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="013b9-124">Каждый уровень вне зависимости от уровня, предшествующего его.</span><span class="sxs-lookup"><span data-stu-id="013b9-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="013b9-125">Элемент **MimeContent** может содержать те же данные, содержащие другие свойства, возвращаемые с элементом.</span><span class="sxs-lookup"><span data-stu-id="013b9-125">The **MimeContent** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="013b9-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="013b9-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="013b9-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="013b9-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="013b9-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="013b9-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="013b9-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="013b9-129">Schema Name</span></span>  <br/> |<span data-ttu-id="013b9-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="013b9-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="013b9-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="013b9-131">Validation File</span></span>  <br/> |<span data-ttu-id="013b9-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="013b9-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="013b9-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="013b9-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="013b9-134">False</span><span class="sxs-lookup"><span data-stu-id="013b9-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="013b9-135">См. также</span><span class="sxs-lookup"><span data-stu-id="013b9-135">See also</span></span>



- [<span data-ttu-id="013b9-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="013b9-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

