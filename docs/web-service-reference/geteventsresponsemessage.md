---
title: GetEventsResponseMessage
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
description: Элемент GetEventsResponseMessage содержит состояние и результат одного запроса GetEvents операции.
ms.openlocfilehash: 90e79194182f61ba7298ef67b1070b1aa239073d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762773"
---
# <a name="geteventsresponsemessage"></a><span data-ttu-id="27337-103">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="27337-103">GetEventsResponseMessage</span></span>

<span data-ttu-id="27337-104">Элемент **GetEventsResponseMessage** содержит состояние и результат одного запроса [GetEvents операции](getevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="27337-104">The **GetEventsResponseMessage** element contains the status and result of a single [GetEvents operation](getevents-operation.md) request.</span></span> 
  
```xml
<GetEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</GetEventsResponseMessage>
```

 <span data-ttu-id="27337-105">**GetEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="27337-105">**GetEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27337-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="27337-106">Attributes and elements</span></span>

<span data-ttu-id="27337-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="27337-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27337-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="27337-108">Attributes</span></span>

|<span data-ttu-id="27337-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="27337-109">**Attribute**</span></span>|<span data-ttu-id="27337-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="27337-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="27337-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="27337-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="27337-112">Описание состояния ответа [GetEvents операции](getevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="27337-112">Describes the status of a [GetEvents operation](getevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="27337-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="27337-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="27337-114">-Success</span><span class="sxs-lookup"><span data-stu-id="27337-114">-  Success</span></span>  <br/><span data-ttu-id="27337-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="27337-115">-  Warning</span></span>  <br/><span data-ttu-id="27337-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="27337-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="27337-117">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="27337-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="27337-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="27337-118">**Value**</span></span>|<span data-ttu-id="27337-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="27337-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="27337-120">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="27337-120">Success</span></span>  <br/> |<span data-ttu-id="27337-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="27337-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="27337-122">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="27337-122">Warning</span></span>  <br/> | <span data-ttu-id="27337-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="27337-123">Describes a request that was not processed.</span></span> <span data-ttu-id="27337-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="27337-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="27337-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="27337-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="27337-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="27337-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="27337-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="27337-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="27337-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="27337-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="27337-129">-Базы данных почтовых ящиков (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="27337-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="27337-130">-Истек срок действия пароль.</span><span class="sxs-lookup"><span data-stu-id="27337-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="27337-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="27337-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="27337-132">Ошибка</span><span class="sxs-lookup"><span data-stu-id="27337-132">Error</span></span>  <br/> | <span data-ttu-id="27337-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="27337-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="27337-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="27337-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="27337-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="27337-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="27337-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="27337-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="27337-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="27337-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="27337-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="27337-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="27337-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="27337-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="27337-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="27337-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="27337-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="27337-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="27337-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="27337-142">Child elements</span></span>

|<span data-ttu-id="27337-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="27337-143">**Element**</span></span>|<span data-ttu-id="27337-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="27337-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27337-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="27337-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="27337-146">Текст с описанием состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="27337-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="27337-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="27337-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="27337-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="27337-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="27337-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="27337-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="27337-150">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="27337-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="27337-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="27337-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="27337-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="27337-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="27337-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="27337-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="27337-154">Уведомление</span><span class="sxs-lookup"><span data-stu-id="27337-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="27337-155">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="27337-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27337-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="27337-156">Parent elements</span></span>

|<span data-ttu-id="27337-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="27337-157">**Element**</span></span>|<span data-ttu-id="27337-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="27337-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27337-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="27337-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="27337-160">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="27337-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="27337-161">Замечания</span><span class="sxs-lookup"><span data-stu-id="27337-161">Remarks</span></span>

<span data-ttu-id="27337-162">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="27337-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27337-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="27337-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27337-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="27337-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27337-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="27337-165">Schema Name</span></span>  <br/> |<span data-ttu-id="27337-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="27337-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="27337-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="27337-167">Validation File</span></span>  <br/> |<span data-ttu-id="27337-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="27337-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27337-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="27337-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="27337-170">False</span><span class="sxs-lookup"><span data-stu-id="27337-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27337-171">См. также</span><span class="sxs-lookup"><span data-stu-id="27337-171">See also</span></span>

- [<span data-ttu-id="27337-172">GetEvents</span><span class="sxs-lookup"><span data-stu-id="27337-172">GetEvents</span></span>](getevents.md) 
- [<span data-ttu-id="27337-173">GetEventsResponse</span><span class="sxs-lookup"><span data-stu-id="27337-173">GetEventsResponse</span></span>](geteventsresponse.md)
- [<span data-ttu-id="27337-174">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="27337-174">GetEvents operation</span></span>](getevents-operation.md)

