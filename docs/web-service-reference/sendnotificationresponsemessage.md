---
title: SendNotificationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotificationResponseMessage
api_type:
- schema
ms.assetid: 2c6d681b-67ac-4331-bc6b-a2e709b638e3
description: Элемент SendNotificationResponseMessage содержит состояние и результат одного запроса операции Сенднотификатион.
ms.openlocfilehash: cf44a09624d1b8a7341f9dd98db48472fea7393b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462110"
---
# <a name="sendnotificationresponsemessage"></a><span data-ttu-id="4ce40-103">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4ce40-103">SendNotificationResponseMessage</span></span>

<span data-ttu-id="4ce40-104">Элемент **SendNotificationResponseMessage** содержит состояние и результат одного запроса операции **сенднотификатион** .</span><span class="sxs-lookup"><span data-stu-id="4ce40-104">The **SendNotificationResponseMessage** element contains the status and result of a single **SendNotification** operation request.</span></span> 
  
```xml
<SendNotificationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</SendNotificationResponseMessage>
```

 <span data-ttu-id="4ce40-105">**сенднотификатионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="4ce40-105">**SendNotificationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ce40-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4ce40-106">Attributes and elements</span></span>

<span data-ttu-id="4ce40-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4ce40-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ce40-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4ce40-108">Attributes</span></span>

|<span data-ttu-id="4ce40-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4ce40-109">**Attribute**</span></span>|<span data-ttu-id="4ce40-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ce40-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4ce40-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="4ce40-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4ce40-112">Описывает состояние ответа операции **сенднотификатион** .</span><span class="sxs-lookup"><span data-stu-id="4ce40-112">Describes the status of a **SendNotification** operation response.</span></span> <br/><br/><span data-ttu-id="4ce40-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="4ce40-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="4ce40-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="4ce40-114">-  Success</span></span>  <br/><span data-ttu-id="4ce40-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="4ce40-115">-  Warning</span></span>  <br/><span data-ttu-id="4ce40-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="4ce40-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="4ce40-117">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="4ce40-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="4ce40-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4ce40-118">**Value**</span></span>|<span data-ttu-id="4ce40-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ce40-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4ce40-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="4ce40-120">**Success**</span></span> <br/> |<span data-ttu-id="4ce40-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="4ce40-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4ce40-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="4ce40-122">**Warning**</span></span> <br/> | <span data-ttu-id="4ce40-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="4ce40-123">Describes a request that was not processed.</span></span> <span data-ttu-id="4ce40-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="4ce40-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="4ce40-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="4ce40-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="4ce40-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="4ce40-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="4ce40-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4ce40-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4ce40-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="4ce40-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="4ce40-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4ce40-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="4ce40-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="4ce40-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="4ce40-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="4ce40-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="4ce40-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="4ce40-132">**Error**</span></span> <br/> | <span data-ttu-id="4ce40-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="4ce40-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4ce40-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="4ce40-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4ce40-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="4ce40-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4ce40-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="4ce40-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="4ce40-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="4ce40-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="4ce40-138">-Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="4ce40-138">-  Attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="4ce40-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="4ce40-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4ce40-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="4ce40-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="4ce40-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="4ce40-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4ce40-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4ce40-142">Child elements</span></span>

|<span data-ttu-id="4ce40-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4ce40-143">**Element**</span></span>|<span data-ttu-id="4ce40-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ce40-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ce40-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="4ce40-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4ce40-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="4ce40-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4ce40-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="4ce40-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4ce40-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="4ce40-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4ce40-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="4ce40-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4ce40-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="4ce40-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4ce40-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="4ce40-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4ce40-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="4ce40-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4ce40-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4ce40-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4ce40-154">Уведомление</span><span class="sxs-lookup"><span data-stu-id="4ce40-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4ce40-155">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="4ce40-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ce40-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4ce40-156">Parent elements</span></span>

|<span data-ttu-id="4ce40-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4ce40-157">**Element**</span></span>|<span data-ttu-id="4ce40-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ce40-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ce40-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="4ce40-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4ce40-160">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ce40-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ce40-161">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4ce40-161">Text value</span></span>

<span data-ttu-id="4ce40-162">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ce40-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ce40-163">Примечания</span><span class="sxs-lookup"><span data-stu-id="4ce40-163">Remarks</span></span>

<span data-ttu-id="4ce40-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ce40-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ce40-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4ce40-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ce40-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4ce40-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ce40-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4ce40-167">Schema Name</span></span>  <br/> |<span data-ttu-id="4ce40-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4ce40-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4ce40-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4ce40-169">Validation File</span></span>  <br/> |<span data-ttu-id="4ce40-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4ce40-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ce40-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4ce40-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ce40-172">False</span><span class="sxs-lookup"><span data-stu-id="4ce40-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ce40-173">См. также</span><span class="sxs-lookup"><span data-stu-id="4ce40-173">See also</span></span>

- [<span data-ttu-id="4ce40-174">сенднотификатион</span><span class="sxs-lookup"><span data-stu-id="4ce40-174">SendNotification</span></span>](sendnotification.md)
- [<span data-ttu-id="4ce40-175">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="4ce40-175">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="4ce40-176">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="4ce40-176">Unsubscribe operation</span></span>](unsubscribe-operation.md)

