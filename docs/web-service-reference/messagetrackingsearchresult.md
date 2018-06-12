---
title: MessageTrackingSearchResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: Элемент MessageTrackingSearchResult содержит результат одного сообщения для элемента FindMessageTrackingReportResponse.
ms.openlocfilehash: ad4fb9d9e2266222303bd2015a7afba0bb46721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834460"
---
# <a name="messagetrackingsearchresult"></a><span data-ttu-id="e0896-103">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="e0896-103">MessageTrackingSearchResult</span></span>

<span data-ttu-id="e0896-104">Элемент **MessageTrackingSearchResult** содержит результат одного сообщения для элемента [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="e0896-104">The **MessageTrackingSearchResult** element contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span> 
  
```xml
<MessageTrackingSearchResult>
   <Subject/>
   <Sender/>
   <PurportedSender/>
   <Recipients/>
   <SubmittedTime/>
   <MessageTrackingReportId/>
   <PreviousHopServer/>
   <FirstHopServer/>
   <Properties/>
</MessageTrackingSearchResult>
```

 <span data-ttu-id="e0896-105">**FindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="e0896-105">**FindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0896-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e0896-106">Attributes and elements</span></span>

<span data-ttu-id="e0896-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e0896-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0896-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e0896-108">Attributes</span></span>

<span data-ttu-id="e0896-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e0896-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e0896-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e0896-110">Child elements</span></span>

|<span data-ttu-id="e0896-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e0896-111">**Element**</span></span>|<span data-ttu-id="e0896-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0896-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0896-113">Subject</span><span class="sxs-lookup"><span data-stu-id="e0896-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="e0896-114">Содержит тему сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e0896-114">Contains the e-mail message subject.</span></span>  <br/> |
|[<span data-ttu-id="e0896-115">Отправитель (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e0896-115">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="e0896-116">Содержит адрес электронной почты отправителя сообщения.</span><span class="sxs-lookup"><span data-stu-id="e0896-116">Contains the e-mail message sender's address.</span></span>  <br/> |
|[<span data-ttu-id="e0896-117">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="e0896-117">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="e0896-118">Содержит контактные данные для утверждения отправителя сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e0896-118">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e0896-119">Получатели (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="e0896-119">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="e0896-120">Содержит список адресов электронной почты, которые получены этого сообщения.</span><span class="sxs-lookup"><span data-stu-id="e0896-120">Contains a list of e-mail addresses that received this message.</span></span>  <br/> |
|[<span data-ttu-id="e0896-121">SubmittedTime</span><span class="sxs-lookup"><span data-stu-id="e0896-121">SubmittedTime</span></span>](submittedtime.md) <br/> |<span data-ttu-id="e0896-122">Содержит время, когда сообщение было отправлено.</span><span class="sxs-lookup"><span data-stu-id="e0896-122">Contains the time that the message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="e0896-123">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="e0896-123">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="e0896-124">Содержит внутренний идентификатор сообщения в базе данных транспорта.</span><span class="sxs-lookup"><span data-stu-id="e0896-124">Contains an internal ID that identifies the message in the transport database.</span></span>  <br/> |
|[<span data-ttu-id="e0896-125">PreviousHopServer</span><span class="sxs-lookup"><span data-stu-id="e0896-125">PreviousHopServer</span></span>](previoushopserver.md) <br/> |<span data-ttu-id="e0896-126">Содержит имя сервера в лесу, которые ранее принимает сообщение.</span><span class="sxs-lookup"><span data-stu-id="e0896-126">Contains the name of the server in the forest that previously accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="e0896-127">FirstHopServer</span><span class="sxs-lookup"><span data-stu-id="e0896-127">FirstHopServer</span></span>](firsthopserver.md) <br/> |<span data-ttu-id="e0896-128">Содержит имя сервера в лесу, сначала принято сообщение.</span><span class="sxs-lookup"><span data-stu-id="e0896-128">Contains the name of the server in the forest that first accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="e0896-129">Свойства (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="e0896-129">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="e0896-130">Содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="e0896-130">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e0896-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e0896-131">Parent elements</span></span>

|<span data-ttu-id="e0896-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e0896-132">**Element**</span></span>|<span data-ttu-id="e0896-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0896-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0896-134">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="e0896-134">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="e0896-135">Содержит список сообщений, которые соответствуют условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="e0896-135">Contains a list of messages that match the search criteria.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e0896-136">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e0896-136">Text value</span></span>

<span data-ttu-id="e0896-137">Нет.</span><span class="sxs-lookup"><span data-stu-id="e0896-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e0896-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="e0896-138">Remarks</span></span>

<span data-ttu-id="e0896-139">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e0896-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0896-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e0896-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0896-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e0896-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0896-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e0896-142">Schema Name</span></span>  <br/> |<span data-ttu-id="e0896-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e0896-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0896-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e0896-144">Validation File</span></span>  <br/> |<span data-ttu-id="e0896-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e0896-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0896-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e0896-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0896-147">False</span><span class="sxs-lookup"><span data-stu-id="e0896-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0896-148">См. также</span><span class="sxs-lookup"><span data-stu-id="e0896-148">See also</span></span>



[<span data-ttu-id="e0896-149">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="e0896-149">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="e0896-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e0896-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

