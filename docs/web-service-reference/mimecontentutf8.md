---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: Элемент MimeContentUTF8 содержит MIME UTF-8-поток объекта, представленного в формате base64Binary и Интернационализация адрес электронной почты поддерживает и [RFC6530].
ms.openlocfilehash: 47599b6634738fd488e5b020f69e36d5fcf550a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834466"
---
# <a name="mimecontentutf8"></a><span data-ttu-id="58e8e-103">MimeContentUTF8</span><span class="sxs-lookup"><span data-stu-id="58e8e-103">MimeContentUTF8</span></span>

<span data-ttu-id="58e8e-104">Элемент **MimeContentUTF8** содержит MIME UTF-8-поток объекта, который представлен в формате base64Binary и поддерживает Интернационализация адрес электронной почты и [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span><span class="sxs-lookup"><span data-stu-id="58e8e-104">The **MimeContentUTF8** element contains the UTF-8 MIME stream of an object that is represented in base64Binary format and supports email address internationalization and [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span></span>
  
```XML
<MimeContentUTF8 CharacterSet="" />
```

 <span data-ttu-id="58e8e-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="58e8e-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58e8e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="58e8e-106">Attributes and elements</span></span>

<span data-ttu-id="58e8e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="58e8e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58e8e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="58e8e-108">Attributes</span></span>

|<span data-ttu-id="58e8e-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="58e8e-109">**Attribute**</span></span>|<span data-ttu-id="58e8e-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="58e8e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="58e8e-111">**CharacterSet**</span><span class="sxs-lookup"><span data-stu-id="58e8e-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="58e8e-112">Если задано, значение этого атрибута игнорируется сервером.</span><span class="sxs-lookup"><span data-stu-id="58e8e-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="58e8e-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="58e8e-113">Child elements</span></span>

<span data-ttu-id="58e8e-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="58e8e-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="58e8e-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="58e8e-115">Parent elements</span></span>

<span data-ttu-id="58e8e-116">[Элемента календаря, имеющего](calendaritem.md) | [контакт](contact.md) | [DistributionList](distributionlist.md) | [элемента](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [ MeetingResponse](meetingresponse.md) | [сообщение](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [задач](task.md)</span><span class="sxs-lookup"><span data-stu-id="58e8e-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="58e8e-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="58e8e-117">Text value</span></span>

<span data-ttu-id="58e8e-118">Текстовое значение, представляющее потока MIME base64binary является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="58e8e-118">A text value that represents a base64binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="58e8e-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="58e8e-119">Remarks</span></span>

<span data-ttu-id="58e8e-120">Содержимое сообщения проходит через трех уровней кодировки перед сохранением в значении **MimeContentUTF8** :</span><span class="sxs-lookup"><span data-stu-id="58e8e-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContentUTF8** value:</span></span> 
  
1. <span data-ttu-id="58e8e-121">Текст сообщения — это тело кодирования, такие как iso-2022-jp для японского языка символов.</span><span class="sxs-lookup"><span data-stu-id="58e8e-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="58e8e-122">Поток MIME — это кодировки UTF8 текста сообщения для элемента **MimeContentUTF8** или кодировка текста сообщения для элемента [MimeContent](mimecontent.md) ASCII.</span><span class="sxs-lookup"><span data-stu-id="58e8e-122">MIME stream — This is the UTF8 encoding of the message text for the **MimeContentUTF8** element, or the ASCII encoding of the message text for the [MimeContent](mimecontent.md) element.</span></span> 
    
3. <span data-ttu-id="58e8e-123">XML-документ — это всегда в кодировке base64 поток ASCII потока MIME, где символы, такие как "\<", значимых XML, скрыты от анализаторы XML.</span><span class="sxs-lookup"><span data-stu-id="58e8e-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="58e8e-124">Каждый уровень вне зависимости от уровня, предшествующего его.</span><span class="sxs-lookup"><span data-stu-id="58e8e-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="58e8e-125">Элемент **MimeContentUTF8** может содержать те же данные, содержащие другие свойства, возвращаемые с элементом.</span><span class="sxs-lookup"><span data-stu-id="58e8e-125">The **MimeContentUTF8** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="58e8e-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="58e8e-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="58e8e-127">Различия версий</span><span class="sxs-lookup"><span data-stu-id="58e8e-127">Version differences</span></span>

<span data-ttu-id="58e8e-128">Этот элемент доступен в версиях Exchange, начиная с построения 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="58e8e-128">This element is available in versions of Exchange starting with build 15.00.0986.00.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58e8e-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="58e8e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58e8e-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="58e8e-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58e8e-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="58e8e-131">Schema Name</span></span>  <br/> |<span data-ttu-id="58e8e-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="58e8e-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="58e8e-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="58e8e-133">Validation File</span></span>  <br/> |<span data-ttu-id="58e8e-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="58e8e-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58e8e-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="58e8e-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="58e8e-136">False</span><span class="sxs-lookup"><span data-stu-id="58e8e-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58e8e-137">См. также</span><span class="sxs-lookup"><span data-stu-id="58e8e-137">See also</span></span>



- [<span data-ttu-id="58e8e-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="58e8e-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

