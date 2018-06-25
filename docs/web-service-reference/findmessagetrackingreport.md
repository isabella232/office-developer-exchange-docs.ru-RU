---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: Элемент FindMessageTrackingReport указывает критерии для типов сообщений для поиска.
ms.openlocfilehash: 77545121aa056992248c045af3f3d36566678b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762584"
---
# <a name="findmessagetrackingreport"></a><span data-ttu-id="f4216-103">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f4216-103">FindMessageTrackingReport</span></span>

<span data-ttu-id="f4216-104">Элемент **FindMessageTrackingReport** указывает критерии для типов сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="f4216-104">The **FindMessageTrackingReport** element specifies criteria for the types of messages to find.</span></span> 
  
```xml
<FindMessageTrackingReport>
   <Scope/>
   <Domain/>
   <Sender/>
   <PurportedSender/>
   <Recipient/>
   <Subject/>
   <StartDateTime/>
   <EndDateTime/>
   <MessageId/>
   <FederatedDeliveryMailbox/>
   <DiagnosticsLevel/>
   <ServerHint/>
   <Properties/>
</FindMessageTrackingReport>
```

 <span data-ttu-id="f4216-105">**FindMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="f4216-105">**FindMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4216-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f4216-106">Attributes and elements</span></span>

<span data-ttu-id="f4216-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f4216-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4216-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f4216-108">Attributes</span></span>

<span data-ttu-id="f4216-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f4216-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4216-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f4216-110">Child elements</span></span>

|<span data-ttu-id="f4216-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f4216-111">**Element**</span></span>|<span data-ttu-id="f4216-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4216-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4216-113">Область (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="f4216-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="f4216-114">Представляет, как широкое должны быть отчета отслеживания сообщений.</span><span class="sxs-lookup"><span data-stu-id="f4216-114">Represents how extensive the message tracking report should be.</span></span>  <br/> |
|[<span data-ttu-id="f4216-115">Домен (отслеживания сообщений)</span><span class="sxs-lookup"><span data-stu-id="f4216-115">Domain (Message Tracking)</span></span>](domain-message-tracking.md) <br/> |<span data-ttu-id="f4216-116">Содержит имя домена, в котором выполняется отслеживания сообщений.</span><span class="sxs-lookup"><span data-stu-id="f4216-116">Contains the name of the domain where the message tracking is executed.</span></span>  <br/> |
|[<span data-ttu-id="f4216-117">Отправитель (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="f4216-117">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="f4216-118">Контактные сведения для отправителя сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f4216-118">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="f4216-119">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="f4216-119">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="f4216-120">Содержит контактные данные для утверждения отправителя сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f4216-120">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="f4216-121">Recipient</span><span class="sxs-lookup"><span data-stu-id="f4216-121">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="f4216-122">Содержит адрес электронной почты получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="f4216-122">Contains the e-mail address for the recipient of the message.</span></span>  <br/> |
|[<span data-ttu-id="f4216-123">Subject</span><span class="sxs-lookup"><span data-stu-id="f4216-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="f4216-124">Содержит тему сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f4216-124">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="f4216-125">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="f4216-125">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="f4216-126">Содержит начальную дату и время для поиска.</span><span class="sxs-lookup"><span data-stu-id="f4216-126">Contains the starting date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="f4216-127">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="f4216-127">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="f4216-128">Содержит конечную дату и время для поиска.</span><span class="sxs-lookup"><span data-stu-id="f4216-128">Contains the ending date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="f4216-129">Код сообщения</span><span class="sxs-lookup"><span data-stu-id="f4216-129">MessageId</span></span>](messageid.md) <br/> |<span data-ttu-id="f4216-130">Содержит идентификатор сообщения для поиска.</span><span class="sxs-lookup"><span data-stu-id="f4216-130">Contains the message identifier for the search.</span></span>  <br/> |
|[<span data-ttu-id="f4216-131">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="f4216-131">FederatedDeliveryMailbox</span></span>](federateddeliverymailbox.md) <br/> |<span data-ttu-id="f4216-132">Содержит имя почтового ящика, где нескольких локальных сообщение было отправлено.</span><span class="sxs-lookup"><span data-stu-id="f4216-132">Contains the name of the mailbox where the cross-premise message was sent.</span></span>  <br/> |
|[<span data-ttu-id="f4216-133">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="f4216-133">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="f4216-134">Представляет уровень детализации для диагностических отчетов.</span><span class="sxs-lookup"><span data-stu-id="f4216-134">Represents the level of detail for diagnostic reports.</span></span>  <br/> |
|[<span data-ttu-id="f4216-135">ServerHint</span><span class="sxs-lookup"><span data-stu-id="f4216-135">ServerHint</span></span>](serverhint.md) <br/> |<span data-ttu-id="f4216-136">Представляет собой отправную точку для отслеживания сообщений в удаленной сети или в лесу.</span><span class="sxs-lookup"><span data-stu-id="f4216-136">Represents the starting point for tracking a message in a remote site or forest.</span></span>  <br/> |
|[<span data-ttu-id="f4216-137">Свойства (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="f4216-137">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="f4216-138">Содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="f4216-138">Contains a list of one or more tracking properties.</span></span> <span data-ttu-id="f4216-139">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="f4216-139">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f4216-140">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f4216-140">Parent elements</span></span>

<span data-ttu-id="f4216-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="f4216-141">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f4216-142">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f4216-142">Text value</span></span>

<span data-ttu-id="f4216-143">Нет.</span><span class="sxs-lookup"><span data-stu-id="f4216-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f4216-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="f4216-144">Remarks</span></span>

<span data-ttu-id="f4216-145">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4216-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4216-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f4216-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4216-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f4216-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4216-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f4216-148">Schema Name</span></span>  <br/> |<span data-ttu-id="f4216-149">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f4216-149">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f4216-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f4216-150">Validation File</span></span>  <br/> |<span data-ttu-id="f4216-151">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f4216-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4216-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f4216-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4216-153">False</span><span class="sxs-lookup"><span data-stu-id="f4216-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4216-154">См. также</span><span class="sxs-lookup"><span data-stu-id="f4216-154">See also</span></span>



[<span data-ttu-id="f4216-155">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f4216-155">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="f4216-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f4216-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

