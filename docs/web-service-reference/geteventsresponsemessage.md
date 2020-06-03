---
title: жетевентсреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEventsResponseMessage
api_type:
- schema
ms.assetid: d433977f-b86a-499e-b9c3-f405ac229358
description: Элемент Жетевентсреспонсемессаже содержит состояние и результат выполнения одного запроса операции Events.
ms.openlocfilehash: d307aa1f5234ab5a7a2527c55f5e48814ea2687b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462859"
---
# <a name="geteventsresponsemessage"></a><span data-ttu-id="92d3f-103">жетевентсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="92d3f-103">GetEventsResponseMessage</span></span>

<span data-ttu-id="92d3f-104">Элемент **жетевентсреспонсемессаже** содержит состояние и результат выполнения одного запроса [операции Events](getevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="92d3f-104">The **GetEventsResponseMessage** element contains the status and result of a single [GetEvents operation](getevents-operation.md) request.</span></span> 
  
```xml
<GetEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</GetEventsResponseMessage>
```

 <span data-ttu-id="92d3f-105">**жетевентсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="92d3f-105">**GetEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92d3f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="92d3f-106">Attributes and elements</span></span>

<span data-ttu-id="92d3f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="92d3f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92d3f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="92d3f-108">Attributes</span></span>

|<span data-ttu-id="92d3f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="92d3f-109">**Attribute**</span></span>|<span data-ttu-id="92d3f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="92d3f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="92d3f-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="92d3f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="92d3f-112">Описывает состояние ответа операции с помощью [событий](getevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="92d3f-112">Describes the status of a [GetEvents operation](getevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="92d3f-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="92d3f-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="92d3f-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="92d3f-114">-  Success</span></span>  <br/><span data-ttu-id="92d3f-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="92d3f-115">-  Warning</span></span>  <br/><span data-ttu-id="92d3f-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="92d3f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="92d3f-117">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="92d3f-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="92d3f-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="92d3f-118">**Value**</span></span>|<span data-ttu-id="92d3f-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="92d3f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="92d3f-120">Успешно</span><span class="sxs-lookup"><span data-stu-id="92d3f-120">Success</span></span>  <br/> |<span data-ttu-id="92d3f-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="92d3f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="92d3f-122">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="92d3f-122">Warning</span></span>  <br/> | <span data-ttu-id="92d3f-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="92d3f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="92d3f-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="92d3f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="92d3f-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="92d3f-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="92d3f-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="92d3f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="92d3f-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="92d3f-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="92d3f-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="92d3f-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="92d3f-129">— База данных почтовых ящиков (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="92d3f-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="92d3f-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="92d3f-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="92d3f-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="92d3f-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="92d3f-132">Ошибка</span><span class="sxs-lookup"><span data-stu-id="92d3f-132">Error</span></span>  <br/> | <span data-ttu-id="92d3f-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="92d3f-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="92d3f-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="92d3f-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="92d3f-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="92d3f-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="92d3f-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="92d3f-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="92d3f-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="92d3f-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="92d3f-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="92d3f-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="92d3f-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="92d3f-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="92d3f-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="92d3f-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="92d3f-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="92d3f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="92d3f-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="92d3f-142">Child elements</span></span>

|<span data-ttu-id="92d3f-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="92d3f-143">**Element**</span></span>|<span data-ttu-id="92d3f-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="92d3f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92d3f-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="92d3f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="92d3f-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="92d3f-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="92d3f-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="92d3f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="92d3f-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="92d3f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="92d3f-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="92d3f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="92d3f-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="92d3f-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="92d3f-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="92d3f-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="92d3f-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="92d3f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="92d3f-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="92d3f-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="92d3f-154">Уведомление</span><span class="sxs-lookup"><span data-stu-id="92d3f-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="92d3f-155">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="92d3f-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92d3f-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="92d3f-156">Parent elements</span></span>

|<span data-ttu-id="92d3f-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="92d3f-157">**Element**</span></span>|<span data-ttu-id="92d3f-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="92d3f-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92d3f-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="92d3f-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="92d3f-160">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="92d3f-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="92d3f-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="92d3f-161">Remarks</span></span>

<span data-ttu-id="92d3f-162">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="92d3f-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92d3f-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="92d3f-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92d3f-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="92d3f-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="92d3f-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="92d3f-165">Schema Name</span></span>  <br/> |<span data-ttu-id="92d3f-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="92d3f-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="92d3f-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="92d3f-167">Validation File</span></span>  <br/> |<span data-ttu-id="92d3f-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="92d3f-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="92d3f-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="92d3f-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="92d3f-170">False</span><span class="sxs-lookup"><span data-stu-id="92d3f-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92d3f-171">См. также</span><span class="sxs-lookup"><span data-stu-id="92d3f-171">See also</span></span>

- [<span data-ttu-id="92d3f-172">GetEvents</span><span class="sxs-lookup"><span data-stu-id="92d3f-172">GetEvents</span></span>](getevents.md) 
- [<span data-ttu-id="92d3f-173">жетевентсреспонсе</span><span class="sxs-lookup"><span data-stu-id="92d3f-173">GetEventsResponse</span></span>](geteventsresponse.md)
- [<span data-ttu-id="92d3f-174">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="92d3f-174">GetEvents operation</span></span>](getevents-operation.md)

