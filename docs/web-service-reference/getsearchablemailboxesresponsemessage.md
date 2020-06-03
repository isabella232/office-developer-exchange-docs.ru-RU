---
title: жетсеарчаблемаилбоксесреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f45865fd-4626-4d80-84f6-7989339fdd85
description: Элемент Жетсеарчаблемаилбоксесреспонсемессаже указывает ответное сообщение для запроса GetSearchableMailboxes.
ms.openlocfilehash: 69f45d87cfbd398013d021cdd39b55497d78ae04
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458259"
---
# <a name="getsearchablemailboxesresponsemessage"></a><span data-ttu-id="e9716-103">жетсеарчаблемаилбоксесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="e9716-103">GetSearchableMailboxesResponseMessage</span></span>

<span data-ttu-id="e9716-104">Элемент **жетсеарчаблемаилбоксесреспонсемессаже** указывает ответное сообщение для запроса **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="e9716-104">The **GetSearchableMailboxesResponseMessage** element specifies the response message for a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <SearchableMailboxes/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetSearchablemailboxesResponseMessage>
```

 <span data-ttu-id="e9716-105">**жетсеарчаблемаилбоксесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e9716-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9716-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e9716-106">Attributes and elements</span></span>

<span data-ttu-id="e9716-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e9716-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9716-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e9716-108">Attributes</span></span>

|<span data-ttu-id="e9716-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e9716-109">**Attribute**</span></span>|<span data-ttu-id="e9716-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e9716-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9716-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="e9716-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="e9716-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="e9716-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="e9716-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="e9716-113">ResponseClass</span></span>

|<span data-ttu-id="e9716-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e9716-114">**Value**</span></span>|<span data-ttu-id="e9716-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e9716-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9716-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="e9716-116">Success</span></span>  <br/> |<span data-ttu-id="e9716-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="e9716-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="e9716-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="e9716-118">Warning</span></span>  <br/> |<span data-ttu-id="e9716-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="e9716-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="e9716-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="e9716-120">Error</span></span>  <br/> |<span data-ttu-id="e9716-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="e9716-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e9716-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e9716-122">Child elements</span></span>

|<span data-ttu-id="e9716-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e9716-123">**Element**</span></span>|<span data-ttu-id="e9716-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e9716-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9716-125">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="e9716-125">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="e9716-126">Содержит массив почтовых ящиков, возвращенных из запроса **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="e9716-126">Contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="e9716-127">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="e9716-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e9716-128">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="e9716-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="e9716-129">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="e9716-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e9716-130">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="e9716-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e9716-131">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="e9716-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e9716-132">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e9716-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e9716-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="e9716-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e9716-134">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="e9716-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9716-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e9716-135">Parent elements</span></span>

|<span data-ttu-id="e9716-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e9716-136">**Element**</span></span>|<span data-ttu-id="e9716-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e9716-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9716-138">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="e9716-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e9716-139">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9716-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9716-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="e9716-140">Remarks</span></span>

<span data-ttu-id="e9716-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e9716-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e9716-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9716-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9716-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e9716-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9716-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e9716-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e9716-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e9716-145">Schema Name</span></span>  <br/> |<span data-ttu-id="e9716-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="e9716-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="e9716-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e9716-147">Validation File</span></span>  <br/> |<span data-ttu-id="e9716-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e9716-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e9716-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e9716-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e9716-150">См. также</span><span class="sxs-lookup"><span data-stu-id="e9716-150">See also</span></span>



- [<span data-ttu-id="e9716-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e9716-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

