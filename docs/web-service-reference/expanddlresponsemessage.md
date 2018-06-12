---
title: ExpandDLResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: Элемент ExpandDLResponseMessage содержит состояние и результат одного запроса операция ExpandDL.
ms.openlocfilehash: 62a81574f9c513b905a92876b3d757c635b4f07b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762438"
---
# <a name="expanddlresponsemessage"></a><span data-ttu-id="71afb-103">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="71afb-103">ExpandDLResponseMessage</span></span>

<span data-ttu-id="71afb-104">Элемент **ExpandDLResponseMessage** содержит состояние и результат одного запроса [ExpandDL операции](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="71afb-104">The **ExpandDLResponseMessage** element contains the status and result of a single [ExpandDL operation](expanddl-operation.md) request.</span></span> 
  
- [<span data-ttu-id="71afb-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="71afb-105">ExpandDLResponse</span></span>](expanddlresponse.md)  
- [<span data-ttu-id="71afb-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="71afb-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="71afb-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="71afb-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

<span data-ttu-id="71afb-108">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="71afb-108">**ExpandDLResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="71afb-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="71afb-109">Attributes and elements</span></span>

<span data-ttu-id="71afb-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="71afb-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71afb-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="71afb-111">Attributes</span></span>

|<span data-ttu-id="71afb-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="71afb-112">**Attribute**</span></span>|<span data-ttu-id="71afb-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71afb-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71afb-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="71afb-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="71afb-115">Описание состояния ответа [ExpandDL операции](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="71afb-115">Describes the status of an [ExpandDL operation](expanddl-operation.md) response.</span></span><br/><br/><span data-ttu-id="71afb-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="71afb-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="71afb-117">-Success</span><span class="sxs-lookup"><span data-stu-id="71afb-117">-  Success</span></span>  <br/><span data-ttu-id="71afb-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="71afb-118">-  Warning</span></span>  <br/><span data-ttu-id="71afb-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="71afb-119">-  Error</span></span>  <br/> |
|<span data-ttu-id="71afb-120">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="71afb-120">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="71afb-121">Представляет следующий индекс, который следует использовать для следующего запроса при использовании индексированного представления разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="71afb-121">Represents the next index that should be used for the next request when an indexed paging view is used.</span></span>  <br/> |
|<span data-ttu-id="71afb-122">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="71afb-122">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="71afb-123">Представляет новое значение перечислителя использовать для следующего запроса при использовании просмотров страниц дроби.</span><span class="sxs-lookup"><span data-stu-id="71afb-123">Represents the new numerator value to use for the next request when fraction page views are used.</span></span>  <br/> |
|<span data-ttu-id="71afb-124">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="71afb-124">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="71afb-125">Представляет Далее делителя для использования в следующем запросе при выполнении дробная разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="71afb-125">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="71afb-126">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="71afb-126">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="71afb-127">Указывает, что дополнительные разбиение на страницы не требуется.</span><span class="sxs-lookup"><span data-stu-id="71afb-127">Indicates that additional paging is not needed.</span></span> <span data-ttu-id="71afb-128">Этот атрибут будет значение true, если текущие результаты содержат последнего элемента в запросе.</span><span class="sxs-lookup"><span data-stu-id="71afb-128">This attribute will be true if the current results contain the last item in the query.</span></span>  <br/> |
|<span data-ttu-id="71afb-129">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="71afb-129">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="71afb-130">Представляет общее число элементов, которые ограничение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="71afb-130">Represents the total number of items that pass the restriction.</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="71afb-131">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="71afb-131">ResponseClass attribute values</span></span>

|<span data-ttu-id="71afb-132">**Значение**</span><span class="sxs-lookup"><span data-stu-id="71afb-132">**Value**</span></span>|<span data-ttu-id="71afb-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71afb-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71afb-134">**Успех**</span><span class="sxs-lookup"><span data-stu-id="71afb-134">**Success**</span></span> <br/> |<span data-ttu-id="71afb-135">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="71afb-135">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="71afb-136">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="71afb-136">**Warning**</span></span> <br/> | <span data-ttu-id="71afb-137">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="71afb-137">Describes a request that was not processed.</span></span> <span data-ttu-id="71afb-138">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="71afb-138">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="71afb-139">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="71afb-139">The following are examples of sources of warnings:</span></span><br/>  <br/><span data-ttu-id="71afb-140">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="71afb-140">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="71afb-141">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="71afb-141">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="71afb-142">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="71afb-142">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="71afb-143">-Базы данных почтовых ящиков (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="71afb-143">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="71afb-144">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="71afb-144">-  A password is expired.</span></span>  <br/><span data-ttu-id="71afb-145">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="71afb-145">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="71afb-146">**Error**</span><span class="sxs-lookup"><span data-stu-id="71afb-146">**Error**</span></span> <br/> | <span data-ttu-id="71afb-147">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="71afb-147">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="71afb-148">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="71afb-148">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="71afb-149">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="71afb-149">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="71afb-150">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="71afb-150">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="71afb-151">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="71afb-151">-  An unknown tag</span></span>  <br/><span data-ttu-id="71afb-152">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="71afb-152">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="71afb-153">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="71afb-153">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="71afb-154">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="71afb-154">-  A server-side failure in response to a valid client-side call</span></span> <br/> <br/>  <span data-ttu-id="71afb-155">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="71afb-155">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="71afb-156">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="71afb-156">Child elements</span></span>

|<span data-ttu-id="71afb-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71afb-157">**Element**</span></span>|<span data-ttu-id="71afb-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71afb-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71afb-159">MessageText</span><span class="sxs-lookup"><span data-stu-id="71afb-159">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="71afb-160">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="71afb-160">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="71afb-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="71afb-161">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="71afb-162">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="71afb-162">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="71afb-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="71afb-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="71afb-164">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="71afb-164">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="71afb-165">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="71afb-165">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="71afb-166">MessageXml</span><span class="sxs-lookup"><span data-stu-id="71afb-166">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="71afb-167">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="71afb-167">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="71afb-168">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="71afb-168">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="71afb-169">Содержит массив почтовых ящиков, которые содержатся в списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="71afb-169">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71afb-170">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="71afb-170">Parent elements</span></span>

|<span data-ttu-id="71afb-171">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71afb-171">**Element**</span></span>|<span data-ttu-id="71afb-172">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71afb-172">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71afb-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="71afb-173">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="71afb-174">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="71afb-174">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="71afb-175">Замечания</span><span class="sxs-lookup"><span data-stu-id="71afb-175">Remarks</span></span>

<span data-ttu-id="71afb-176">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="71afb-176">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71afb-177">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="71afb-177">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71afb-178">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="71afb-178">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71afb-179">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="71afb-179">Schema Name</span></span>  <br/> |<span data-ttu-id="71afb-180">Схема Types</span><span class="sxs-lookup"><span data-stu-id="71afb-180">Types schema</span></span>  <br/> |
|<span data-ttu-id="71afb-181">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="71afb-181">Validation File</span></span>  <br/> |<span data-ttu-id="71afb-182">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71afb-182">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71afb-183">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="71afb-183">Can be Empty</span></span>  <br/> |<span data-ttu-id="71afb-184">False</span><span class="sxs-lookup"><span data-stu-id="71afb-184">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71afb-185">См. также</span><span class="sxs-lookup"><span data-stu-id="71afb-185">See also</span></span>

- [<span data-ttu-id="71afb-186">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="71afb-186">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="71afb-187">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="71afb-187">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="71afb-188">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="71afb-188">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

