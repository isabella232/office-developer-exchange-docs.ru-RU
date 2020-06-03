---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: Элемент InternetMessageHeader представляет заголовок Интернет-сообщения для данного заголовка в коллекции заголовков. Чтобы получить всю коллекцию заголовков сообщений Интернета, используйте свойство PR_TRANSPORT_MESSAGE_HEADERS. Для получения дополнительных сведений о службах EWS и заголовках сообщений Интернета Сижеттинг в службах EWS, MIME и отсутствующих заголовках сообщений через Интернет.
ms.openlocfilehash: 7b662617e0b1a1fcdcce3449b729485ba6e0956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459309"
---
# <a name="internetmessageheader"></a><span data-ttu-id="04981-105">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="04981-105">InternetMessageHeader</span></span>

<span data-ttu-id="04981-106">Элемент **InternetMessageHeader** представляет заголовок Интернет-сообщения для данного заголовка в коллекции заголовков.</span><span class="sxs-lookup"><span data-stu-id="04981-106">The **InternetMessageHeader** element represents the Internet message header for a given header within the headers collection.</span></span> <span data-ttu-id="04981-107">Чтобы получить всю коллекцию заголовков сообщений Интернета, используйте свойство **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="04981-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="04981-108">Дополнительные сведения о службах EWS и заголовках сообщений в Интернете приведены в статье "как заголовки сообщений Интернета в [EWS, MIME и отсутствующие заголовки сообщений в Интернете](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)".</span><span class="sxs-lookup"><span data-stu-id="04981-108">For more information about EWS and Internet message headers, see "Getting Internet message headers in [EWS, MIME, and the missing Internet message headers](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 <span data-ttu-id="04981-109">**интернесеадертипе**</span><span class="sxs-lookup"><span data-stu-id="04981-109">**InternetHeaderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04981-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="04981-110">Attributes and elements</span></span>

<span data-ttu-id="04981-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="04981-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04981-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="04981-112">Attributes</span></span>

|<span data-ttu-id="04981-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="04981-113">**Attribute**</span></span>|<span data-ttu-id="04981-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="04981-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="04981-115">**хеадернаме**</span><span class="sxs-lookup"><span data-stu-id="04981-115">**HeaderName**</span></span> <br/> |<span data-ttu-id="04981-116">Определяет имя заголовка.</span><span class="sxs-lookup"><span data-stu-id="04981-116">Identifies the header name.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="04981-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="04981-117">Child elements</span></span>

<span data-ttu-id="04981-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="04981-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04981-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="04981-119">Parent elements</span></span>

|<span data-ttu-id="04981-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="04981-120">**Element**</span></span>|<span data-ttu-id="04981-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="04981-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04981-122">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="04981-122">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="04981-123">Представляет коллекцию всех заголовков сообщений Интернета, которые находятся в элементе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="04981-123">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04981-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="04981-124">Text value</span></span>

<span data-ttu-id="04981-125">Текстовое значение представляет значение заголовка.</span><span class="sxs-lookup"><span data-stu-id="04981-125">The text value represents the value for the header.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04981-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="04981-126">Remarks</span></span>

<span data-ttu-id="04981-127">Ниже приведено определение расширенного свойства управляемого API EWS для свойства **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="04981-127">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="04981-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="04981-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04981-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="04981-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04981-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="04981-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04981-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="04981-131">Schema Name</span></span>  <br/> |<span data-ttu-id="04981-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="04981-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="04981-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="04981-133">Validation File</span></span>  <br/> |<span data-ttu-id="04981-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="04981-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04981-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="04981-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="04981-136">False</span><span class="sxs-lookup"><span data-stu-id="04981-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04981-137">См. также</span><span class="sxs-lookup"><span data-stu-id="04981-137">See also</span></span>



- [<span data-ttu-id="04981-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="04981-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="04981-139">EWS, MIME и отсутствующие заголовки сообщений Интернета</span><span class="sxs-lookup"><span data-stu-id="04981-139">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

