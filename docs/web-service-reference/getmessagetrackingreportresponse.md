---
title: GetMessageTrackingReportResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReportResponse
api_type:
- schema
ms.assetid: 41177894-2008-44a6-86f8-bc34c0a48e36
description: Элемент GetMessageTrackingReportResponse содержит ответ на операцию GetMessageTrackingReport.
ms.openlocfilehash: bdb8b97e57f92a32cbdc498d09297920366b58bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762852"
---
# <a name="getmessagetrackingreportresponse"></a><span data-ttu-id="a5dca-103">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="a5dca-103">GetMessageTrackingReportResponse</span></span>

<span data-ttu-id="a5dca-104">Элемент **GetMessageTrackingReportResponse** содержит ответ для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a5dca-104">The **GetMessageTrackingReportResponse** element contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
```xml
<GetMessageTrackingReportResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MessageTrackingReport/>
   <Diagnostics/>
   <Errors/>
   <Properties/>
</GetMessageTrackingReportResponse>
```

 <span data-ttu-id="a5dca-105">**GetMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a5dca-105">**GetMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5dca-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a5dca-106">Attributes and elements</span></span>

<span data-ttu-id="a5dca-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a5dca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5dca-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a5dca-108">Attributes</span></span>

|<span data-ttu-id="a5dca-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a5dca-109">**Attribute**</span></span>|<span data-ttu-id="a5dca-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5dca-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a5dca-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="a5dca-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a5dca-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="a5dca-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="a5dca-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="a5dca-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="a5dca-114">-Success</span><span class="sxs-lookup"><span data-stu-id="a5dca-114">-  Success</span></span>  <br/><span data-ttu-id="a5dca-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="a5dca-115">-  Warning</span></span>  <br/><span data-ttu-id="a5dca-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="a5dca-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a5dca-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a5dca-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="a5dca-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a5dca-118">**Value**</span></span>|<span data-ttu-id="a5dca-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5dca-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a5dca-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="a5dca-120">**Success**</span></span> <br/> |<span data-ttu-id="a5dca-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="a5dca-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a5dca-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="a5dca-122">**Warning**</span></span> <br/> | <span data-ttu-id="a5dca-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="a5dca-123">Describes a request that was not processed.</span></span> <span data-ttu-id="a5dca-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="a5dca-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="a5dca-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="a5dca-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="a5dca-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="a5dca-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="a5dca-127">-Active Directory домена служит (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5dca-127">-  Active Directory Domain Serves (AD DS) is offline.</span></span>  <br/><span data-ttu-id="a5dca-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="a5dca-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="a5dca-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5dca-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="a5dca-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="a5dca-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="a5dca-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="a5dca-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="a5dca-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="a5dca-132">**Error**</span></span> <br/> | <span data-ttu-id="a5dca-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="a5dca-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="a5dca-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="a5dca-134">The following are examples of sources of errors:</span></span>  <br/>  <span data-ttu-id="a5dca-135">Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a5dca-135">Invalid attributes or elements</span></span>  <br/><br/><span data-ttu-id="a5dca-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="a5dca-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="a5dca-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="a5dca-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="a5dca-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="a5dca-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="a5dca-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="a5dca-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a5dca-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="a5dca-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="a5dca-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="a5dca-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a5dca-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a5dca-142">Child elements</span></span>

|<span data-ttu-id="a5dca-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5dca-143">**Element**</span></span>|<span data-ttu-id="a5dca-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5dca-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5dca-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="a5dca-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a5dca-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="a5dca-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a5dca-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a5dca-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a5dca-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="a5dca-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a5dca-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a5dca-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a5dca-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="a5dca-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="a5dca-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="a5dca-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a5dca-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a5dca-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a5dca-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="a5dca-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a5dca-154">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a5dca-154">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="a5dca-155">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a5dca-155">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a5dca-156">Диагностика (en)</span><span class="sxs-lookup"><span data-stu-id="a5dca-156">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="a5dca-157">Предоставляет сведения о времени и производительности, который используется для создания отчетов в центре обработки данных.</span><span class="sxs-lookup"><span data-stu-id="a5dca-157">Provides timing and performance information that is used for reporting in a DataCenter.</span></span>  <br/> |
|<span data-ttu-id="a5dca-158">[сведения об ошибках](errors-ex15websvcsotherref.md);</span><span class="sxs-lookup"><span data-stu-id="a5dca-158">[Errors](errors-ex15websvcsotherref.md)</span></span> <br/> |<span data-ttu-id="a5dca-159">Содержит контейнер свойств для хранения ошибки, возвращенные с помощью веб-службы.</span><span class="sxs-lookup"><span data-stu-id="a5dca-159">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="a5dca-160">Свойства (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="a5dca-160">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="a5dca-161">Содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="a5dca-161">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a5dca-162">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a5dca-162">Parent elements</span></span>

<span data-ttu-id="a5dca-163">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5dca-163">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a5dca-164">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a5dca-164">Text value</span></span>

<span data-ttu-id="a5dca-165">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5dca-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a5dca-166">Замечания</span><span class="sxs-lookup"><span data-stu-id="a5dca-166">Remarks</span></span>

<span data-ttu-id="a5dca-167">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5dca-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5dca-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a5dca-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5dca-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a5dca-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a5dca-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a5dca-170">Schema Name</span></span>  <br/> |<span data-ttu-id="a5dca-171">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a5dca-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a5dca-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a5dca-172">Validation File</span></span>  <br/> |<span data-ttu-id="a5dca-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a5dca-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a5dca-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a5dca-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5dca-175">False</span><span class="sxs-lookup"><span data-stu-id="a5dca-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5dca-176">См. также</span><span class="sxs-lookup"><span data-stu-id="a5dca-176">See also</span></span>

- [<span data-ttu-id="a5dca-177">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a5dca-177">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="a5dca-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a5dca-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

