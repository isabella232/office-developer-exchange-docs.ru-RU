---
title: Ошибки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Errors
api_type:
- schema
ms.assetid: ea37a2b5-e2d1-4089-960f-7014b9535a50
description: Элемент ошибки содержит контейнер свойств для хранения ошибки, возвращенные с помощью веб-службы.
ms.openlocfilehash: a029492c1e3c11cc31d3501bd4ea0024ef8ecb91
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762391"
---
# <a name="errors"></a><span data-ttu-id="ff089-103">Ошибки</span><span class="sxs-lookup"><span data-stu-id="ff089-103">Errors</span></span>

<span data-ttu-id="ff089-104">Элемент **ошибки** содержит контейнер свойств для хранения ошибки, возвращенные с помощью веб-службы.</span><span class="sxs-lookup"><span data-stu-id="ff089-104">The **Errors** element contains a property bag to store errors that are returned through the Web service.</span></span> 
  
[<span data-ttu-id="ff089-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="ff089-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
<span data-ttu-id="ff089-106">[сведения об ошибках](errors-ex15websvcsotherref.md);</span><span class="sxs-lookup"><span data-stu-id="ff089-106">[Errors](errors-ex15websvcsotherref.md)</span></span>
  
```xml
<Errors>
   <Properties/>
</Errors>
```

 <span data-ttu-id="ff089-107">**ArrayOfArraysOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="ff089-107">**ArrayOfArraysOfTrackingPropertiesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff089-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ff089-108">Attributes and elements</span></span>

<span data-ttu-id="ff089-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ff089-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff089-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ff089-110">Attributes</span></span>

<span data-ttu-id="ff089-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ff089-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff089-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ff089-112">Child elements</span></span>

|<span data-ttu-id="ff089-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ff089-113">**Element**</span></span>|<span data-ttu-id="ff089-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ff089-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff089-115">Свойства (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="ff089-115">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="ff089-116">Содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="ff089-116">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff089-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ff089-117">Parent elements</span></span>

|<span data-ttu-id="ff089-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ff089-118">**Element**</span></span>|<span data-ttu-id="ff089-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ff089-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff089-120">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="ff089-120">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="ff089-121">Содержит состояние и результат одного запроса [FindMessageTrackingReport операции](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ff089-121">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="ff089-122">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="ff089-122">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="ff089-123">Содержит результат single [GetMessageTrackingReport операции](getmessagetrackingreport-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="ff089-123">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff089-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ff089-124">Text value</span></span>

<span data-ttu-id="ff089-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="ff089-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ff089-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="ff089-126">Remarks</span></span>

<span data-ttu-id="ff089-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ff089-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff089-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ff089-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff089-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ff089-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff089-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ff089-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ff089-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ff089-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff089-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ff089-132">Validation File</span></span>  <br/> |<span data-ttu-id="ff089-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ff089-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff089-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ff089-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff089-135">False</span><span class="sxs-lookup"><span data-stu-id="ff089-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff089-136">См. также</span><span class="sxs-lookup"><span data-stu-id="ff089-136">See also</span></span>



[<span data-ttu-id="ff089-137">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="ff089-137">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
  
[<span data-ttu-id="ff089-138">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="ff089-138">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="ff089-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ff089-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

