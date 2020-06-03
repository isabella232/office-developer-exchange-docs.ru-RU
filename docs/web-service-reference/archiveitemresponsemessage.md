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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463393"
---
# <a name="archiveitemresponsemessage"></a><span data-ttu-id="dfc94-103">арчивеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="dfc94-103">ArchiveItemResponseMessage</span></span>

<span data-ttu-id="dfc94-104">Элемент **арчивеитемреспонсемессаже** указывает ответное сообщение на запрос **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="dfc94-104">The **ArchiveItemResponseMessage** element specifies the response message to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponseMessage ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
    <Items></Items>
</ArchiveItemResponseMessage>
```

 <span data-ttu-id="dfc94-105">**итеминфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="dfc94-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dfc94-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dfc94-106">Attributes and elements</span></span>

<span data-ttu-id="dfc94-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dfc94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dfc94-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dfc94-108">Attributes</span></span>

|<span data-ttu-id="dfc94-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="dfc94-109">**Attribute**</span></span>|<span data-ttu-id="dfc94-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dfc94-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dfc94-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="dfc94-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="dfc94-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="dfc94-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="dfc94-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="dfc94-113">ResponseClass</span></span>

|<span data-ttu-id="dfc94-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="dfc94-114">**Value**</span></span>|<span data-ttu-id="dfc94-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dfc94-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dfc94-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="dfc94-116">Success</span></span>  <br/> |<span data-ttu-id="dfc94-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="dfc94-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="dfc94-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="dfc94-118">Warning</span></span>  <br/> |<span data-ttu-id="dfc94-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="dfc94-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="dfc94-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="dfc94-120">Error</span></span>  <br/> |<span data-ttu-id="dfc94-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="dfc94-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dfc94-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dfc94-122">Child elements</span></span>

|<span data-ttu-id="dfc94-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dfc94-123">**Element**</span></span>|<span data-ttu-id="dfc94-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dfc94-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dfc94-125">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="dfc94-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="dfc94-126">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="dfc94-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="dfc94-127">Items</span><span class="sxs-lookup"><span data-stu-id="dfc94-127">Items</span></span>](items.md) <br/> |<span data-ttu-id="dfc94-128">Содержит массив элементов.</span><span class="sxs-lookup"><span data-stu-id="dfc94-128">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="dfc94-129">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="dfc94-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="dfc94-130">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="dfc94-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="dfc94-131">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="dfc94-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="dfc94-132">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="dfc94-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="dfc94-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="dfc94-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="dfc94-134">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="dfc94-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dfc94-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dfc94-135">Parent elements</span></span>

|<span data-ttu-id="dfc94-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dfc94-136">**Element**</span></span>|<span data-ttu-id="dfc94-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dfc94-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dfc94-138">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="dfc94-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dfc94-139">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfc94-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dfc94-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="dfc94-140">Remarks</span></span>

<span data-ttu-id="dfc94-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="dfc94-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dfc94-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dfc94-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dfc94-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dfc94-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dfc94-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dfc94-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dfc94-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dfc94-145">Schema Name</span></span>  <br/> |<span data-ttu-id="dfc94-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="dfc94-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="dfc94-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dfc94-147">Validation File</span></span>  <br/> |<span data-ttu-id="dfc94-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dfc94-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dfc94-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dfc94-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="dfc94-150">См. также</span><span class="sxs-lookup"><span data-stu-id="dfc94-150">See also</span></span>

- [<span data-ttu-id="dfc94-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dfc94-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

