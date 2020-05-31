---
title: невбодиконтент
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
description: Элемент Невбодиконтент представляет новое содержимое основного текста сообщения.
ms.openlocfilehash: b87393e460b1eee1c13efebf38e898d17915bd71
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834516"
---
# <a name="newbodycontent"></a><span data-ttu-id="b50a8-103">невбодиконтент</span><span class="sxs-lookup"><span data-stu-id="b50a8-103">NewBodyContent</span></span>

<span data-ttu-id="b50a8-104">Элемент **невбодиконтент** представляет новое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="b50a8-104">The **NewBodyContent** element represents the new body content of a message.</span></span> 
  
```xml
<NewBodyContent BodyType=""/>
```

 <span data-ttu-id="b50a8-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="b50a8-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b50a8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b50a8-106">Attributes and elements</span></span>

<span data-ttu-id="b50a8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b50a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b50a8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b50a8-108">Attributes</span></span>

|<span data-ttu-id="b50a8-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b50a8-109">**Attribute**</span></span>|<span data-ttu-id="b50a8-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b50a8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b50a8-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="b50a8-111">**BodyType**</span></span> <br/> |<span data-ttu-id="b50a8-112">Представляет реальное содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="b50a8-112">Represents the actual body content of a message.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="b50a8-113">Атрибут BodyType</span><span class="sxs-lookup"><span data-stu-id="b50a8-113">BodyType Attribute</span></span>

|<span data-ttu-id="b50a8-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b50a8-114">**Value**</span></span>|<span data-ttu-id="b50a8-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b50a8-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b50a8-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="b50a8-116">**HTML**</span></span> <br/> |<span data-ttu-id="b50a8-117">Преобразует все тексты в HTML.</span><span class="sxs-lookup"><span data-stu-id="b50a8-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="b50a8-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="b50a8-118">**Text**</span></span> <br/> |<span data-ttu-id="b50a8-119">Преобразует все тексты в обычный текст.</span><span class="sxs-lookup"><span data-stu-id="b50a8-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b50a8-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b50a8-120">Child elements</span></span>

<span data-ttu-id="b50a8-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="b50a8-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b50a8-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b50a8-122">Parent elements</span></span>

|<span data-ttu-id="b50a8-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b50a8-123">**Element**</span></span>|<span data-ttu-id="b50a8-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b50a8-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b50a8-125">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="b50a8-125">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="b50a8-126">Содержит ответ отправителю элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b50a8-126">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b50a8-127">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="b50a8-127">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="b50a8-128">Содержит ответ на отправителя и всех идентифицированных получателей элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b50a8-128">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b50a8-129">форвардитем</span><span class="sxs-lookup"><span data-stu-id="b50a8-129">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="b50a8-130">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="b50a8-130">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="b50a8-131">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="b50a8-131">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="b50a8-132">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="b50a8-132">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="b50a8-133">постреплитем</span><span class="sxs-lookup"><span data-stu-id="b50a8-133">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="b50a8-134">Содержит ответ на элемент POST.</span><span class="sxs-lookup"><span data-stu-id="b50a8-134">Contains a reply to a post item.</span></span> <span data-ttu-id="b50a8-135">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b50a8-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b50a8-136">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b50a8-136">Text value</span></span>

<span data-ttu-id="b50a8-137">Текстовое значение представляет новое содержимое основного текста сообщения.</span><span class="sxs-lookup"><span data-stu-id="b50a8-137">The text value represents the new body content of a message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b50a8-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="b50a8-138">Remarks</span></span>

<span data-ttu-id="b50a8-139">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS сервера Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b50a8-139">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b50a8-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b50a8-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b50a8-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b50a8-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b50a8-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b50a8-142">Schema Name</span></span>  <br/> |<span data-ttu-id="b50a8-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b50a8-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="b50a8-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b50a8-144">Validation File</span></span>  <br/> |<span data-ttu-id="b50a8-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b50a8-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b50a8-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b50a8-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="b50a8-147">False</span><span class="sxs-lookup"><span data-stu-id="b50a8-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b50a8-148">См. также</span><span class="sxs-lookup"><span data-stu-id="b50a8-148">See also</span></span>



- [<span data-ttu-id="b50a8-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b50a8-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

