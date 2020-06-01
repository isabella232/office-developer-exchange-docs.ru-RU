---
title: упдатеинбоксрулесреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRulesResponse
api_type:
- schema
ms.assetid: 0947b6aa-0d95-421b-aebb-d03021ecc110
description: Элемент Упдатеинбоксрулесреспонсе определяет ответ на запрос UpdateInboxRules.
ms.openlocfilehash: 1216a32bdaf2dd5211021add0728844eb62089ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455907"
---
# <a name="updateinboxrulesresponse"></a><span data-ttu-id="c4e1a-103">упдатеинбоксрулесреспонсе</span><span class="sxs-lookup"><span data-stu-id="c4e1a-103">UpdateInboxRulesResponse</span></span>

<span data-ttu-id="c4e1a-104">Элемент **упдатеинбоксрулесреспонсе** определяет ответ на запрос UpdateInboxRules.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-104">The **UpdateInboxRulesResponse** element defines a response to an UpdateInboxRules request.</span></span> 
  
```XML
<UpdateInboxRulesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RuleOperationErrors/>
</UpdateInboxRulesResponse>
```

 <span data-ttu-id="c4e1a-105">**упдатеинбоксрулесреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-105">**UpdateInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4e1a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c4e1a-106">Attributes and elements</span></span>

<span data-ttu-id="c4e1a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4e1a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c4e1a-108">Attributes</span></span>

|<span data-ttu-id="c4e1a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-109">**Attribute**</span></span>|<span data-ttu-id="c4e1a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c4e1a-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="c4e1a-112">Описывает состояние ответа [на операцию отмены подписки](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c4e1a-112">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span><br/><br/> <span data-ttu-id="c4e1a-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="c4e1a-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="c4e1a-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="c4e1a-114">-  Success</span></span>  <br/><span data-ttu-id="c4e1a-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="c4e1a-115">-  Warning</span></span>  <br/><span data-ttu-id="c4e1a-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="c4e1a-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="c4e1a-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="c4e1a-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="c4e1a-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-118">**Value**</span></span>|<span data-ttu-id="c4e1a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c4e1a-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-120">**Success**</span></span> <br/> |<span data-ttu-id="c4e1a-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="c4e1a-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-122">**Warning**</span></span> <br/> | <span data-ttu-id="c4e1a-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-123">Describes a request that was not processed.</span></span> <span data-ttu-id="c4e1a-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="c4e1a-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="c4e1a-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="c4e1a-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="c4e1a-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="c4e1a-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="c4e1a-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="c4e1a-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="c4e1a-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-132">**Error**</span></span> <br/> | <span data-ttu-id="c4e1a-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="c4e1a-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="c4e1a-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="c4e1a-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="c4e1a-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="c4e1a-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="c4e1a-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="c4e1a-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="c4e1a-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="c4e1a-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="c4e1a-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="c4e1a-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="c4e1a-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="c4e1a-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="c4e1a-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="c4e1a-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c4e1a-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c4e1a-142">Child elements</span></span>

|<span data-ttu-id="c4e1a-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-143">**Element**</span></span>|<span data-ttu-id="c4e1a-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c4e1a-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4e1a-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="c4e1a-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c4e1a-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c4e1a-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="c4e1a-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c4e1a-148">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="c4e1a-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="c4e1a-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c4e1a-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="c4e1a-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c4e1a-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="c4e1a-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c4e1a-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c4e1a-154">рулеоператионеррорс</span><span class="sxs-lookup"><span data-stu-id="c4e1a-154">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="c4e1a-155">Представляет массив ошибок проверки правил для каждого поля правила, в котором возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-155">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c4e1a-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c4e1a-156">Parent elements</span></span>

<span data-ttu-id="c4e1a-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c4e1a-158">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c4e1a-158">Text value</span></span>

<span data-ttu-id="c4e1a-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c4e1a-160">Примечания</span><span class="sxs-lookup"><span data-stu-id="c4e1a-160">Remarks</span></span>

<span data-ttu-id="c4e1a-161">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4e1a-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4e1a-162">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c4e1a-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4e1a-163">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c4e1a-163">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c4e1a-164">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c4e1a-164">Schema name</span></span>  <br/> |<span data-ttu-id="c4e1a-165">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c4e1a-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c4e1a-166">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c4e1a-166">Validation file</span></span>  <br/> |<span data-ttu-id="c4e1a-167">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c4e1a-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c4e1a-168">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c4e1a-168">Can be empty</span></span>  <br/> |<span data-ttu-id="c4e1a-169">False</span><span class="sxs-lookup"><span data-stu-id="c4e1a-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4e1a-170">См. также</span><span class="sxs-lookup"><span data-stu-id="c4e1a-170">See also</span></span>

- [<span data-ttu-id="c4e1a-171">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="c4e1a-171">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="c4e1a-172">Операция UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="c4e1a-172">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="c4e1a-173">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c4e1a-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

