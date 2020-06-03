---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: Элемент MimeContentUTF8 содержит MIME-поток в кодировке UTF-8 объекта, представленный в формате base64Binary и поддерживающий международную связь с адресами электронной почты и [RFC6530].
ms.openlocfilehash: a9214bda876c1aadac5b026b3adf38faea8ef17a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530431"
---
# <a name="mimecontentutf8"></a><span data-ttu-id="591a3-103">MimeContentUTF8</span><span class="sxs-lookup"><span data-stu-id="591a3-103">MimeContentUTF8</span></span>

<span data-ttu-id="591a3-104">Элемент **MimeContentUTF8** содержит MIME-поток в кодировке UTF-8 объекта, представленный в формате base64Binary и поддерживающий международную связь с адресами электронной почты и [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span><span class="sxs-lookup"><span data-stu-id="591a3-104">The **MimeContentUTF8** element contains the UTF-8 MIME stream of an object that is represented in base64Binary format and supports email address internationalization and [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span></span>
  
```XML
<MimeContentUTF8 CharacterSet="" />
```

 <span data-ttu-id="591a3-105">**мимеконтенттипе**</span><span class="sxs-lookup"><span data-stu-id="591a3-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="591a3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="591a3-106">Attributes and elements</span></span>

<span data-ttu-id="591a3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="591a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="591a3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="591a3-108">Attributes</span></span>

|<span data-ttu-id="591a3-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="591a3-109">**Attribute**</span></span>|<span data-ttu-id="591a3-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="591a3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="591a3-111">**CharacterSet**</span><span class="sxs-lookup"><span data-stu-id="591a3-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="591a3-112">Если этот параметр установлен, то значение этого атрибута игнорируется сервером.</span><span class="sxs-lookup"><span data-stu-id="591a3-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="591a3-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="591a3-113">Child elements</span></span>

<span data-ttu-id="591a3-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="591a3-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="591a3-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="591a3-115">Parent elements</span></span>

<span data-ttu-id="591a3-116">[Календаритем](calendaritem.md)  |  [Contact (контакт](contact.md)  |  ) [Дистрибутионлист](distributionlist.md)  |  [Элемент](item.md)  |  [Митингканцеллатион](meetingcancellation.md)  |  [Митингмессаже](meetingmessage.md)  |  [Свойство meetingrequest](meetingrequest.md)  |  [Митингреспонсе](meetingresponse.md)  |  [Message (сообщение](message-ex15websvcsotherref.md)  |  ) [RemoveItem](removeitem.md)  |  [Task (задача](task.md) )</span><span class="sxs-lookup"><span data-stu-id="591a3-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="591a3-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="591a3-117">Text value</span></span>

<span data-ttu-id="591a3-118">Текстовое значение, представляющее поток MIME base64Binary, является обязательным при использовании этого элемента.</span><span class="sxs-lookup"><span data-stu-id="591a3-118">A text value that represents a base64binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="591a3-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="591a3-119">Remarks</span></span>

<span data-ttu-id="591a3-120">Содержимое сообщения проходит через три указанных ниже уровня кодирования, прежде чем он будет сохранен в значении **MimeContentUTF8** :</span><span class="sxs-lookup"><span data-stu-id="591a3-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContentUTF8** value:</span></span> 
  
1. <span data-ttu-id="591a3-121">Текст сообщения — это кодировка текста, например ISO-2022-JP для японских символов.</span><span class="sxs-lookup"><span data-stu-id="591a3-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="591a3-122">Поток MIME — это кодировка UTF8 текста сообщения для элемента **MimeContentUTF8** или кодировка ASCII текста сообщения для элемента [сохранитьmimecontent](mimecontent.md) .</span><span class="sxs-lookup"><span data-stu-id="591a3-122">MIME stream — This is the UTF8 encoding of the message text for the **MimeContentUTF8** element, or the ASCII encoding of the message text for the [MimeContent](mimecontent.md) element.</span></span> 
    
3. <span data-ttu-id="591a3-123">XML-документ — это всегда зашифрованный поток ASCII потока MIME, в котором символы, такие как ' \< ', которые являются осмысленными для XML, скрыты из синтаксических анализаторов XML.</span><span class="sxs-lookup"><span data-stu-id="591a3-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="591a3-124">Каждый уровень не зависит от уровня, который предшествует ему.</span><span class="sxs-lookup"><span data-stu-id="591a3-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="591a3-125">Элемент **MimeContentUTF8** может содержать те же данные, что и другие свойства, возвращаемые с элементом.</span><span class="sxs-lookup"><span data-stu-id="591a3-125">The **MimeContentUTF8** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="591a3-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="591a3-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="591a3-127">Различия версий</span><span class="sxs-lookup"><span data-stu-id="591a3-127">Version differences</span></span>

<span data-ttu-id="591a3-128">Этот элемент доступен в версиях Exchange, начинающихся с сборки 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="591a3-128">This element is available in versions of Exchange starting with build 15.00.0986.00.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="591a3-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="591a3-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="591a3-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="591a3-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="591a3-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="591a3-131">Schema Name</span></span>  <br/> |<span data-ttu-id="591a3-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="591a3-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="591a3-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="591a3-133">Validation File</span></span>  <br/> |<span data-ttu-id="591a3-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="591a3-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="591a3-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="591a3-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="591a3-136">False</span><span class="sxs-lookup"><span data-stu-id="591a3-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="591a3-137">См. также</span><span class="sxs-lookup"><span data-stu-id="591a3-137">See also</span></span>



- [<span data-ttu-id="591a3-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="591a3-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

