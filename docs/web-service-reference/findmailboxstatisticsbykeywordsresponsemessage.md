---
title: FindMailboxStatisticsByKeywordsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d3835800-8887-43db-9a8a-fe3cfea7a863
description: Элемент FindMailboxStatisticsByKeywordsResponseMessage указывает сообщение ответа на запрос FindMailboxStatisticsByKeywords.
ms.openlocfilehash: 9479252ed53335d07a6402707bc69e5eaadfa7c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762582"
---
# <a name="findmailboxstatisticsbykeywordsresponsemessage"></a><span data-ttu-id="24ad4-103">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="24ad4-103">FindMailboxStatisticsByKeywordsResponseMessage</span></span>

<span data-ttu-id="24ad4-104">Элемент **FindMailboxStatisticsByKeywordsResponseMessage** указывает сообщение ответа на запрос **FindMailboxStatisticsByKeywords** .</span><span class="sxs-lookup"><span data-stu-id="24ad4-104">The **FindMailboxStatisticsByKeywordsResponseMessage** element specifies the response message for a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxStatisticsSearchResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindMailboxStatisticsByKeywordsResponseMessage>
```

 <span data-ttu-id="24ad4-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="24ad4-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24ad4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="24ad4-106">Attributes and elements</span></span>

<span data-ttu-id="24ad4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="24ad4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24ad4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="24ad4-108">Attributes</span></span>

|<span data-ttu-id="24ad4-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="24ad4-109">**Attribute**</span></span>|<span data-ttu-id="24ad4-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24ad4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="24ad4-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="24ad4-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="24ad4-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="24ad4-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="24ad4-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="24ad4-113">ResponseClass</span></span>

|<span data-ttu-id="24ad4-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="24ad4-114">**Value**</span></span>|<span data-ttu-id="24ad4-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24ad4-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="24ad4-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="24ad4-116">Success</span></span>  <br/> |<span data-ttu-id="24ad4-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="24ad4-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="24ad4-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="24ad4-118">Warning</span></span>  <br/> |<span data-ttu-id="24ad4-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="24ad4-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="24ad4-120">Error</span><span class="sxs-lookup"><span data-stu-id="24ad4-120">Error</span></span>  <br/> |<span data-ttu-id="24ad4-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="24ad4-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="24ad4-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="24ad4-122">Child elements</span></span>

|<span data-ttu-id="24ad4-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="24ad4-123">**Element**</span></span>|<span data-ttu-id="24ad4-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24ad4-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24ad4-125">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="24ad4-125">MailboxStatisticsSearchResult</span></span>](mailboxstatisticssearchresult.md) <br/> |<span data-ttu-id="24ad4-126">Указывает результат поиска в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="24ad4-126">Specifies the result of a mailbox search.</span></span>  <br/> |
|[<span data-ttu-id="24ad4-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="24ad4-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="24ad4-128">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="24ad4-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="24ad4-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="24ad4-129">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="24ad4-130">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="24ad4-130">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="24ad4-131">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="24ad4-131">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="24ad4-132">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="24ad4-132">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="24ad4-133">MessageXml</span><span class="sxs-lookup"><span data-stu-id="24ad4-133">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="24ad4-134">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="24ad4-134">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24ad4-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="24ad4-135">Parent elements</span></span>

|<span data-ttu-id="24ad4-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="24ad4-136">**Element**</span></span>|<span data-ttu-id="24ad4-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24ad4-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24ad4-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="24ad4-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="24ad4-139">Указывает массив сообщения ответа.</span><span class="sxs-lookup"><span data-stu-id="24ad4-139">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="24ad4-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="24ad4-140">Remarks</span></span>

<span data-ttu-id="24ad4-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="24ad4-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="24ad4-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="24ad4-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24ad4-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="24ad4-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24ad4-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="24ad4-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="24ad4-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="24ad4-145">Schema Name</span></span>  <br/> |<span data-ttu-id="24ad4-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="24ad4-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="24ad4-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="24ad4-147">Validation File</span></span>  <br/> |<span data-ttu-id="24ad4-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="24ad4-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="24ad4-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="24ad4-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="24ad4-150">См. также</span><span class="sxs-lookup"><span data-stu-id="24ad4-150">See also</span></span>



- [<span data-ttu-id="24ad4-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="24ad4-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

