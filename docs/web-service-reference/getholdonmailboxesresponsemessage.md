---
title: жесолдонмаилбоксесреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7d0d90-d418-4ce9-8cea-afe8f14728c3
description: Элемент Жесолдонмаилбоксесреспонсемессаже указывает ответное сообщение для запроса GetHoldOnMailboxes.
ms.openlocfilehash: e1c43f75bfa62b20de9248546e71c92ae5998ed9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762808"
---
# <a name="getholdonmailboxesresponsemessage"></a><span data-ttu-id="befbd-103">жесолдонмаилбоксесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="befbd-103">GetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="befbd-104">Элемент **жесолдонмаилбоксесреспонсемессаже** указывает ответное сообщение для запроса **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="befbd-104">The **GetHoldOnMailboxesResponseMessage** element specifies the response message for a **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<GetHoldOnMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxHoldResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="befbd-105">**жесолдонмаилбоксесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="befbd-105">**GetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="befbd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="befbd-106">Attributes and elements</span></span>

<span data-ttu-id="befbd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="befbd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="befbd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="befbd-108">Attributes</span></span>

|<span data-ttu-id="befbd-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="befbd-109">**Attribute**</span></span>|<span data-ttu-id="befbd-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="befbd-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="befbd-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="befbd-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="befbd-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="befbd-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="befbd-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="befbd-113">ResponseClass</span></span>

|<span data-ttu-id="befbd-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="befbd-114">**Value**</span></span>|<span data-ttu-id="befbd-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="befbd-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="befbd-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="befbd-116">Success</span></span>  <br/> |<span data-ttu-id="befbd-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="befbd-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="befbd-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="befbd-118">Warning</span></span>  <br/> |<span data-ttu-id="befbd-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="befbd-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="befbd-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="befbd-120">Error</span></span>  <br/> |<span data-ttu-id="befbd-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="befbd-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="befbd-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="befbd-122">Child elements</span></span>

|<span data-ttu-id="befbd-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="befbd-123">**Element**</span></span>|<span data-ttu-id="befbd-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="befbd-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="befbd-125">маилбоксхолдресулт</span><span class="sxs-lookup"><span data-stu-id="befbd-125">MailboxHoldResult</span></span>](mailboxholdresult.md) <br/> |<span data-ttu-id="befbd-126">Содержит результат запроса **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="befbd-126">Contains the result of the **GetHoldOnMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="befbd-127">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="befbd-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="befbd-128">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="befbd-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="befbd-129">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="befbd-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="befbd-130">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="befbd-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="befbd-131">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="befbd-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="befbd-132">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="befbd-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="befbd-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="befbd-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="befbd-134">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="befbd-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="befbd-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="befbd-135">Parent elements</span></span>

|<span data-ttu-id="befbd-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="befbd-136">**Element**</span></span>|<span data-ttu-id="befbd-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="befbd-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="befbd-138">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="befbd-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="befbd-139">Содержит сообщения ответа для запроса веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="befbd-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="befbd-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="befbd-140">Remarks</span></span>

<span data-ttu-id="befbd-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="befbd-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="befbd-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="befbd-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="befbd-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="befbd-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="befbd-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="befbd-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="befbd-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="befbd-145">Schema Name</span></span>  <br/> |<span data-ttu-id="befbd-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="befbd-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="befbd-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="befbd-147">Validation File</span></span>  <br/> |<span data-ttu-id="befbd-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="befbd-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="befbd-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="befbd-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="befbd-150">См. также</span><span class="sxs-lookup"><span data-stu-id="befbd-150">See also</span></span>



- [<span data-ttu-id="befbd-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="befbd-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

