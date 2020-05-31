---
title: експанддлреспонсемессаже
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
description: Элемент Експанддлреспонсемессаже содержит состояние и результат одного запроса операции ExpandDL.
ms.openlocfilehash: 62a81574f9c513b905a92876b3d757c635b4f07b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762438"
---
# <a name="expanddlresponsemessage"></a><span data-ttu-id="fd8a8-103">експанддлреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fd8a8-103">ExpandDLResponseMessage</span></span>

<span data-ttu-id="fd8a8-104">Элемент **експанддлреспонсемессаже** содержит состояние и результат одного запроса [операции ExpandDL](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fd8a8-104">The **ExpandDLResponseMessage** element contains the status and result of a single [ExpandDL operation](expanddl-operation.md) request.</span></span> 
  
- [<span data-ttu-id="fd8a8-105">експанддлреспонсе</span><span class="sxs-lookup"><span data-stu-id="fd8a8-105">ExpandDLResponse</span></span>](expanddlresponse.md)  
- [<span data-ttu-id="fd8a8-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fd8a8-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="fd8a8-107">експанддлреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fd8a8-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

<span data-ttu-id="fd8a8-108">**експанддлреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-108">**ExpandDLResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fd8a8-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fd8a8-109">Attributes and elements</span></span>

<span data-ttu-id="fd8a8-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd8a8-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fd8a8-111">Attributes</span></span>

|<span data-ttu-id="fd8a8-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-112">**Attribute**</span></span>|<span data-ttu-id="fd8a8-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fd8a8-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="fd8a8-115">Описывает состояние ответа [операции ExpandDL](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fd8a8-115">Describes the status of an [ExpandDL operation](expanddl-operation.md) response.</span></span><br/><br/><span data-ttu-id="fd8a8-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="fd8a8-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="fd8a8-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="fd8a8-117">-  Success</span></span>  <br/><span data-ttu-id="fd8a8-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="fd8a8-118">-  Warning</span></span>  <br/><span data-ttu-id="fd8a8-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="fd8a8-119">-  Error</span></span>  <br/> |
|<span data-ttu-id="fd8a8-120">**индекседпагингоффсет**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-120">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="fd8a8-121">Представляет следующий индекс, который должен использоваться для следующего запроса при использовании индексированного представления разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-121">Represents the next index that should be used for the next request when an indexed paging view is used.</span></span>  <br/> |
|<span data-ttu-id="fd8a8-122">**нумератороффсет**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-122">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="fd8a8-123">Представляет новое значение числителя, которое будет использоваться для следующего запроса при использовании представлений страницы дробной части.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-123">Represents the new numerator value to use for the next request when fraction page views are used.</span></span>  <br/> |
|<span data-ttu-id="fd8a8-124">**абсолутеденоминатор**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-124">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="fd8a8-125">Представляет следующий знаменатель, который будет использоваться для следующего запроса при выполнении дробного разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-125">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="fd8a8-126">**инклудесластитеминранже**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-126">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="fd8a8-127">Указывает, что дополнительный разбиение по страницам не требуется.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-127">Indicates that additional paging is not needed.</span></span> <span data-ttu-id="fd8a8-128">Этот атрибут будет иметь значение true, если текущие результаты содержат последний элемент в запросе.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-128">This attribute will be true if the current results contain the last item in the query.</span></span>  <br/> |
|<span data-ttu-id="fd8a8-129">**тоталитемсинвиев**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-129">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="fd8a8-130">Представляет общее число элементов, которые прошли ограничение.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-130">Represents the total number of items that pass the restriction.</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="fd8a8-131">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="fd8a8-131">ResponseClass attribute values</span></span>

|<span data-ttu-id="fd8a8-132">**Значение**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-132">**Value**</span></span>|<span data-ttu-id="fd8a8-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fd8a8-134">**Success**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-134">**Success**</span></span> <br/> |<span data-ttu-id="fd8a8-135">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-135">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="fd8a8-136">**Warning**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-136">**Warning**</span></span> <br/> | <span data-ttu-id="fd8a8-137">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-137">Describes a request that was not processed.</span></span> <span data-ttu-id="fd8a8-138">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-138">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="fd8a8-139">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-139">The following are examples of sources of warnings:</span></span><br/>  <br/><span data-ttu-id="fd8a8-140">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-140">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="fd8a8-141">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-141">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="fd8a8-142">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-142">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="fd8a8-143">— База данных почтовых ящиков (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-143">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="fd8a8-144">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-144">-  A password is expired.</span></span>  <br/><span data-ttu-id="fd8a8-145">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-145">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="fd8a8-146">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-146">**Error**</span></span> <br/> | <span data-ttu-id="fd8a8-147">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-147">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="fd8a8-148">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-148">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="fd8a8-149">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="fd8a8-149">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="fd8a8-150">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="fd8a8-150">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="fd8a8-151">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="fd8a8-151">-  An unknown tag</span></span>  <br/><span data-ttu-id="fd8a8-152">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="fd8a8-152">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="fd8a8-153">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="fd8a8-153">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="fd8a8-154">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="fd8a8-154">-  A server-side failure in response to a valid client-side call</span></span> <br/> <br/>  <span data-ttu-id="fd8a8-155">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="fd8a8-155">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fd8a8-156">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fd8a8-156">Child elements</span></span>

|<span data-ttu-id="fd8a8-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-157">**Element**</span></span>|<span data-ttu-id="fd8a8-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd8a8-159">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="fd8a8-159">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="fd8a8-160">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-160">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="fd8a8-161">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fd8a8-161">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="fd8a8-162">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-162">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="fd8a8-163">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="fd8a8-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="fd8a8-164">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-164">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="fd8a8-165">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-165">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="fd8a8-166">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="fd8a8-166">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="fd8a8-167">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-167">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="fd8a8-168">длекспансион</span><span class="sxs-lookup"><span data-stu-id="fd8a8-168">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="fd8a8-169">Содержит массив почтовых ящиков, содержащихся в списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-169">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd8a8-170">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fd8a8-170">Parent elements</span></span>

|<span data-ttu-id="fd8a8-171">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-171">**Element**</span></span>|<span data-ttu-id="fd8a8-172">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd8a8-172">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd8a8-173">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fd8a8-173">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fd8a8-174">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-174">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fd8a8-175">Примечания</span><span class="sxs-lookup"><span data-stu-id="fd8a8-175">Remarks</span></span>

<span data-ttu-id="fd8a8-176">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fd8a8-176">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd8a8-177">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fd8a8-177">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd8a8-178">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fd8a8-178">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd8a8-179">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fd8a8-179">Schema Name</span></span>  <br/> |<span data-ttu-id="fd8a8-180">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fd8a8-180">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd8a8-181">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fd8a8-181">Validation File</span></span>  <br/> |<span data-ttu-id="fd8a8-182">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fd8a8-182">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd8a8-183">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fd8a8-183">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd8a8-184">False</span><span class="sxs-lookup"><span data-stu-id="fd8a8-184">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd8a8-185">См. также</span><span class="sxs-lookup"><span data-stu-id="fd8a8-185">See also</span></span>

- [<span data-ttu-id="fd8a8-186">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="fd8a8-186">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="fd8a8-187">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="fd8a8-187">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="fd8a8-188">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fd8a8-188">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

