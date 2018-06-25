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
description: Элемент GetMessageTrackingReport содержит запрос на операцию GetMessageTrackingReport, чтобы получить полный сообщение отслеживания отчетов для указанного идентификатора.
ms.openlocfilehash: cb16f6e9d322cefb0d59c962af8e2f60ebae0e90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762854"
---
# <a name="getmessagetrackingreport"></a><span data-ttu-id="dde94-103">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="dde94-103">GetMessageTrackingReport</span></span>

<span data-ttu-id="dde94-104">Элемент **GetMessageTrackingReport** содержит запроса для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного сообщения, отслеживания отчетов для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="dde94-104">The **GetMessageTrackingReport** element contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span> 
  
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

 <span data-ttu-id="dde94-105">**GetMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="dde94-105">**GetMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dde94-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dde94-106">Attributes and elements</span></span>

<span data-ttu-id="dde94-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dde94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dde94-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dde94-108">Attributes</span></span>

<span data-ttu-id="dde94-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dde94-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dde94-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dde94-110">Child elements</span></span>

|<span data-ttu-id="dde94-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dde94-111">**Element**</span></span>|<span data-ttu-id="dde94-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dde94-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dde94-113">Область (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="dde94-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="dde94-114">Указывает, где выполняется поиск.</span><span class="sxs-lookup"><span data-stu-id="dde94-114">Specifies where to perform the search.</span></span> <span data-ttu-id="dde94-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="dde94-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="dde94-116">Шаблон_отчета</span><span class="sxs-lookup"><span data-stu-id="dde94-116">ReportTemplate</span></span>](reporttemplate.md) <br/> |<span data-ttu-id="dde94-117">Указывает тип отслеживания отчетов для извлечения.</span><span class="sxs-lookup"><span data-stu-id="dde94-117">Specifies the type of tracking report to retrieve.</span></span> <span data-ttu-id="dde94-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="dde94-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="dde94-119">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="dde94-119">RecipientFilter</span></span>](recipientfilter.md) <br/> |<span data-ttu-id="dde94-120">Указывает адрес получателя для использования с отчетом по указанным отслеживания.</span><span class="sxs-lookup"><span data-stu-id="dde94-120">Specifies a recipient address to use with the specified tracking report.</span></span> <span data-ttu-id="dde94-121">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="dde94-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="dde94-122">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="dde94-122">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="dde94-123">Задает строку удостоверение, полученное от **FindMessageTrackingReport** операции.</span><span class="sxs-lookup"><span data-stu-id="dde94-123">Specifies an identity string that was obtained from the **FindMessageTrackingReport** operation.</span></span> <span data-ttu-id="dde94-124">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="dde94-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="dde94-125">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="dde94-125">ReturnQueueEvents</span></span>](returnqueueevents.md) <br/> |<span data-ttu-id="dde94-126">Указывает, что пользователь, выполняющий задачи имеет привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="dde94-126">Specifies that the person who is running the task has a privileged role.</span></span> <span data-ttu-id="dde94-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="dde94-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="dde94-128">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="dde94-128">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="dde94-129">Задает сведения о времени и производительности, который будет использоваться для немедленной отчет об отслеживании.</span><span class="sxs-lookup"><span data-stu-id="dde94-129">Specifies timing and performance information that will be used to derive the tracking report.</span></span> <span data-ttu-id="dde94-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="dde94-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="dde94-131">Свойства (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="dde94-131">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="dde94-132">Задает список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="dde94-132">Specifies a list of one or more tracking properties.</span></span> <span data-ttu-id="dde94-133">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="dde94-133">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dde94-134">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dde94-134">Parent elements</span></span>

<span data-ttu-id="dde94-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="dde94-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dde94-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="dde94-136">Remarks</span></span>

<span data-ttu-id="dde94-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dde94-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dde94-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dde94-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dde94-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dde94-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dde94-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dde94-140">Schema Name</span></span>  <br/> |<span data-ttu-id="dde94-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dde94-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dde94-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dde94-142">Validation File</span></span>  <br/> |<span data-ttu-id="dde94-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dde94-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dde94-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dde94-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="dde94-145">False</span><span class="sxs-lookup"><span data-stu-id="dde94-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dde94-146">См. также</span><span class="sxs-lookup"><span data-stu-id="dde94-146">See also</span></span>



[<span data-ttu-id="dde94-147">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="dde94-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="dde94-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dde94-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

