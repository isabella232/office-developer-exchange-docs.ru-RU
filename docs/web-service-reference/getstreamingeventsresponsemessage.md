---
title: жетстреаминжевентсреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEventsResponseMessage
api_type:
- schema
ms.assetid: 655e4e78-af74-48b0-a988-7d86ab368feb
description: Элемент Жетстреаминжевентсреспонсемессаже содержит состояние и результат одного запроса операции GetStreamingEvents.
ms.openlocfilehash: 055fb7eeb12e241739eb860cecbe398b8a322bd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459148"
---
# <a name="getstreamingeventsresponsemessage"></a><span data-ttu-id="25ab1-103">жетстреаминжевентсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="25ab1-103">GetStreamingEventsResponseMessage</span></span>

<span data-ttu-id="25ab1-104">Элемент **жетстреаминжевентсреспонсемессаже** содержит состояние и результат одного запроса [операции GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="25ab1-104">The **GetStreamingEventsResponseMessage** element contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span> 
  
```xml
<GetStreamingEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notifications/>
   <ErrorSubscriptionIds/>
   <ConnectionStatus/>
</GetStreamingEventsResponseMessage>
```

 <span data-ttu-id="25ab1-105">**жетстреаминжевентсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="25ab1-105">**GetStreamingEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25ab1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="25ab1-106">Attributes and elements</span></span>

<span data-ttu-id="25ab1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="25ab1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25ab1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="25ab1-108">Attributes</span></span>

|<span data-ttu-id="25ab1-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="25ab1-109">**Attribute**</span></span>|<span data-ttu-id="25ab1-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25ab1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25ab1-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="25ab1-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="25ab1-112">Описывает состояние ответа [операции GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="25ab1-112">Describes the status of a [GetStreamingEvents operation](getstreamingevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="25ab1-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="25ab1-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="25ab1-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="25ab1-114">-  Success</span></span>  <br/><span data-ttu-id="25ab1-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="25ab1-115">-  Warning</span></span>  <br/><span data-ttu-id="25ab1-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="25ab1-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="25ab1-117">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="25ab1-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="25ab1-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="25ab1-118">**Value**</span></span>|<span data-ttu-id="25ab1-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25ab1-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25ab1-120">Успешно</span><span class="sxs-lookup"><span data-stu-id="25ab1-120">Success</span></span>  <br/> |<span data-ttu-id="25ab1-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="25ab1-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="25ab1-122">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="25ab1-122">Warning</span></span>  <br/> | <span data-ttu-id="25ab1-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="25ab1-123">Describes a request that was not processed.</span></span> <span data-ttu-id="25ab1-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="25ab1-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="25ab1-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="25ab1-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="25ab1-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="25ab1-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="25ab1-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="25ab1-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="25ab1-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="25ab1-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="25ab1-129">— База данных почтовых ящиков (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="25ab1-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="25ab1-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="25ab1-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="25ab1-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="25ab1-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="25ab1-132">Ошибка</span><span class="sxs-lookup"><span data-stu-id="25ab1-132">Error</span></span>  <br/> | <span data-ttu-id="25ab1-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="25ab1-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="25ab1-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="25ab1-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="25ab1-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="25ab1-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="25ab1-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="25ab1-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="25ab1-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="25ab1-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="25ab1-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="25ab1-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="25ab1-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="25ab1-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="25ab1-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="25ab1-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="25ab1-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="25ab1-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="25ab1-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="25ab1-142">Child elements</span></span>

|<span data-ttu-id="25ab1-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25ab1-143">**Element**</span></span>|<span data-ttu-id="25ab1-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25ab1-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25ab1-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="25ab1-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="25ab1-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="25ab1-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="25ab1-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="25ab1-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="25ab1-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="25ab1-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="25ab1-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="25ab1-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="25ab1-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="25ab1-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="25ab1-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="25ab1-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="25ab1-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="25ab1-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="25ab1-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="25ab1-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="25ab1-154">Уведомления</span><span class="sxs-lookup"><span data-stu-id="25ab1-154">Notifications</span></span>](notifications.md) <br/> |<span data-ttu-id="25ab1-155">Содержит список сведений о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="25ab1-155">Contains a list of information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="25ab1-156">еррорсубскриптионидс</span><span class="sxs-lookup"><span data-stu-id="25ab1-156">ErrorSubscriptionIds</span></span>](errorsubscriptionids.md) <br/> |<span data-ttu-id="25ab1-157">Содержит список недопустимых идентификаторов подписки.</span><span class="sxs-lookup"><span data-stu-id="25ab1-157">Contains a list of subscription IDs that are invalid.</span></span>  <br/> |
|[<span data-ttu-id="25ab1-158">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="25ab1-158">ConnectionStatus</span></span>](connectionstatus.md) <br/> |<span data-ttu-id="25ab1-159">Предоставляет текстовое описание состояния попотоковой подписки.</span><span class="sxs-lookup"><span data-stu-id="25ab1-159">Provides a text description of the status of a streaming subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="25ab1-160">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="25ab1-160">Parent elements</span></span>

|<span data-ttu-id="25ab1-161">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25ab1-161">**Element**</span></span>|<span data-ttu-id="25ab1-162">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25ab1-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25ab1-163">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="25ab1-163">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="25ab1-164">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="25ab1-164">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25ab1-165">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="25ab1-165">Text value</span></span>

<span data-ttu-id="25ab1-166">Нет.</span><span class="sxs-lookup"><span data-stu-id="25ab1-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="25ab1-167">Примечания</span><span class="sxs-lookup"><span data-stu-id="25ab1-167">Remarks</span></span>

<span data-ttu-id="25ab1-168">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="25ab1-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25ab1-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="25ab1-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25ab1-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="25ab1-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="25ab1-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="25ab1-171">Schema Name</span></span>  <br/> |<span data-ttu-id="25ab1-172">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="25ab1-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="25ab1-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="25ab1-173">Validation File</span></span>  <br/> |<span data-ttu-id="25ab1-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="25ab1-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="25ab1-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="25ab1-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="25ab1-176">False</span><span class="sxs-lookup"><span data-stu-id="25ab1-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25ab1-177">См. также</span><span class="sxs-lookup"><span data-stu-id="25ab1-177">See also</span></span>

- [<span data-ttu-id="25ab1-178">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="25ab1-178">GetStreamingEvents</span></span>](getstreamingevents.md) 
- [<span data-ttu-id="25ab1-179">жетстреаминжевентсреспонсе</span><span class="sxs-lookup"><span data-stu-id="25ab1-179">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
- [<span data-ttu-id="25ab1-180">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="25ab1-180">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)

