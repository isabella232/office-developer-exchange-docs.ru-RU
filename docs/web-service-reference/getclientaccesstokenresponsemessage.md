---
title: жетклиентакцесстокенреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 45ca2500-ceab-4c98-9576-cb9e158e5896
description: Элемент Жетклиентакцесстокенреспонсемессаже указывает ответное сообщение для запроса GetClientAccessToken.
ms.openlocfilehash: 16fe684dd48f77156ed88d02a6ae7b8f3312cd87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762714"
---
# <a name="getclientaccesstokenresponsemessage"></a><span data-ttu-id="e3f0e-103">жетклиентакцесстокенреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="e3f0e-103">GetClientAccessTokenResponseMessage</span></span>

<span data-ttu-id="e3f0e-104">Элемент **жетклиентакцесстокенреспонсемессаже** указывает ответное сообщение для запроса **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="e3f0e-104">The **GetClientAccessTokenResponseMessage** element specifies the response message for a **GetClientAccessToken** request.</span></span> 
  
```XML
<GetClientAccessTokenResponseMessage ResponseClass=" Success | Warning | Error ">
    <Token/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetClientAccessTokenResponseMessage>
```

 <span data-ttu-id="e3f0e-105">**жетклиентакцесстокенреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e3f0e-105">**GetClientAccessTokenResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3f0e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e3f0e-106">Attributes and elements</span></span>

<span data-ttu-id="e3f0e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3f0e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e3f0e-108">Attributes</span></span>

|<span data-ttu-id="e3f0e-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e3f0e-109">**Attribute**</span></span>|<span data-ttu-id="e3f0e-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3f0e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e3f0e-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="e3f0e-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="e3f0e-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="e3f0e-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="e3f0e-113">ResponseClass</span></span>

|<span data-ttu-id="e3f0e-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e3f0e-114">**Value**</span></span>|<span data-ttu-id="e3f0e-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3f0e-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e3f0e-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="e3f0e-116">Success</span></span>  <br/> |<span data-ttu-id="e3f0e-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="e3f0e-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="e3f0e-118">Warning</span></span>  <br/> |<span data-ttu-id="e3f0e-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="e3f0e-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="e3f0e-120">Error</span></span>  <br/> |<span data-ttu-id="e3f0e-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e3f0e-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e3f0e-122">Child elements</span></span>

|<span data-ttu-id="e3f0e-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e3f0e-123">**Element**</span></span>|<span data-ttu-id="e3f0e-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3f0e-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3f0e-125">Маркер (Клиентакцесстокентипе)</span><span class="sxs-lookup"><span data-stu-id="e3f0e-125">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md) <br/> |<span data-ttu-id="e3f0e-126">Указывает маркер клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-126">Specifies a client access token.</span></span>  <br/> |
|[<span data-ttu-id="e3f0e-127">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="e3f0e-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e3f0e-128">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="e3f0e-129">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="e3f0e-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e3f0e-130">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e3f0e-131">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="e3f0e-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e3f0e-132">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e3f0e-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="e3f0e-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e3f0e-134">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3f0e-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e3f0e-135">Parent elements</span></span>

|<span data-ttu-id="e3f0e-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e3f0e-136">**Element**</span></span>|<span data-ttu-id="e3f0e-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3f0e-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3f0e-138">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="e3f0e-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e3f0e-139">Содержит сообщения ответа для запроса веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="e3f0e-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e3f0e-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="e3f0e-140">Remarks</span></span>

<span data-ttu-id="e3f0e-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e3f0e-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e3f0e-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3f0e-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e3f0e-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3f0e-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e3f0e-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e3f0e-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e3f0e-145">Schema Name</span></span>  <br/> |<span data-ttu-id="e3f0e-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="e3f0e-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="e3f0e-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e3f0e-147">Validation File</span></span>  <br/> |<span data-ttu-id="e3f0e-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e3f0e-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e3f0e-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e3f0e-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e3f0e-150">См. также</span><span class="sxs-lookup"><span data-stu-id="e3f0e-150">See also</span></span>



- [<span data-ttu-id="e3f0e-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e3f0e-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

