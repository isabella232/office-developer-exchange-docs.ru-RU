---
title: MessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReport
api_type:
- schema
ms.assetid: 2740bcf6-f86d-4756-a0f2-24ed6e9b75f7
description: Элемент MessageTrackingReport содержит одно сообщение, которое возвращается в операции GetMessageTrackingReport.
ms.openlocfilehash: fc3e56fbb1bee411fa31751f558f520874133076
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463218"
---
# <a name="messagetrackingreport"></a><span data-ttu-id="963de-103">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="963de-103">MessageTrackingReport</span></span>

<span data-ttu-id="963de-104">Элемент **MessageTrackingReport** содержит одно сообщение, которое возвращается в [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="963de-104">The **MessageTrackingReport** element contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
```XML
<MessageTrackingReport>
   <Sender/>
   <PurportedSender/>
   <Subject/>
   <SubmitTime/>
   <OriginalRecipients/>
   <RecipientTrackingEvents/>
   <Properties/>
</MessageTrackingReport>
```

 <span data-ttu-id="963de-105">**мессажетраккингрепорттипе**</span><span class="sxs-lookup"><span data-stu-id="963de-105">**MessageTrackingReportType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="963de-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="963de-106">Attributes and elements</span></span>

<span data-ttu-id="963de-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="963de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="963de-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="963de-108">Attributes</span></span>

<span data-ttu-id="963de-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="963de-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="963de-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="963de-110">Child elements</span></span>

|<span data-ttu-id="963de-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="963de-111">**Element**</span></span>|<span data-ttu-id="963de-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="963de-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="963de-113">Отправитель (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="963de-113">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="963de-114">Содержит контактные данные отправителя сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="963de-114">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="963de-115">пурпортедсендер</span><span class="sxs-lookup"><span data-stu-id="963de-115">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="963de-116">Содержит контактные данные отправителя предполагаемым сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="963de-116">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="963de-117">Тема</span><span class="sxs-lookup"><span data-stu-id="963de-117">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="963de-118">Содержит тему сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="963de-118">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="963de-119">субмиттиме</span><span class="sxs-lookup"><span data-stu-id="963de-119">SubmitTime</span></span>](submittime.md) <br/> |<span data-ttu-id="963de-120">Содержит время, в течение которого сообщение электронной почты было отправлено.</span><span class="sxs-lookup"><span data-stu-id="963de-120">Contains the time of day that the e-mail message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="963de-121">оригиналреЦипиентс</span><span class="sxs-lookup"><span data-stu-id="963de-121">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="963de-122">Содержит список получателей сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="963de-122">Contains a list of the recipients of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="963de-123">реЦипиенттраккинжевентс</span><span class="sxs-lookup"><span data-stu-id="963de-123">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="963de-124">Содержит список одного или нескольких событий отслеживания для получателей.</span><span class="sxs-lookup"><span data-stu-id="963de-124">Contains a list of one or more tracking events for the recipients.</span></span>  <br/> |
|[<span data-ttu-id="963de-125">Свойства (Аррайофтраккингпропертиестипе)</span><span class="sxs-lookup"><span data-stu-id="963de-125">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="963de-126">Содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="963de-126">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="963de-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="963de-127">Parent elements</span></span>

|<span data-ttu-id="963de-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="963de-128">**Element**</span></span>|<span data-ttu-id="963de-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="963de-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="963de-130">жетмессажетраккингрепортреспонсе</span><span class="sxs-lookup"><span data-stu-id="963de-130">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="963de-131">Содержит результат одного запроса [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="963de-131">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="963de-132">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="963de-132">Text value</span></span>

<span data-ttu-id="963de-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="963de-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="963de-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="963de-134">Remarks</span></span>

<span data-ttu-id="963de-135">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="963de-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="963de-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="963de-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="963de-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="963de-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="963de-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="963de-138">Schema Name</span></span>  <br/> |<span data-ttu-id="963de-139">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="963de-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="963de-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="963de-140">Validation File</span></span>  <br/> |<span data-ttu-id="963de-141">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="963de-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="963de-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="963de-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="963de-143">False</span><span class="sxs-lookup"><span data-stu-id="963de-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="963de-144">См. также</span><span class="sxs-lookup"><span data-stu-id="963de-144">See also</span></span>



[<span data-ttu-id="963de-145">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="963de-145">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
  
[<span data-ttu-id="963de-146">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="963de-146">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="963de-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="963de-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
- [<span data-ttu-id="963de-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="963de-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

