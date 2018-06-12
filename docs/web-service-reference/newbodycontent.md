---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: Элемент NewBodyContent представляет новое содержимое текста сообщения.
ms.openlocfilehash: b87393e460b1eee1c13efebf38e898d17915bd71
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834516"
---
# <a name="newbodycontent"></a><span data-ttu-id="6301f-103">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="6301f-103">NewBodyContent</span></span>

<span data-ttu-id="6301f-104">Элемент **NewBodyContent** представляет новое содержимое текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="6301f-104">The **NewBodyContent** element represents the new body content of a message.</span></span> 
  
```xml
<NewBodyContent BodyType=""/>
```

 <span data-ttu-id="6301f-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="6301f-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6301f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6301f-106">Attributes and elements</span></span>

<span data-ttu-id="6301f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6301f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6301f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6301f-108">Attributes</span></span>

|<span data-ttu-id="6301f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6301f-109">**Attribute**</span></span>|<span data-ttu-id="6301f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6301f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6301f-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="6301f-111">**BodyType**</span></span> <br/> |<span data-ttu-id="6301f-112">Представляет фактическое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="6301f-112">Represents the actual body content of a message.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="6301f-113">Атрибут типа текста сообщения</span><span class="sxs-lookup"><span data-stu-id="6301f-113">BodyType Attribute</span></span>

|<span data-ttu-id="6301f-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="6301f-114">**Value**</span></span>|<span data-ttu-id="6301f-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6301f-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6301f-116">**HTML-КОД**</span><span class="sxs-lookup"><span data-stu-id="6301f-116">**HTML**</span></span> <br/> |<span data-ttu-id="6301f-117">Преобразует все тексты в HTML-код.</span><span class="sxs-lookup"><span data-stu-id="6301f-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="6301f-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="6301f-118">**Text**</span></span> <br/> |<span data-ttu-id="6301f-119">Преобразует все тексты в обычный текст.</span><span class="sxs-lookup"><span data-stu-id="6301f-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6301f-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6301f-120">Child elements</span></span>

<span data-ttu-id="6301f-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="6301f-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6301f-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6301f-122">Parent elements</span></span>

|<span data-ttu-id="6301f-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6301f-123">**Element**</span></span>|<span data-ttu-id="6301f-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6301f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6301f-125">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="6301f-125">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="6301f-126">Содержит ответ отправителя элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6301f-126">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6301f-127">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="6301f-127">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="6301f-128">Содержит ответ для отправителя и всех указанных получателей элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6301f-128">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6301f-129">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="6301f-129">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="6301f-130">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="6301f-130">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="6301f-131">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="6301f-131">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="6301f-132">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="6301f-132">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="6301f-133">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="6301f-133">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="6301f-134">Содержит ответ элемента записи.</span><span class="sxs-lookup"><span data-stu-id="6301f-134">Contains a reply to a post item.</span></span> <span data-ttu-id="6301f-135">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6301f-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6301f-136">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6301f-136">Text value</span></span>

<span data-ttu-id="6301f-137">Текстовое значение представляет новое содержимое текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="6301f-137">The text value represents the new body content of a message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6301f-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="6301f-138">Remarks</span></span>

<span data-ttu-id="6301f-139">Схема, описывающая этот элемент находится в виртуальном каталоге EWS сервера Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6301f-139">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6301f-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6301f-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6301f-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6301f-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6301f-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6301f-142">Schema Name</span></span>  <br/> |<span data-ttu-id="6301f-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6301f-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="6301f-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6301f-144">Validation File</span></span>  <br/> |<span data-ttu-id="6301f-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6301f-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6301f-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6301f-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="6301f-147">False</span><span class="sxs-lookup"><span data-stu-id="6301f-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6301f-148">См. также</span><span class="sxs-lookup"><span data-stu-id="6301f-148">See also</span></span>



- [<span data-ttu-id="6301f-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6301f-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

