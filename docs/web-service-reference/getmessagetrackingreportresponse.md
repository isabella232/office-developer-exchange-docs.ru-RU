---
title: жетмессажетраккингрепортреспонсе
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
description: Элемент Жетмессажетраккингрепортреспонсе содержит ответ для операции GetMessageTrackingReport.
ms.openlocfilehash: 15e1f5c91c07dbaad224fb0cd3bc89f444a18087
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460570"
---
# <a name="getmessagetrackingreportresponse"></a><span data-ttu-id="8a79f-103">жетмессажетраккингрепортреспонсе</span><span class="sxs-lookup"><span data-stu-id="8a79f-103">GetMessageTrackingReportResponse</span></span>

<span data-ttu-id="8a79f-104">Элемент **жетмессажетраккингрепортреспонсе** содержит ответ для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8a79f-104">The **GetMessageTrackingReportResponse** element contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
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

 <span data-ttu-id="8a79f-105">**жетмессажетраккингрепортреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8a79f-105">**GetMessageTrackingReportResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a79f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8a79f-106">Attributes and elements</span></span>

<span data-ttu-id="8a79f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8a79f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a79f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8a79f-108">Attributes</span></span>

|<span data-ttu-id="8a79f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8a79f-109">**Attribute**</span></span>|<span data-ttu-id="8a79f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a79f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8a79f-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="8a79f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="8a79f-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="8a79f-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="8a79f-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="8a79f-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="8a79f-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="8a79f-114">-  Success</span></span>  <br/><span data-ttu-id="8a79f-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="8a79f-115">-  Warning</span></span>  <br/><span data-ttu-id="8a79f-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="8a79f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="8a79f-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="8a79f-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="8a79f-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="8a79f-118">**Value**</span></span>|<span data-ttu-id="8a79f-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a79f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8a79f-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="8a79f-120">**Success**</span></span> <br/> |<span data-ttu-id="8a79f-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="8a79f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="8a79f-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="8a79f-122">**Warning**</span></span> <br/> | <span data-ttu-id="8a79f-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="8a79f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="8a79f-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="8a79f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="8a79f-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="8a79f-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="8a79f-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="8a79f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="8a79f-127">-Домен Active Directory обслуживает (AD DS) в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="8a79f-127">-  Active Directory Domain Serves (AD DS) is offline.</span></span>  <br/><span data-ttu-id="8a79f-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="8a79f-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="8a79f-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="8a79f-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="8a79f-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="8a79f-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="8a79f-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="8a79f-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="8a79f-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="8a79f-132">**Error**</span></span> <br/> | <span data-ttu-id="8a79f-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="8a79f-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="8a79f-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="8a79f-134">The following are examples of sources of errors:</span></span>  <br/>  <span data-ttu-id="8a79f-135">Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="8a79f-135">Invalid attributes or elements</span></span>  <br/><br/><span data-ttu-id="8a79f-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="8a79f-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="8a79f-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="8a79f-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="8a79f-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="8a79f-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="8a79f-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="8a79f-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="8a79f-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="8a79f-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="8a79f-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="8a79f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8a79f-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8a79f-142">Child elements</span></span>

|<span data-ttu-id="8a79f-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a79f-143">**Element**</span></span>|<span data-ttu-id="8a79f-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a79f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a79f-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="8a79f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8a79f-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="8a79f-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8a79f-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="8a79f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8a79f-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="8a79f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="8a79f-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="8a79f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8a79f-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="8a79f-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="8a79f-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="8a79f-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="8a79f-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="8a79f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8a79f-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="8a79f-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="8a79f-154">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="8a79f-154">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="8a79f-155">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8a79f-155">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="8a79f-156">Диагностики</span><span class="sxs-lookup"><span data-stu-id="8a79f-156">Diagnostics</span></span>](diagnostics.md) <br/> |<span data-ttu-id="8a79f-157">Предоставляет сведения о времени и производительности, которые используются для отчетов в центре обработки данных.</span><span class="sxs-lookup"><span data-stu-id="8a79f-157">Provides timing and performance information that is used for reporting in a DataCenter.</span></span>  <br/> |
|<span data-ttu-id="8a79f-158">[сведения об ошибках](errors-ex15websvcsotherref.md);</span><span class="sxs-lookup"><span data-stu-id="8a79f-158">[Errors](errors-ex15websvcsotherref.md)</span></span> <br/> |<span data-ttu-id="8a79f-159">Содержит контейнер свойств для хранения ошибок, возвращаемых через веб-службу.</span><span class="sxs-lookup"><span data-stu-id="8a79f-159">Contains a property bag to store errors that are returned through the Web service.</span></span>  <br/> |
|[<span data-ttu-id="8a79f-160">Свойства (Аррайофтраккингпропертиестипе)</span><span class="sxs-lookup"><span data-stu-id="8a79f-160">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="8a79f-161">Содержит список одного или нескольких свойств отслеживания.</span><span class="sxs-lookup"><span data-stu-id="8a79f-161">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a79f-162">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8a79f-162">Parent elements</span></span>

<span data-ttu-id="8a79f-163">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8a79f-163">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="8a79f-164">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8a79f-164">Text value</span></span>

<span data-ttu-id="8a79f-165">Нет.</span><span class="sxs-lookup"><span data-stu-id="8a79f-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8a79f-166">Примечания</span><span class="sxs-lookup"><span data-stu-id="8a79f-166">Remarks</span></span>

<span data-ttu-id="8a79f-167">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a79f-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a79f-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8a79f-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a79f-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8a79f-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8a79f-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8a79f-170">Schema Name</span></span>  <br/> |<span data-ttu-id="8a79f-171">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8a79f-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8a79f-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8a79f-172">Validation File</span></span>  <br/> |<span data-ttu-id="8a79f-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8a79f-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8a79f-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8a79f-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a79f-175">False</span><span class="sxs-lookup"><span data-stu-id="8a79f-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a79f-176">См. также</span><span class="sxs-lookup"><span data-stu-id="8a79f-176">See also</span></span>

- [<span data-ttu-id="8a79f-177">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="8a79f-177">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="8a79f-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a79f-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

