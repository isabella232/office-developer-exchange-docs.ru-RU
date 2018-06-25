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
description: Элемент InternetMessageHeader представляет заголовок сообщения Интернета для заданного заголовка в коллекции заголовков. Чтобы получить вся коллекция заголовков сообщений Интернета, используйте свойство PR_TRANSPORT_MESSAGE_HEADERS. Дополнительные сведения о веб-служб Exchange и Интернет заголовки сообщений, seeGetting заголовков сообщений Интернета в веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета.
ms.openlocfilehash: 9457cdabe99c0adcb8183cbc039cc86db881fec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833952"
---
# <a name="internetmessageheader"></a><span data-ttu-id="46798-105">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="46798-105">InternetMessageHeader</span></span>

<span data-ttu-id="46798-106">Элемент **InternetMessageHeader** представляет заголовок сообщения Интернета для заданного заголовка в коллекции заголовков.</span><span class="sxs-lookup"><span data-stu-id="46798-106">The **InternetMessageHeader** element represents the Internet message header for a given header within the headers collection.</span></span> <span data-ttu-id="46798-107">Чтобы получить вся коллекция заголовков сообщений Интернета, используйте свойство **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="46798-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="46798-108">Дополнительные сведения о веб-служб Exchange и Интернет заголовки сообщений в разделе «Приступая к Интернету заголовки сообщений в [веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="46798-108">For more information about EWS and Internet message headers, see "Getting Internet message headers in [EWS, MIME, and the missing Internet message headers](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 <span data-ttu-id="46798-109">**InternetHeaderType**</span><span class="sxs-lookup"><span data-stu-id="46798-109">**InternetHeaderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46798-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46798-110">Attributes and elements</span></span>

<span data-ttu-id="46798-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="46798-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46798-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46798-112">Attributes</span></span>

|<span data-ttu-id="46798-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="46798-113">**Attribute**</span></span>|<span data-ttu-id="46798-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46798-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="46798-115">**HeaderName**</span><span class="sxs-lookup"><span data-stu-id="46798-115">**HeaderName**</span></span> <br/> |<span data-ttu-id="46798-116">Определяет имя заголовка.</span><span class="sxs-lookup"><span data-stu-id="46798-116">Identifies the header name.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="46798-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46798-117">Child elements</span></span>

<span data-ttu-id="46798-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="46798-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="46798-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46798-119">Parent elements</span></span>

|<span data-ttu-id="46798-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46798-120">**Element**</span></span>|<span data-ttu-id="46798-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46798-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46798-122">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="46798-122">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="46798-123">Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="46798-123">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="46798-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="46798-124">Text value</span></span>

<span data-ttu-id="46798-125">Текстовое значение представляет значение для заголовка.</span><span class="sxs-lookup"><span data-stu-id="46798-125">The text value represents the value for the header.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="46798-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="46798-126">Remarks</span></span>

<span data-ttu-id="46798-127">Ниже приведен управляемый API EWS расширенные определений для свойства **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="46798-127">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="46798-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="46798-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46798-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46798-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46798-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46798-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46798-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46798-131">Schema Name</span></span>  <br/> |<span data-ttu-id="46798-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="46798-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="46798-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46798-133">Validation File</span></span>  <br/> |<span data-ttu-id="46798-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46798-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46798-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46798-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="46798-136">False</span><span class="sxs-lookup"><span data-stu-id="46798-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46798-137">См. также</span><span class="sxs-lookup"><span data-stu-id="46798-137">See also</span></span>



- [<span data-ttu-id="46798-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46798-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="46798-139">Веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета</span><span class="sxs-lookup"><span data-stu-id="46798-139">EWS, MIME, and the missing Internet message headers</span></span>](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

