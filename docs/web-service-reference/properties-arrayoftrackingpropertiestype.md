---
title: Свойства (Аррайофтраккингпропертиестипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: Элемент Properties содержит список одного или нескольких свойств отслеживания.
ms.openlocfilehash: 007a4dc14c84c47ea7af8ccacc554c134d563e44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465634"
---
# <a name="properties-arrayoftrackingpropertiestype"></a><span data-ttu-id="7dcdb-103">Свойства (Аррайофтраккингпропертиестипе)</span><span class="sxs-lookup"><span data-stu-id="7dcdb-103">Properties (ArrayOfTrackingPropertiesType)</span></span>

<span data-ttu-id="7dcdb-104">Элемент **Properties** содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="7dcdb-104">The **Properties** element contains a list of one or more tracking properties.</span></span> 
  
- [<span data-ttu-id="7dcdb-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7dcdb-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
- [<span data-ttu-id="7dcdb-106">Свойства (Аррайофтраккингпропертиестипе)</span><span class="sxs-lookup"><span data-stu-id="7dcdb-106">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

<span data-ttu-id="7dcdb-107">**аррайофтраккингпропертиестипе**</span><span class="sxs-lookup"><span data-stu-id="7dcdb-107">**ArrayOfTrackingPropertiesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7dcdb-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7dcdb-108">Attributes and elements</span></span>

<span data-ttu-id="7dcdb-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7dcdb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7dcdb-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7dcdb-110">Attributes</span></span>

<span data-ttu-id="7dcdb-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7dcdb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7dcdb-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7dcdb-112">Child elements</span></span>

|<span data-ttu-id="7dcdb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7dcdb-113">**Element**</span></span>|<span data-ttu-id="7dcdb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7dcdb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7dcdb-115">траккингпропертитипе</span><span class="sxs-lookup"><span data-stu-id="7dcdb-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="7dcdb-116">Представляет строку имени и значения, используемую для создания свойств отчетов об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="7dcdb-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7dcdb-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7dcdb-117">Parent elements</span></span>

|<span data-ttu-id="7dcdb-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7dcdb-118">**Element**</span></span>|<span data-ttu-id="7dcdb-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7dcdb-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7dcdb-120">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7dcdb-120">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="7dcdb-121">Задает условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="7dcdb-121">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="7dcdb-122">финдмессажетраккингрепортреспонсе</span><span class="sxs-lookup"><span data-stu-id="7dcdb-122">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="7dcdb-123">Содержит состояние и результат одного запроса [операции FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7dcdb-123">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="7dcdb-124">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7dcdb-124">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="7dcdb-125">Содержит запрос для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="7dcdb-125">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="7dcdb-126">жетмессажетраккингрепортреспонсе</span><span class="sxs-lookup"><span data-stu-id="7dcdb-126">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="7dcdb-127">Содержит результат одного запроса [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7dcdb-127">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="7dcdb-128">реЦипиенттраккинжевент</span><span class="sxs-lookup"><span data-stu-id="7dcdb-128">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="7dcdb-129">Содержит сведения об отдельном событии получателя.</span><span class="sxs-lookup"><span data-stu-id="7dcdb-129">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="7dcdb-130">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7dcdb-130">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="7dcdb-131">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7dcdb-131">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="7dcdb-132">мессажетраккингсеарчресулт</span><span class="sxs-lookup"><span data-stu-id="7dcdb-132">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="7dcdb-133">Содержит один результат одного сообщения для элемента [финдмессажетраккингрепортреспонсе](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="7dcdb-133">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7dcdb-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7dcdb-134">Text value</span></span>

<span data-ttu-id="7dcdb-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="7dcdb-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7dcdb-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="7dcdb-136">Remarks</span></span>

<span data-ttu-id="7dcdb-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7dcdb-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7dcdb-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7dcdb-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7dcdb-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7dcdb-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7dcdb-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7dcdb-140">Schema Name</span></span>  <br/> |<span data-ttu-id="7dcdb-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7dcdb-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7dcdb-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7dcdb-142">Validation File</span></span>  <br/> |<span data-ttu-id="7dcdb-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7dcdb-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7dcdb-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7dcdb-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="7dcdb-145">False</span><span class="sxs-lookup"><span data-stu-id="7dcdb-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7dcdb-146">См. также</span><span class="sxs-lookup"><span data-stu-id="7dcdb-146">See also</span></span>

- [<span data-ttu-id="7dcdb-147">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7dcdb-147">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="7dcdb-148">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7dcdb-148">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="7dcdb-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7dcdb-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

