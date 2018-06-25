---
title: GetSearchableMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f45865fd-4626-4d80-84f6-7989339fdd85
description: Элемент GetSearchableMailboxesResponseMessage указывает сообщение ответа на запрос GetSearchableMailboxes.
ms.openlocfilehash: 2a4d1fe357656fe29d8572e7f32a4bc2e4a6131e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762916"
---
# <a name="getsearchablemailboxesresponsemessage"></a><span data-ttu-id="e82ee-103">GetSearchableMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e82ee-103">GetSearchableMailboxesResponseMessage</span></span>

<span data-ttu-id="e82ee-104">Элемент **GetSearchableMailboxesResponseMessage** указывает сообщение ответа на запрос **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="e82ee-104">The **GetSearchableMailboxesResponseMessage** element specifies the response message for a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <SearchableMailboxes/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetSearchablemailboxesResponseMessage>
```

 <span data-ttu-id="e82ee-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e82ee-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e82ee-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e82ee-106">Attributes and elements</span></span>

<span data-ttu-id="e82ee-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e82ee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e82ee-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e82ee-108">Attributes</span></span>

|<span data-ttu-id="e82ee-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e82ee-109">**Attribute**</span></span>|<span data-ttu-id="e82ee-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e82ee-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e82ee-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e82ee-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="e82ee-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="e82ee-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="e82ee-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e82ee-113">ResponseClass</span></span>

|<span data-ttu-id="e82ee-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e82ee-114">**Value**</span></span>|<span data-ttu-id="e82ee-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e82ee-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e82ee-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="e82ee-116">Success</span></span>  <br/> |<span data-ttu-id="e82ee-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="e82ee-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="e82ee-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="e82ee-118">Warning</span></span>  <br/> |<span data-ttu-id="e82ee-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="e82ee-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="e82ee-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="e82ee-120">Error</span></span>  <br/> |<span data-ttu-id="e82ee-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e82ee-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e82ee-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e82ee-122">Child elements</span></span>

|<span data-ttu-id="e82ee-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e82ee-123">**Element**</span></span>|<span data-ttu-id="e82ee-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e82ee-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e82ee-125">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="e82ee-125">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="e82ee-126">Содержит массив почтовых ящиков, возвращаемый запросом **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="e82ee-126">Contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="e82ee-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e82ee-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e82ee-128">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="e82ee-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="e82ee-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="e82ee-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e82ee-130">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="e82ee-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e82ee-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e82ee-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e82ee-132">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="e82ee-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e82ee-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e82ee-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e82ee-134">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="e82ee-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e82ee-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e82ee-135">Parent elements</span></span>

|<span data-ttu-id="e82ee-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e82ee-136">**Element**</span></span>|<span data-ttu-id="e82ee-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e82ee-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e82ee-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e82ee-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e82ee-139">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e82ee-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e82ee-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="e82ee-140">Remarks</span></span>

<span data-ttu-id="e82ee-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e82ee-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e82ee-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e82ee-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e82ee-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e82ee-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e82ee-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e82ee-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e82ee-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e82ee-145">Schema Name</span></span>  <br/> |<span data-ttu-id="e82ee-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="e82ee-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="e82ee-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e82ee-147">Validation File</span></span>  <br/> |<span data-ttu-id="e82ee-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e82ee-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e82ee-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e82ee-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e82ee-150">См. также</span><span class="sxs-lookup"><span data-stu-id="e82ee-150">See also</span></span>



- [<span data-ttu-id="e82ee-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e82ee-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

