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
ms.openlocfilehash: a72ae3b20f2cae3d37a90da36b816e6f3265c716
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462917"
---
# <a name="findmessagetrackingreportresponse"></a><span data-ttu-id="7dc57-103">финдмессажетраккингрепортреспонсе</span><span class="sxs-lookup"><span data-stu-id="7dc57-103">FindMessageTrackingReportResponse</span></span>

<span data-ttu-id="7dc57-104">Элемент **финдмессажетраккингрепортреспонсе** содержит состояние и результат одного запроса [операции FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7dc57-104">The **FindMessageTrackingReportResponse** element contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="7dc57-105">**финдмессажетраккингрепортреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="7dc57-105">**FindMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7dc57-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7dc57-106">Attributes and elements</span></span>

<span data-ttu-id="7dc57-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7dc57-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7dc57-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7dc57-108">Attributes</span></span>

|<span data-ttu-id="7dc57-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7dc57-109">**Attribute**</span></span>|<span data-ttu-id="7dc57-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7dc57-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7dc57-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="7dc57-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7dc57-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="7dc57-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="7dc57-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="7dc57-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="7dc57-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="7dc57-114">-  Success</span></span>  <br/><span data-ttu-id="7dc57-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="7dc57-115">-  Warning</span></span>  <br/><span data-ttu-id="7dc57-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="7dc57-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="7dc57-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="7dc57-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="7dc57-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7dc57-118">**Value**</span></span>|<span data-ttu-id="7dc57-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7dc57-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7dc57-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="7dc57-120">**Success**</span></span> <br/> |<span data-ttu-id="7dc57-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="7dc57-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7dc57-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="7dc57-122">**Warning**</span></span> <br/> | <span data-ttu-id="7dc57-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="7dc57-123">Describes a request that was not processed.</span></span> <span data-ttu-id="7dc57-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="7dc57-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="7dc57-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="7dc57-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="7dc57-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="7dc57-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="7dc57-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="7dc57-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="7dc57-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="7dc57-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="7dc57-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="7dc57-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="7dc57-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="7dc57-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="7dc57-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="7dc57-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="7dc57-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="7dc57-132">**Error**</span></span> <br/> | <span data-ttu-id="7dc57-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="7dc57-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="7dc57-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="7dc57-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="7dc57-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="7dc57-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7dc57-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="7dc57-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="7dc57-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="7dc57-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="7dc57-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="7dc57-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="7dc57-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="7dc57-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7dc57-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="7dc57-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="7dc57-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="7dc57-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7dc57-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7dc57-142">Child elements</span></span>

|<span data-ttu-id="7dc57-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7dc57-143">**Element**</span></span>|<span data-ttu-id="7dc57-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7dc57-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7dc57-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="7dc57-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7dc57-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="7dc57-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7dc57-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="7dc57-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7dc57-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="7dc57-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7dc57-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="7dc57-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7dc57-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="7dc57-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="7dc57-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="7dc57-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7dc57-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="7dc57-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7dc57-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="7dc57-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7dc57-154">Диагностики</span><span class="sxs-lookup"><span data-stu-id="7dc57-154">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="7dc57-155">Содержит сведения, которые будут использоваться для создания различных статистических отчетов для функции отслеживания в центре обработки данных.</span><span class="sxs-lookup"><span data-stu-id="7dc57-155">Contains information that will be used to produce various statistical reports for the tracking feature in a DataCenter.</span></span>  <br/> |
|[<span data-ttu-id="7dc57-156">мессажетраккингсеарчресултс</span><span class="sxs-lookup"><span data-stu-id="7dc57-156">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="7dc57-157">Содержит и массив сообщений, которые отвечают требованиям поиска.</span><span class="sxs-lookup"><span data-stu-id="7dc57-157">Contains and array of messages that match the search requirements.</span></span>  <br/> |
|[<span data-ttu-id="7dc57-158">ексекутедсеарчскопе</span><span class="sxs-lookup"><span data-stu-id="7dc57-158">ExecutedSearchScope</span></span>](executedsearchscope.md) <br/> |<span data-ttu-id="7dc57-159">Содержит область поиска, выполненного для получения результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="7dc57-159">Contains the scope of the search that was performed to get the search results.</span></span>  <br/> |
|<span data-ttu-id="7dc57-160">[сведения об ошибках](errors-ex15websvcsotherref.md);</span><span class="sxs-lookup"><span data-stu-id="7dc57-160">[Errors](errors-ex15websvcsotherref.md)</span></span> <br/> |<span data-ttu-id="7dc57-161">Содержит контейнер свойств для хранения ошибок, возвращаемых через веб-службу.</span><span class="sxs-lookup"><span data-stu-id="7dc57-161">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="7dc57-162">Свойства (Аррайофтраккингпропертиестипе)</span><span class="sxs-lookup"><span data-stu-id="7dc57-162">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="7dc57-163">Содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="7dc57-163">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7dc57-164">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7dc57-164">Parent elements</span></span>

<span data-ttu-id="7dc57-165">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7dc57-165">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7dc57-166">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7dc57-166">Text value</span></span>

<span data-ttu-id="7dc57-167">Нет.</span><span class="sxs-lookup"><span data-stu-id="7dc57-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7dc57-168">Примечания</span><span class="sxs-lookup"><span data-stu-id="7dc57-168">Remarks</span></span>

<span data-ttu-id="7dc57-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7dc57-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7dc57-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7dc57-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7dc57-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7dc57-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7dc57-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7dc57-172">Schema Name</span></span>  <br/> |<span data-ttu-id="7dc57-173">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7dc57-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7dc57-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7dc57-174">Validation File</span></span>  <br/> |<span data-ttu-id="7dc57-175">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7dc57-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7dc57-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7dc57-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="7dc57-177">False</span><span class="sxs-lookup"><span data-stu-id="7dc57-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7dc57-178">См. также</span><span class="sxs-lookup"><span data-stu-id="7dc57-178">See also</span></span>

- [<span data-ttu-id="7dc57-179">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7dc57-179">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="7dc57-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7dc57-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

