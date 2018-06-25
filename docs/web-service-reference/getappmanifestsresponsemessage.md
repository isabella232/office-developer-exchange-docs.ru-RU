---
title: GetAppManifestsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 815908f1-4223-42d8-92dc-f8bdfc6b5df8
description: Элемент GetAppManifestsResponseMessage указывает сообщение ответа на запрос GetAppManifests.
ms.openlocfilehash: 05eeef7f7194c1dc05be93ed13ebff93d5013e94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762690"
---
# <a name="getappmanifestsresponsemessage"></a><span data-ttu-id="e349c-103">GetAppManifestsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e349c-103">GetAppManifestsResponseMessage</span></span>

<span data-ttu-id="e349c-104">Элемент **GetAppManifestsResponseMessage** указывает сообщение ответа на запрос **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="e349c-104">The **GetAppManifestsResponseMessage** element specifies the response message for a **GetAppManifests** request.</span></span> 
  
```XML
<GetAppManifestsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppManifestsResponseMessage>
```

 <span data-ttu-id="e349c-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e349c-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e349c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e349c-106">Attributes and elements</span></span>

<span data-ttu-id="e349c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e349c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e349c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e349c-108">Attributes</span></span>

|<span data-ttu-id="e349c-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e349c-109">**Attribute**</span></span>|<span data-ttu-id="e349c-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e349c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e349c-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e349c-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="e349c-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="e349c-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="e349c-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e349c-113">ResponseClass</span></span>

|<span data-ttu-id="e349c-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e349c-114">**Value**</span></span>|<span data-ttu-id="e349c-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e349c-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e349c-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="e349c-116">Success</span></span>  <br/> |<span data-ttu-id="e349c-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="e349c-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="e349c-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="e349c-118">Warning</span></span>  <br/> |<span data-ttu-id="e349c-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="e349c-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="e349c-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="e349c-120">Error</span></span>  <br/> |<span data-ttu-id="e349c-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e349c-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e349c-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e349c-122">Child elements</span></span>

|<span data-ttu-id="e349c-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e349c-123">**Element**</span></span>|<span data-ttu-id="e349c-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e349c-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e349c-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e349c-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e349c-126">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="e349c-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="e349c-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="e349c-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e349c-128">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="e349c-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e349c-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e349c-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e349c-130">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="e349c-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e349c-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e349c-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e349c-132">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="e349c-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e349c-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e349c-133">Parent elements</span></span>

|<span data-ttu-id="e349c-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e349c-134">**Element**</span></span>|<span data-ttu-id="e349c-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e349c-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e349c-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e349c-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e349c-137">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e349c-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e349c-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="e349c-138">Remarks</span></span>

<span data-ttu-id="e349c-139">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e349c-139">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e349c-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e349c-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e349c-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e349c-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e349c-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e349c-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e349c-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e349c-143">Schema Name</span></span>  <br/> |<span data-ttu-id="e349c-144">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="e349c-144">Message schema</span></span>  <br/> |
|<span data-ttu-id="e349c-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e349c-145">Validation File</span></span>  <br/> |<span data-ttu-id="e349c-146">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e349c-146">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e349c-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e349c-147">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e349c-148">См. также</span><span class="sxs-lookup"><span data-stu-id="e349c-148">See also</span></span>



- [<span data-ttu-id="e349c-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e349c-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

