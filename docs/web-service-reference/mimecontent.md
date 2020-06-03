---
title: Сохранитьmimecontent
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
description: Элемент Сохранитьmimecontent содержит MIME-поток MIME объекта, представленного в формате base64Binary и поддерживающий [RFC2045].
ms.openlocfilehash: 039ef1245d48e4cf13141970921dd210f4bd7d06
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530438"
---
# <a name="mimecontent"></a><span data-ttu-id="f2efc-103">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="f2efc-103">MimeContent</span></span>

<span data-ttu-id="f2efc-104">Элемент **сохранитьmimecontent** содержит MIME-поток MIME объекта, представленного в формате base64Binary и поддерживающий [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span><span class="sxs-lookup"><span data-stu-id="f2efc-104">The **MimeContent** element contains the ASCII MIME stream of an object that is represented in base64Binary format and supports [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span></span>
  
```xml
<MimeContent CharacterSet="" />
```

 <span data-ttu-id="f2efc-105">**мимеконтенттипе**</span><span class="sxs-lookup"><span data-stu-id="f2efc-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2efc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f2efc-106">Attributes and elements</span></span>

<span data-ttu-id="f2efc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f2efc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2efc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f2efc-108">Attributes</span></span>

|<span data-ttu-id="f2efc-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f2efc-109">**Attribute**</span></span>|<span data-ttu-id="f2efc-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f2efc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f2efc-111">**CharacterSet**</span><span class="sxs-lookup"><span data-stu-id="f2efc-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="f2efc-112">Если этот параметр установлен, то значение этого атрибута игнорируется сервером.</span><span class="sxs-lookup"><span data-stu-id="f2efc-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f2efc-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f2efc-113">Child elements</span></span>

<span data-ttu-id="f2efc-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f2efc-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f2efc-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f2efc-115">Parent elements</span></span>

<span data-ttu-id="f2efc-116">[Календаритем](calendaritem.md)  |  [Contact (контакт](contact.md)  |  ) [Дистрибутионлист](distributionlist.md)  |  [Элемент](item.md)  |  [Митингканцеллатион](meetingcancellation.md)  |  [Митингмессаже](meetingmessage.md)  |  [Свойство meetingrequest](meetingrequest.md)  |  [Митингреспонсе](meetingresponse.md)  |  [Message (сообщение](message-ex15websvcsotherref.md)  |  ) [RemoveItem](removeitem.md)  |  [Task (задача](task.md) )</span><span class="sxs-lookup"><span data-stu-id="f2efc-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f2efc-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f2efc-117">Text value</span></span>

<span data-ttu-id="f2efc-118">Текстовое значение, представляющее поток MIME base64Binary, является обязательным при использовании этого элемента.</span><span class="sxs-lookup"><span data-stu-id="f2efc-118">A text value that represents a base64Binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f2efc-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="f2efc-119">Remarks</span></span>

<span data-ttu-id="f2efc-120">Содержимое сообщения проходит через три указанных ниже уровня кодирования, прежде чем он будет сохранен в значении **сохранитьmimecontent** :</span><span class="sxs-lookup"><span data-stu-id="f2efc-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContent** value:</span></span> 
  
1. <span data-ttu-id="f2efc-121">Текст сообщения — это кодировка текста, например ISO-2022-JP для японских символов.</span><span class="sxs-lookup"><span data-stu-id="f2efc-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="f2efc-122">Поток MIME — это кодировка ASCII текста сообщения для элемента **сохранитьmimecontent** или кодировка UTF8 текста сообщения для элемента [MimeContentUTF8](mimecontentutf8.md) .</span><span class="sxs-lookup"><span data-stu-id="f2efc-122">MIME stream — This is the ASCII encoding of the message text for the **MimeContent** element, or the UTF8 encoding of the message text for the [MimeContentUTF8](mimecontentutf8.md) element.</span></span> 
    
3. <span data-ttu-id="f2efc-123">XML-документ — это всегда зашифрованный поток ASCII потока MIME, в котором символы, такие как ' \< ', которые являются осмысленными для XML, скрыты из синтаксических анализаторов XML.</span><span class="sxs-lookup"><span data-stu-id="f2efc-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="f2efc-124">Каждый уровень не зависит от уровня, который предшествует ему.</span><span class="sxs-lookup"><span data-stu-id="f2efc-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="f2efc-125">Элемент **сохранитьmimecontent** может содержать те же данные, что и другие свойства, возвращаемые с элементом.</span><span class="sxs-lookup"><span data-stu-id="f2efc-125">The **MimeContent** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="f2efc-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2efc-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2efc-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f2efc-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2efc-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f2efc-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2efc-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f2efc-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f2efc-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f2efc-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2efc-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f2efc-131">Validation File</span></span>  <br/> |<span data-ttu-id="f2efc-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f2efc-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2efc-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f2efc-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2efc-134">False</span><span class="sxs-lookup"><span data-stu-id="f2efc-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2efc-135">См. также</span><span class="sxs-lookup"><span data-stu-id="f2efc-135">See also</span></span>



- [<span data-ttu-id="f2efc-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f2efc-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

