---
title: финдмессажетраккингрепортреспонсе
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
description: Элемент Финдмессажетраккингрепортреспонсе содержит состояние и результат одного запроса операции FindMessageTrackingReport.
ms.openlocfilehash: fa381f500eac9a46b11aea8c813f1ffc625a3bc3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762588"
---
# <a name="findmessagetrackingreportresponse"></a><span data-ttu-id="cc4bb-103">финдмессажетраккингрепортреспонсе</span><span class="sxs-lookup"><span data-stu-id="cc4bb-103">FindMessageTrackingReportResponse</span></span>

<span data-ttu-id="cc4bb-104">Элемент **финдмессажетраккингрепортреспонсе** содержит состояние и результат одного запроса [операции FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="cc4bb-104">The **FindMessageTrackingReportResponse** element contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="cc4bb-105">**финдмессажетраккингрепортреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-105">**FindMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc4bb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cc4bb-106">Attributes and elements</span></span>

<span data-ttu-id="cc4bb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc4bb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cc4bb-108">Attributes</span></span>

|<span data-ttu-id="cc4bb-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-109">**Attribute**</span></span>|<span data-ttu-id="cc4bb-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cc4bb-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="cc4bb-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="cc4bb-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="cc4bb-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="cc4bb-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="cc4bb-114">-  Success</span></span>  <br/><span data-ttu-id="cc4bb-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="cc4bb-115">-  Warning</span></span>  <br/><span data-ttu-id="cc4bb-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="cc4bb-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="cc4bb-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="cc4bb-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="cc4bb-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-118">**Value**</span></span>|<span data-ttu-id="cc4bb-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cc4bb-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-120">**Success**</span></span> <br/> |<span data-ttu-id="cc4bb-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="cc4bb-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-122">**Warning**</span></span> <br/> | <span data-ttu-id="cc4bb-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-123">Describes a request that was not processed.</span></span> <span data-ttu-id="cc4bb-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="cc4bb-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="cc4bb-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="cc4bb-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="cc4bb-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="cc4bb-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="cc4bb-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="cc4bb-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="cc4bb-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-132">**Error**</span></span> <br/> | <span data-ttu-id="cc4bb-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="cc4bb-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="cc4bb-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="cc4bb-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="cc4bb-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="cc4bb-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="cc4bb-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="cc4bb-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="cc4bb-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="cc4bb-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="cc4bb-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="cc4bb-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="cc4bb-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="cc4bb-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="cc4bb-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="cc4bb-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cc4bb-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cc4bb-142">Child elements</span></span>

|<span data-ttu-id="cc4bb-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-143">**Element**</span></span>|<span data-ttu-id="cc4bb-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cc4bb-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc4bb-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="cc4bb-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="cc4bb-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="cc4bb-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="cc4bb-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="cc4bb-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="cc4bb-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="cc4bb-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="cc4bb-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="cc4bb-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="cc4bb-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="cc4bb-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="cc4bb-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="cc4bb-154">Диагностики</span><span class="sxs-lookup"><span data-stu-id="cc4bb-154">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="cc4bb-155">Содержит сведения, которые будут использоваться для создания различных статистических отчетов для функции отслеживания в центре обработки данных.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-155">Contains information that will be used to produce various statistical reports for the tracking feature in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="cc4bb-156">мессажетраккингсеарчресултс</span><span class="sxs-lookup"><span data-stu-id="cc4bb-156">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="cc4bb-157">Содержит и массив сообщений, которые отвечают требованиям поиска.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-157">Contains and array of messages that match the search requirements.</span></span>  <br/> |
|[<span data-ttu-id="cc4bb-158">ексекутедсеарчскопе</span><span class="sxs-lookup"><span data-stu-id="cc4bb-158">ExecutedSearchScope</span></span>](executedsearchscope.md) <br/> |<span data-ttu-id="cc4bb-159">Содержит область поиска, выполненного для получения результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-159">Contains the scope of the search that was performed to get the search results.</span></span>  <br/> |
|<span data-ttu-id="cc4bb-160">[сведения об ошибках](errors-ex15websvcsotherref.md);</span><span class="sxs-lookup"><span data-stu-id="cc4bb-160">[Errors](errors-ex15websvcsotherref.md)</span></span> <br/> |<span data-ttu-id="cc4bb-161">Содержит контейнер свойств для хранения ошибок, возвращаемых через веб-службу.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-161">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="cc4bb-162">Свойства (Аррайофтраккингпропертиестипе)</span><span class="sxs-lookup"><span data-stu-id="cc4bb-162">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="cc4bb-163">Содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-163">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc4bb-164">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cc4bb-164">Parent elements</span></span>

<span data-ttu-id="cc4bb-165">Нет.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-165">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="cc4bb-166">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cc4bb-166">Text value</span></span>

<span data-ttu-id="cc4bb-167">Нет.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cc4bb-168">Примечания</span><span class="sxs-lookup"><span data-stu-id="cc4bb-168">Remarks</span></span>

<span data-ttu-id="cc4bb-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc4bb-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc4bb-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cc4bb-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc4bb-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cc4bb-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cc4bb-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cc4bb-172">Schema Name</span></span>  <br/> |<span data-ttu-id="cc4bb-173">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cc4bb-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cc4bb-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cc4bb-174">Validation File</span></span>  <br/> |<span data-ttu-id="cc4bb-175">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cc4bb-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cc4bb-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cc4bb-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc4bb-177">False</span><span class="sxs-lookup"><span data-stu-id="cc4bb-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc4bb-178">См. также</span><span class="sxs-lookup"><span data-stu-id="cc4bb-178">See also</span></span>

- [<span data-ttu-id="cc4bb-179">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="cc4bb-179">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="cc4bb-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cc4bb-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

