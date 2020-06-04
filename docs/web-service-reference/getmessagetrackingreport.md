---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: Элемент GetMessageTrackingReport содержит запрос операции GetMessageTrackingReport, чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.
ms.openlocfilehash: 30596acd209580147e0f03e12a7868502159b29c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466579"
---
# <a name="getmessagetrackingreport"></a><span data-ttu-id="d5118-103">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="d5118-103">GetMessageTrackingReport</span></span>

<span data-ttu-id="d5118-104">Элемент **GetMessageTrackingReport** содержит запрос [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="d5118-104">The **GetMessageTrackingReport** element contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span> 
  
```XML
<GetMessageTrackingReport>
   <Scope/>
   <ReportTemplate/>
   <RecipientFilter/>
   <MessageTrackingReportId/>
   <ReturnQueueEvents/>
   <DiagnosticsLevel/>
   <Properties/>
</GetMessageTrackingReport>
```

 <span data-ttu-id="d5118-105">**жетмессажетраккингрепортрекуесттипе**</span><span class="sxs-lookup"><span data-stu-id="d5118-105">**GetMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5118-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d5118-106">Attributes and elements</span></span>

<span data-ttu-id="d5118-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d5118-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5118-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d5118-108">Attributes</span></span>

<span data-ttu-id="d5118-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d5118-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5118-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d5118-110">Child elements</span></span>

|<span data-ttu-id="d5118-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d5118-111">**Element**</span></span>|<span data-ttu-id="d5118-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d5118-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5118-113">Область действия (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="d5118-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="d5118-114">Указывает, где выполнять поиск.</span><span class="sxs-lookup"><span data-stu-id="d5118-114">Specifies where to perform the search.</span></span> <span data-ttu-id="d5118-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5118-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d5118-116">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="d5118-116">ReportTemplate</span></span>](reporttemplate.md) <br/> |<span data-ttu-id="d5118-117">Указывает тип отчета отслеживания, который требуется получить.</span><span class="sxs-lookup"><span data-stu-id="d5118-117">Specifies the type of tracking report to retrieve.</span></span> <span data-ttu-id="d5118-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5118-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d5118-119">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="d5118-119">RecipientFilter</span></span>](recipientfilter.md) <br/> |<span data-ttu-id="d5118-120">Указывает адрес получателя, который будет использоваться с указанным отчетом об отслеживании.</span><span class="sxs-lookup"><span data-stu-id="d5118-120">Specifies a recipient address to use with the specified tracking report.</span></span> <span data-ttu-id="d5118-121">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d5118-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d5118-122">мессажетраккингрепортид</span><span class="sxs-lookup"><span data-stu-id="d5118-122">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="d5118-123">Задает строку удостоверения, полученную из операции **FindMessageTrackingReport** .</span><span class="sxs-lookup"><span data-stu-id="d5118-123">Specifies an identity string that was obtained from the **FindMessageTrackingReport** operation.</span></span> <span data-ttu-id="d5118-124">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5118-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d5118-125">ретурнкуеуивентс</span><span class="sxs-lookup"><span data-stu-id="d5118-125">ReturnQueueEvents</span></span>](returnqueueevents.md) <br/> |<span data-ttu-id="d5118-126">Указывает, что пользователь, выполняющий задачу, имеет привилегированную роль.</span><span class="sxs-lookup"><span data-stu-id="d5118-126">Specifies that the person who is running the task has a privileged role.</span></span> <span data-ttu-id="d5118-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d5118-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d5118-128">диагностикслевел</span><span class="sxs-lookup"><span data-stu-id="d5118-128">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="d5118-129">Задает сведения о времени и производительности, которые будут использоваться для формирования отчета об отслеживании.</span><span class="sxs-lookup"><span data-stu-id="d5118-129">Specifies timing and performance information that will be used to derive the tracking report.</span></span> <span data-ttu-id="d5118-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d5118-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d5118-131">Свойства (Аррайофтраккингпропертиестипе)</span><span class="sxs-lookup"><span data-stu-id="d5118-131">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="d5118-132">Задает список из одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="d5118-132">Specifies a list of one or more tracking properties.</span></span> <span data-ttu-id="d5118-133">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d5118-133">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5118-134">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d5118-134">Parent elements</span></span>

<span data-ttu-id="d5118-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="d5118-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d5118-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="d5118-136">Remarks</span></span>

<span data-ttu-id="d5118-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5118-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5118-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d5118-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5118-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d5118-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d5118-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d5118-140">Schema Name</span></span>  <br/> |<span data-ttu-id="d5118-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d5118-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d5118-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d5118-142">Validation File</span></span>  <br/> |<span data-ttu-id="d5118-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d5118-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d5118-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d5118-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5118-145">False</span><span class="sxs-lookup"><span data-stu-id="d5118-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5118-146">См. также</span><span class="sxs-lookup"><span data-stu-id="d5118-146">See also</span></span>



[<span data-ttu-id="d5118-147">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="d5118-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="d5118-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d5118-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

