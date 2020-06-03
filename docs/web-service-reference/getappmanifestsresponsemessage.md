---
title: жетаппманифестсреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 815908f1-4223-42d8-92dc-f8bdfc6b5df8
description: Элемент Жетаппманифестсреспонсемессаже указывает ответное сообщение для запроса GetAppManifests.
ms.openlocfilehash: 26a521d8647a010fe956596eaf63d4df4756edb2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459534"
---
# <a name="getappmanifestsresponsemessage"></a><span data-ttu-id="4aac8-103">жетаппманифестсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="4aac8-103">GetAppManifestsResponseMessage</span></span>

<span data-ttu-id="4aac8-104">Элемент **жетаппманифестсреспонсемессаже** указывает ответное сообщение для запроса **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="4aac8-104">The **GetAppManifestsResponseMessage** element specifies the response message for a **GetAppManifests** request.</span></span> 
  
```XML
<GetAppManifestsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppManifestsResponseMessage>
```

 <span data-ttu-id="4aac8-105">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="4aac8-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4aac8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4aac8-106">Attributes and elements</span></span>

<span data-ttu-id="4aac8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4aac8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4aac8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4aac8-108">Attributes</span></span>

|<span data-ttu-id="4aac8-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4aac8-109">**Attribute**</span></span>|<span data-ttu-id="4aac8-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4aac8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4aac8-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="4aac8-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="4aac8-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="4aac8-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="4aac8-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="4aac8-113">ResponseClass</span></span>

|<span data-ttu-id="4aac8-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4aac8-114">**Value**</span></span>|<span data-ttu-id="4aac8-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4aac8-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4aac8-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="4aac8-116">Success</span></span>  <br/> |<span data-ttu-id="4aac8-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="4aac8-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="4aac8-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="4aac8-118">Warning</span></span>  <br/> |<span data-ttu-id="4aac8-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="4aac8-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="4aac8-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="4aac8-120">Error</span></span>  <br/> |<span data-ttu-id="4aac8-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="4aac8-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4aac8-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4aac8-122">Child elements</span></span>

|<span data-ttu-id="4aac8-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4aac8-123">**Element**</span></span>|<span data-ttu-id="4aac8-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4aac8-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4aac8-125">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="4aac8-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4aac8-126">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="4aac8-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="4aac8-127">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="4aac8-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4aac8-128">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="4aac8-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4aac8-129">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="4aac8-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4aac8-130">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4aac8-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4aac8-131">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="4aac8-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4aac8-132">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="4aac8-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4aac8-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4aac8-133">Parent elements</span></span>

|<span data-ttu-id="4aac8-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4aac8-134">**Element**</span></span>|<span data-ttu-id="4aac8-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4aac8-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4aac8-136">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="4aac8-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4aac8-137">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4aac8-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4aac8-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="4aac8-138">Remarks</span></span>

<span data-ttu-id="4aac8-139">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4aac8-139">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4aac8-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4aac8-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4aac8-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4aac8-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4aac8-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4aac8-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4aac8-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4aac8-143">Schema Name</span></span>  <br/> |<span data-ttu-id="4aac8-144">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="4aac8-144">Message schema</span></span>  <br/> |
|<span data-ttu-id="4aac8-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4aac8-145">Validation File</span></span>  <br/> |<span data-ttu-id="4aac8-146">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4aac8-146">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4aac8-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4aac8-147">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4aac8-148">См. также</span><span class="sxs-lookup"><span data-stu-id="4aac8-148">See also</span></span>



- [<span data-ttu-id="4aac8-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4aac8-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

