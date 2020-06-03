---
title: жетконверсатионитемсреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2e930650-7848-4bf2-a975-026309b3ea02
description: Элемент Жетконверсатионитемсреспонсемессаже указывает ответное сообщение для запроса GetConversationItems.
ms.openlocfilehash: b38bca60bb51c24a7635391c4e23e5426366cd72
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461074"
---
# <a name="getconversationitemsresponsemessage"></a><span data-ttu-id="13a1f-103">жетконверсатионитемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="13a1f-103">GetConversationItemsResponseMessage</span></span>

<span data-ttu-id="13a1f-104">Элемент **жетконверсатионитемсреспонсемессаже** указывает ответное сообщение для запроса **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="13a1f-104">The **GetConversationItemsResponseMessage** element specifies the response message for a **GetConversationItems** request.</span></span> 
  
```XML
<GetConversationItemsResponseMessage ResponseClass="Success | Warning | Error">
    <Conversation/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetConversationItemsResponseMessage>
```

 <span data-ttu-id="13a1f-105">**жетконверсатионитемсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="13a1f-105">**GetConversationItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13a1f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="13a1f-106">Attributes and elements</span></span>

<span data-ttu-id="13a1f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="13a1f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13a1f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="13a1f-108">Attributes</span></span>

|<span data-ttu-id="13a1f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="13a1f-109">**Attribute**</span></span>|<span data-ttu-id="13a1f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="13a1f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="13a1f-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="13a1f-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="13a1f-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="13a1f-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="13a1f-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="13a1f-113">ResponseClass</span></span>

|<span data-ttu-id="13a1f-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="13a1f-114">**Value**</span></span>|<span data-ttu-id="13a1f-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="13a1f-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="13a1f-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="13a1f-116">Success</span></span>  <br/> |<span data-ttu-id="13a1f-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="13a1f-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="13a1f-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="13a1f-118">Warning</span></span>  <br/> |<span data-ttu-id="13a1f-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="13a1f-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="13a1f-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="13a1f-120">Error</span></span>  <br/> |<span data-ttu-id="13a1f-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="13a1f-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="13a1f-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="13a1f-122">Child elements</span></span>

|<span data-ttu-id="13a1f-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="13a1f-123">**Element**</span></span>|<span data-ttu-id="13a1f-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="13a1f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13a1f-125">Беседа (Конверсатионреспонсетипе)</span><span class="sxs-lookup"><span data-stu-id="13a1f-125">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="13a1f-126">Представляет один диалог, возвращенный в ответе **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="13a1f-126">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
|[<span data-ttu-id="13a1f-127">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="13a1f-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="13a1f-128">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="13a1f-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="13a1f-129">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="13a1f-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="13a1f-130">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="13a1f-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="13a1f-131">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="13a1f-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="13a1f-132">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="13a1f-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="13a1f-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="13a1f-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="13a1f-134">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="13a1f-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="13a1f-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="13a1f-135">Parent elements</span></span>

|<span data-ttu-id="13a1f-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="13a1f-136">**Element**</span></span>|<span data-ttu-id="13a1f-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="13a1f-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13a1f-138">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="13a1f-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="13a1f-139">Содержит сообщения ответа для запроса веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="13a1f-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="13a1f-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="13a1f-140">Remarks</span></span>

<span data-ttu-id="13a1f-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="13a1f-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="13a1f-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="13a1f-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13a1f-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="13a1f-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13a1f-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="13a1f-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="13a1f-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="13a1f-145">Schema Name</span></span>  <br/> |<span data-ttu-id="13a1f-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="13a1f-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="13a1f-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="13a1f-147">Validation File</span></span>  <br/> |<span data-ttu-id="13a1f-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="13a1f-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="13a1f-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="13a1f-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="13a1f-150">См. также</span><span class="sxs-lookup"><span data-stu-id="13a1f-150">See also</span></span>



- [<span data-ttu-id="13a1f-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="13a1f-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

