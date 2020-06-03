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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462110"
---
# <a name="sendnotificationresponsemessage"></a><span data-ttu-id="3f0f1-103">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3f0f1-103">SendNotificationResponseMessage</span></span>

<span data-ttu-id="3f0f1-104">Элемент **SendNotificationResponseMessage** содержит состояние и результат одного запроса операции **сенднотификатион** .</span><span class="sxs-lookup"><span data-stu-id="3f0f1-104">The **SendNotificationResponseMessage** element contains the status and result of a single **SendNotification** operation request.</span></span> 
  
```xml
<SendNotificationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</SendNotificationResponseMessage>
```

 <span data-ttu-id="3f0f1-105">**сенднотификатионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-105">**SendNotificationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f0f1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3f0f1-106">Attributes and elements</span></span>

<span data-ttu-id="3f0f1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f0f1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3f0f1-108">Attributes</span></span>

|<span data-ttu-id="3f0f1-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-109">**Attribute**</span></span>|<span data-ttu-id="3f0f1-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3f0f1-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="3f0f1-112">Описывает состояние ответа операции **сенднотификатион** .</span><span class="sxs-lookup"><span data-stu-id="3f0f1-112">Describes the status of a **SendNotification** operation response.</span></span> <br/><br/><span data-ttu-id="3f0f1-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="3f0f1-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="3f0f1-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="3f0f1-114">-  Success</span></span>  <br/><span data-ttu-id="3f0f1-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="3f0f1-115">-  Warning</span></span>  <br/><span data-ttu-id="3f0f1-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="3f0f1-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="3f0f1-117">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="3f0f1-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="3f0f1-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-118">**Value**</span></span>|<span data-ttu-id="3f0f1-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3f0f1-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-120">**Success**</span></span> <br/> |<span data-ttu-id="3f0f1-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="3f0f1-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-122">**Warning**</span></span> <br/> | <span data-ttu-id="3f0f1-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-123">Describes a request that was not processed.</span></span> <span data-ttu-id="3f0f1-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="3f0f1-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="3f0f1-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="3f0f1-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="3f0f1-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="3f0f1-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="3f0f1-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="3f0f1-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="3f0f1-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-132">**Error**</span></span> <br/> | <span data-ttu-id="3f0f1-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="3f0f1-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="3f0f1-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="3f0f1-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="3f0f1-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="3f0f1-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="3f0f1-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="3f0f1-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="3f0f1-138">-Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="3f0f1-138">-  Attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="3f0f1-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="3f0f1-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="3f0f1-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="3f0f1-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="3f0f1-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="3f0f1-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3f0f1-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3f0f1-142">Child elements</span></span>

|<span data-ttu-id="3f0f1-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-143">**Element**</span></span>|<span data-ttu-id="3f0f1-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f0f1-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="3f0f1-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3f0f1-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3f0f1-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="3f0f1-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3f0f1-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="3f0f1-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="3f0f1-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3f0f1-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="3f0f1-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="3f0f1-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="3f0f1-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3f0f1-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="3f0f1-154">Уведомление</span><span class="sxs-lookup"><span data-stu-id="3f0f1-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3f0f1-155">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f0f1-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3f0f1-156">Parent elements</span></span>

|<span data-ttu-id="3f0f1-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-157">**Element**</span></span>|<span data-ttu-id="3f0f1-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f0f1-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f0f1-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="3f0f1-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="3f0f1-160">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3f0f1-161">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3f0f1-161">Text value</span></span>

<span data-ttu-id="3f0f1-162">Нет.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3f0f1-163">Примечания</span><span class="sxs-lookup"><span data-stu-id="3f0f1-163">Remarks</span></span>

<span data-ttu-id="3f0f1-164">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f0f1-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f0f1-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3f0f1-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f0f1-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3f0f1-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3f0f1-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3f0f1-167">Schema Name</span></span>  <br/> |<span data-ttu-id="3f0f1-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3f0f1-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3f0f1-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3f0f1-169">Validation File</span></span>  <br/> |<span data-ttu-id="3f0f1-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3f0f1-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3f0f1-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3f0f1-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f0f1-172">False</span><span class="sxs-lookup"><span data-stu-id="3f0f1-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f0f1-173">См. также</span><span class="sxs-lookup"><span data-stu-id="3f0f1-173">See also</span></span>

- [<span data-ttu-id="3f0f1-174">сенднотификатион</span><span class="sxs-lookup"><span data-stu-id="3f0f1-174">SendNotification</span></span>](sendnotification.md)
- [<span data-ttu-id="3f0f1-175">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="3f0f1-175">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="3f0f1-176">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="3f0f1-176">Unsubscribe operation</span></span>](unsubscribe-operation.md)

