---
title: арчивеитемреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2ac58d6f-e019-4352-b82f-8ac67a171e63
description: Элемент Арчивеитемреспонсемессаже указывает ответное сообщение на запрос ArchiveItem.
ms.openlocfilehash: 24d09d63cab6805194e35031d8590290573de0a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463393"
---
# <a name="archiveitemresponsemessage"></a><span data-ttu-id="0cb97-103">арчивеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="0cb97-103">ArchiveItemResponseMessage</span></span>

<span data-ttu-id="0cb97-104">Элемент **арчивеитемреспонсемессаже** указывает ответное сообщение на запрос **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="0cb97-104">The **ArchiveItemResponseMessage** element specifies the response message to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponseMessage ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
    <Items></Items>
</ArchiveItemResponseMessage>
```

 <span data-ttu-id="0cb97-105">**итеминфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="0cb97-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0cb97-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0cb97-106">Attributes and elements</span></span>

<span data-ttu-id="0cb97-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0cb97-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0cb97-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0cb97-108">Attributes</span></span>

|<span data-ttu-id="0cb97-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0cb97-109">**Attribute**</span></span>|<span data-ttu-id="0cb97-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0cb97-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0cb97-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="0cb97-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="0cb97-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="0cb97-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="0cb97-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="0cb97-113">ResponseClass</span></span>

|<span data-ttu-id="0cb97-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0cb97-114">**Value**</span></span>|<span data-ttu-id="0cb97-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0cb97-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0cb97-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="0cb97-116">Success</span></span>  <br/> |<span data-ttu-id="0cb97-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="0cb97-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="0cb97-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="0cb97-118">Warning</span></span>  <br/> |<span data-ttu-id="0cb97-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="0cb97-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="0cb97-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="0cb97-120">Error</span></span>  <br/> |<span data-ttu-id="0cb97-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="0cb97-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0cb97-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0cb97-122">Child elements</span></span>

|<span data-ttu-id="0cb97-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0cb97-123">**Element**</span></span>|<span data-ttu-id="0cb97-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0cb97-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cb97-125">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="0cb97-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0cb97-126">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="0cb97-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="0cb97-127">Items</span><span class="sxs-lookup"><span data-stu-id="0cb97-127">Items</span></span>](items.md) <br/> |<span data-ttu-id="0cb97-128">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="0cb97-128">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="0cb97-129">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="0cb97-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0cb97-130">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="0cb97-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0cb97-131">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="0cb97-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0cb97-132">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="0cb97-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0cb97-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="0cb97-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0cb97-134">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="0cb97-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0cb97-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0cb97-135">Parent elements</span></span>

|<span data-ttu-id="0cb97-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0cb97-136">**Element**</span></span>|<span data-ttu-id="0cb97-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0cb97-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cb97-138">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="0cb97-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0cb97-139">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="0cb97-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0cb97-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="0cb97-140">Remarks</span></span>

<span data-ttu-id="0cb97-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0cb97-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0cb97-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0cb97-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0cb97-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0cb97-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0cb97-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0cb97-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0cb97-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0cb97-145">Schema Name</span></span>  <br/> |<span data-ttu-id="0cb97-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="0cb97-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="0cb97-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0cb97-147">Validation File</span></span>  <br/> |<span data-ttu-id="0cb97-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0cb97-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0cb97-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0cb97-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0cb97-150">См. также</span><span class="sxs-lookup"><span data-stu-id="0cb97-150">See also</span></span>

- [<span data-ttu-id="0cb97-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0cb97-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

