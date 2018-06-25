---
title: FindMessageTrackingReportResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReportResponse
api_type:
- schema
ms.assetid: ed4265dc-0e79-4b34-8bf4-88a94875629d
description: Элемент FindMessageTrackingReportResponse содержит состояние и результат одного запроса FindMessageTrackingReport операции.
ms.openlocfilehash: fa381f500eac9a46b11aea8c813f1ffc625a3bc3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762588"
---
# <a name="findmessagetrackingreportresponse"></a><span data-ttu-id="3221c-103">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="3221c-103">FindMessageTrackingReportResponse</span></span>

<span data-ttu-id="3221c-104">Элемент **FindMessageTrackingReportResponse** содержит состояние и результат одного запроса [FindMessageTrackingReport операции](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3221c-104">The **FindMessageTrackingReportResponse** element contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span> 
  
```xml
<FindMessageTrackingReportResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Diagnostics/>
   <MessageTrackingSearchResults/>
   <Errors/>
   <Properties/>
</FindMessageTrackingReportResponse>
```

 <span data-ttu-id="3221c-105">**FindMessageTrackingReportResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3221c-105">**FindMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3221c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3221c-106">Attributes and elements</span></span>

<span data-ttu-id="3221c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3221c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3221c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3221c-108">Attributes</span></span>

|<span data-ttu-id="3221c-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="3221c-109">**Attribute**</span></span>|<span data-ttu-id="3221c-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3221c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3221c-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="3221c-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="3221c-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="3221c-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="3221c-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="3221c-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="3221c-114">-Success</span><span class="sxs-lookup"><span data-stu-id="3221c-114">-  Success</span></span>  <br/><span data-ttu-id="3221c-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="3221c-115">-  Warning</span></span>  <br/><span data-ttu-id="3221c-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="3221c-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="3221c-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="3221c-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="3221c-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="3221c-118">**Value**</span></span>|<span data-ttu-id="3221c-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3221c-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3221c-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="3221c-120">**Success**</span></span> <br/> |<span data-ttu-id="3221c-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="3221c-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="3221c-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="3221c-122">**Warning**</span></span> <br/> | <span data-ttu-id="3221c-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="3221c-123">Describes a request that was not processed.</span></span> <span data-ttu-id="3221c-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="3221c-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="3221c-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="3221c-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="3221c-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="3221c-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="3221c-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="3221c-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="3221c-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="3221c-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="3221c-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="3221c-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="3221c-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="3221c-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="3221c-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="3221c-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="3221c-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="3221c-132">**Error**</span></span> <br/> | <span data-ttu-id="3221c-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="3221c-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="3221c-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="3221c-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="3221c-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3221c-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="3221c-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="3221c-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="3221c-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="3221c-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="3221c-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="3221c-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="3221c-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="3221c-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="3221c-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="3221c-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="3221c-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="3221c-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3221c-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3221c-142">Child elements</span></span>

|<span data-ttu-id="3221c-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3221c-143">**Element**</span></span>|<span data-ttu-id="3221c-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3221c-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3221c-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="3221c-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3221c-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="3221c-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3221c-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3221c-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3221c-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="3221c-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="3221c-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3221c-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3221c-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="3221c-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="3221c-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="3221c-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="3221c-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="3221c-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3221c-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="3221c-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="3221c-154">Диагностика (en)</span><span class="sxs-lookup"><span data-stu-id="3221c-154">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="3221c-155">Содержит сведения, которые будут использоваться для создания различные статистические отчеты для отслеживания функции в центре обработки данных.</span><span class="sxs-lookup"><span data-stu-id="3221c-155">Contains information that will be used to produce various statistical reports for the tracking feature in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="3221c-156">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="3221c-156">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="3221c-157">Содержит массива сообщений, которые соответствуют требованиям поиска.</span><span class="sxs-lookup"><span data-stu-id="3221c-157">Contains and array of messages that match the search requirements.</span></span>  <br/> |
|[<span data-ttu-id="3221c-158">ExecutedSearchScope</span><span class="sxs-lookup"><span data-stu-id="3221c-158">ExecutedSearchScope</span></span>](executedsearchscope.md) <br/> |<span data-ttu-id="3221c-159">Содержит область поиска, выполняемого для получения результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="3221c-159">Contains the scope of the search that was performed to get the search results.</span></span>  <br/> |
|<span data-ttu-id="3221c-160">[сведения об ошибках](errors-ex15websvcsotherref.md);</span><span class="sxs-lookup"><span data-stu-id="3221c-160">[Errors](errors-ex15websvcsotherref.md)</span></span> <br/> |<span data-ttu-id="3221c-161">Содержит контейнер свойств для хранения ошибки, возвращенные с помощью веб-службы.</span><span class="sxs-lookup"><span data-stu-id="3221c-161">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="3221c-162">Свойства (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="3221c-162">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="3221c-163">Содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="3221c-163">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3221c-164">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3221c-164">Parent elements</span></span>

<span data-ttu-id="3221c-165">Нет.</span><span class="sxs-lookup"><span data-stu-id="3221c-165">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3221c-166">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3221c-166">Text value</span></span>

<span data-ttu-id="3221c-167">Нет.</span><span class="sxs-lookup"><span data-stu-id="3221c-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3221c-168">Замечания</span><span class="sxs-lookup"><span data-stu-id="3221c-168">Remarks</span></span>

<span data-ttu-id="3221c-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3221c-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3221c-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3221c-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3221c-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3221c-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3221c-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3221c-172">Schema Name</span></span>  <br/> |<span data-ttu-id="3221c-173">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3221c-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3221c-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3221c-174">Validation File</span></span>  <br/> |<span data-ttu-id="3221c-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3221c-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3221c-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3221c-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="3221c-177">False</span><span class="sxs-lookup"><span data-stu-id="3221c-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3221c-178">См. также</span><span class="sxs-lookup"><span data-stu-id="3221c-178">See also</span></span>

- [<span data-ttu-id="3221c-179">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3221c-179">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="3221c-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3221c-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

