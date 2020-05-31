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
ms.openlocfilehash: 05eeef7f7194c1dc05be93ed13ebff93d5013e94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762690"
---
# <a name="getappmanifestsresponsemessage"></a><span data-ttu-id="012ac-103">жетаппманифестсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="012ac-103">GetAppManifestsResponseMessage</span></span>

<span data-ttu-id="012ac-104">Элемент **жетаппманифестсреспонсемессаже** указывает ответное сообщение для запроса **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="012ac-104">The **GetAppManifestsResponseMessage** element specifies the response message for a **GetAppManifests** request.</span></span> 
  
```XML
<GetAppManifestsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppManifestsResponseMessage>
```

 <span data-ttu-id="012ac-105">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="012ac-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="012ac-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="012ac-106">Attributes and elements</span></span>

<span data-ttu-id="012ac-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="012ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="012ac-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="012ac-108">Attributes</span></span>

|<span data-ttu-id="012ac-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="012ac-109">**Attribute**</span></span>|<span data-ttu-id="012ac-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="012ac-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="012ac-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="012ac-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="012ac-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="012ac-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="012ac-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="012ac-113">ResponseClass</span></span>

|<span data-ttu-id="012ac-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="012ac-114">**Value**</span></span>|<span data-ttu-id="012ac-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="012ac-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="012ac-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="012ac-116">Success</span></span>  <br/> |<span data-ttu-id="012ac-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="012ac-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="012ac-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="012ac-118">Warning</span></span>  <br/> |<span data-ttu-id="012ac-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="012ac-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="012ac-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="012ac-120">Error</span></span>  <br/> |<span data-ttu-id="012ac-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="012ac-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="012ac-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="012ac-122">Child elements</span></span>

|<span data-ttu-id="012ac-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="012ac-123">**Element**</span></span>|<span data-ttu-id="012ac-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="012ac-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="012ac-125">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="012ac-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="012ac-126">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="012ac-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="012ac-127">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="012ac-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="012ac-128">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="012ac-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="012ac-129">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="012ac-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="012ac-130">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="012ac-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="012ac-131">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="012ac-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="012ac-132">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="012ac-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="012ac-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="012ac-133">Parent elements</span></span>

|<span data-ttu-id="012ac-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="012ac-134">**Element**</span></span>|<span data-ttu-id="012ac-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="012ac-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="012ac-136">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="012ac-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="012ac-137">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="012ac-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="012ac-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="012ac-138">Remarks</span></span>

<span data-ttu-id="012ac-139">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="012ac-139">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="012ac-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="012ac-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="012ac-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="012ac-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="012ac-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="012ac-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="012ac-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="012ac-143">Schema Name</span></span>  <br/> |<span data-ttu-id="012ac-144">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="012ac-144">Message schema</span></span>  <br/> |
|<span data-ttu-id="012ac-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="012ac-145">Validation File</span></span>  <br/> |<span data-ttu-id="012ac-146">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="012ac-146">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="012ac-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="012ac-147">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="012ac-148">См. также</span><span class="sxs-lookup"><span data-stu-id="012ac-148">See also</span></span>



- [<span data-ttu-id="012ac-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="012ac-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

