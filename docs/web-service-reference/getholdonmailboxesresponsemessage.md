---
title: GetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7d0d90-d418-4ce9-8cea-afe8f14728c3
description: Элемент GetHoldOnMailboxesResponseMessage указывает сообщение ответа на запрос GetHoldOnMailboxes.
ms.openlocfilehash: e1c43f75bfa62b20de9248546e71c92ae5998ed9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762808"
---
# <a name="getholdonmailboxesresponsemessage"></a><span data-ttu-id="f4f99-103">GetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f4f99-103">GetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="f4f99-104">Элемент **GetHoldOnMailboxesResponseMessage** указывает сообщение ответа на запрос **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="f4f99-104">The **GetHoldOnMailboxesResponseMessage** element specifies the response message for a **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<GetHoldOnMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxHoldResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="f4f99-105">**GetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f4f99-105">**GetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4f99-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f4f99-106">Attributes and elements</span></span>

<span data-ttu-id="f4f99-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f4f99-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4f99-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f4f99-108">Attributes</span></span>

|<span data-ttu-id="f4f99-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f4f99-109">**Attribute**</span></span>|<span data-ttu-id="f4f99-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4f99-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f4f99-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f4f99-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="f4f99-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="f4f99-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="f4f99-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f4f99-113">ResponseClass</span></span>

|<span data-ttu-id="f4f99-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f4f99-114">**Value**</span></span>|<span data-ttu-id="f4f99-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4f99-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f4f99-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="f4f99-116">Success</span></span>  <br/> |<span data-ttu-id="f4f99-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="f4f99-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="f4f99-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="f4f99-118">Warning</span></span>  <br/> |<span data-ttu-id="f4f99-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="f4f99-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="f4f99-120">Error</span><span class="sxs-lookup"><span data-stu-id="f4f99-120">Error</span></span>  <br/> |<span data-ttu-id="f4f99-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f4f99-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f4f99-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f4f99-122">Child elements</span></span>

|<span data-ttu-id="f4f99-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f4f99-123">**Element**</span></span>|<span data-ttu-id="f4f99-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4f99-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4f99-125">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="f4f99-125">MailboxHoldResult</span></span>](mailboxholdresult.md) <br/> |<span data-ttu-id="f4f99-126">Содержит результат запроса **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="f4f99-126">Contains the result of the **GetHoldOnMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="f4f99-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f4f99-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f4f99-128">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="f4f99-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="f4f99-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="f4f99-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f4f99-130">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="f4f99-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f4f99-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f4f99-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f4f99-132">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="f4f99-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f4f99-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f4f99-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f4f99-134">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="f4f99-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f4f99-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f4f99-135">Parent elements</span></span>

|<span data-ttu-id="f4f99-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f4f99-136">**Element**</span></span>|<span data-ttu-id="f4f99-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4f99-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4f99-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f4f99-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f4f99-139">Содержит сообщения ответа на запрос веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="f4f99-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f4f99-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="f4f99-140">Remarks</span></span>

<span data-ttu-id="f4f99-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f4f99-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f4f99-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4f99-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4f99-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f4f99-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4f99-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f4f99-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4f99-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f4f99-145">Schema Name</span></span>  <br/> |<span data-ttu-id="f4f99-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="f4f99-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="f4f99-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f4f99-147">Validation File</span></span>  <br/> |<span data-ttu-id="f4f99-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f4f99-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4f99-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f4f99-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f4f99-150">См. также</span><span class="sxs-lookup"><span data-stu-id="f4f99-150">See also</span></span>



- [<span data-ttu-id="f4f99-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f4f99-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

