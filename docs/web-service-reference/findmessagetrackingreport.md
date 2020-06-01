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
description: Элемент FindMessageTrackingReport указывает условия для типов сообщений, которые требуется найти.
ms.openlocfilehash: d30e5391bb4305cae0004a9788df971a57297cae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462938"
---
# <a name="findmessagetrackingreport"></a><span data-ttu-id="7430e-103">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7430e-103">FindMessageTrackingReport</span></span>

<span data-ttu-id="7430e-104">Элемент **FindMessageTrackingReport** указывает условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="7430e-104">The **FindMessageTrackingReport** element specifies criteria for the types of messages to find.</span></span> 
  
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

 <span data-ttu-id="7430e-105">**финдмессажетраккингрепортрекуесттипе**</span><span class="sxs-lookup"><span data-stu-id="7430e-105">**FindMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7430e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7430e-106">Attributes and elements</span></span>

<span data-ttu-id="7430e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7430e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7430e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7430e-108">Attributes</span></span>

<span data-ttu-id="7430e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7430e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7430e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7430e-110">Child elements</span></span>

|<span data-ttu-id="7430e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7430e-111">**Element**</span></span>|<span data-ttu-id="7430e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7430e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7430e-113">Область действия (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="7430e-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="7430e-114">Указывает, насколько обширным должен быть отчет об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="7430e-114">Represents how extensive the message tracking report should be.</span></span>  <br/> |
|[<span data-ttu-id="7430e-115">Domain (отслеживание сообщений)</span><span class="sxs-lookup"><span data-stu-id="7430e-115">Domain (Message Tracking)</span></span>](domain-message-tracking.md) <br/> |<span data-ttu-id="7430e-116">Содержит имя домена, в котором выполняется отслеживание сообщений.</span><span class="sxs-lookup"><span data-stu-id="7430e-116">Contains the name of the domain where the message tracking is executed.</span></span>  <br/> |
|[<span data-ttu-id="7430e-117">Отправитель (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7430e-117">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="7430e-118">Содержит контактные данные отправителя сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7430e-118">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="7430e-119">пурпортедсендер</span><span class="sxs-lookup"><span data-stu-id="7430e-119">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="7430e-120">Содержит контактные данные отправителя предполагаемым сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7430e-120">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="7430e-121">Получатель</span><span class="sxs-lookup"><span data-stu-id="7430e-121">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="7430e-122">Содержит адрес электронной почты получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="7430e-122">Contains the e-mail address for the recipient of the message.</span></span>  <br/> |
|[<span data-ttu-id="7430e-123">Тема</span><span class="sxs-lookup"><span data-stu-id="7430e-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="7430e-124">Содержит тему сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7430e-124">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="7430e-125">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="7430e-125">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="7430e-126">Содержит дату и время начала поиска.</span><span class="sxs-lookup"><span data-stu-id="7430e-126">Contains the starting date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="7430e-127">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="7430e-127">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="7430e-128">Содержит дату и время окончания поиска.</span><span class="sxs-lookup"><span data-stu-id="7430e-128">Contains the ending date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="7430e-129">MessageId</span><span class="sxs-lookup"><span data-stu-id="7430e-129">MessageId</span></span>](messageid.md) <br/> |<span data-ttu-id="7430e-130">Содержит идентификатор сообщения для поиска.</span><span class="sxs-lookup"><span data-stu-id="7430e-130">Contains the message identifier for the search.</span></span>  <br/> |
|[<span data-ttu-id="7430e-131">федератедделиверимаилбокс</span><span class="sxs-lookup"><span data-stu-id="7430e-131">FederatedDeliveryMailbox</span></span>](federateddeliverymailbox.md) <br/> |<span data-ttu-id="7430e-132">Содержит имя почтового ящика, в котором было отправлено сообщение, переданное в другом месте.</span><span class="sxs-lookup"><span data-stu-id="7430e-132">Contains the name of the mailbox where the cross-premise message was sent.</span></span>  <br/> |
|[<span data-ttu-id="7430e-133">диагностикслевел</span><span class="sxs-lookup"><span data-stu-id="7430e-133">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="7430e-134">Представляет уровень детализации для диагностических отчетов.</span><span class="sxs-lookup"><span data-stu-id="7430e-134">Represents the level of detail for diagnostic reports.</span></span>  <br/> |
|[<span data-ttu-id="7430e-135">серверхинт</span><span class="sxs-lookup"><span data-stu-id="7430e-135">ServerHint</span></span>](serverhint.md) <br/> |<span data-ttu-id="7430e-136">Представляет отправную точку для отслеживания сообщения на удаленном сайте или в лесу.</span><span class="sxs-lookup"><span data-stu-id="7430e-136">Represents the starting point for tracking a message in a remote site or forest.</span></span>  <br/> |
|[<span data-ttu-id="7430e-137">Свойства (Аррайофтраккингпропертиестипе)</span><span class="sxs-lookup"><span data-stu-id="7430e-137">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="7430e-138">Содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="7430e-138">Contains a list of one or more tracking properties.</span></span> <span data-ttu-id="7430e-139">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7430e-139">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7430e-140">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7430e-140">Parent elements</span></span>

<span data-ttu-id="7430e-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7430e-141">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7430e-142">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7430e-142">Text value</span></span>

<span data-ttu-id="7430e-143">Нет.</span><span class="sxs-lookup"><span data-stu-id="7430e-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7430e-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="7430e-144">Remarks</span></span>

<span data-ttu-id="7430e-145">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7430e-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7430e-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7430e-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7430e-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7430e-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7430e-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7430e-148">Schema Name</span></span>  <br/> |<span data-ttu-id="7430e-149">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7430e-149">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7430e-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7430e-150">Validation File</span></span>  <br/> |<span data-ttu-id="7430e-151">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7430e-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7430e-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7430e-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="7430e-153">False</span><span class="sxs-lookup"><span data-stu-id="7430e-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7430e-154">См. также</span><span class="sxs-lookup"><span data-stu-id="7430e-154">See also</span></span>



[<span data-ttu-id="7430e-155">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7430e-155">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="7430e-156">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7430e-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

