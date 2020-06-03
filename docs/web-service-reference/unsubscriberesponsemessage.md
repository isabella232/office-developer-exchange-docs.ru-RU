---
title: унсубскрибереспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnsubscribeResponseMessage
api_type:
- schema
ms.assetid: 92c53b13-0ca1-4b44-b925-b23682e9417c
description: Элемент Унсубскрибереспонсемессаже содержит состояние и результат одного запроса на отмену подписки.
ms.openlocfilehash: e5b42404d09e6367c134934409ec2a45351e135e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467167"
---
# <a name="unsubscriberesponsemessage"></a><span data-ttu-id="3f75e-103">унсубскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="3f75e-103">UnsubscribeResponseMessage</span></span>

<span data-ttu-id="3f75e-104">Элемент **унсубскрибереспонсемессаже** содержит состояние и результат одного запроса на [отмену подписки](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3f75e-104">The **UnsubscribeResponseMessage** element contains the status and result of a single [Unsubscribe operation](unsubscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="3f75e-105">унсубскрибереспонсе</span><span class="sxs-lookup"><span data-stu-id="3f75e-105">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
- [<span data-ttu-id="3f75e-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="3f75e-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="3f75e-107">унсубскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="3f75e-107">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
  
```xml
<UnsubscribeResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UnsubscribeResponseMessage>
```

 <span data-ttu-id="3f75e-108">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="3f75e-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f75e-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3f75e-109">Attributes and elements</span></span>

<span data-ttu-id="3f75e-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3f75e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f75e-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3f75e-111">Attributes</span></span>

|<span data-ttu-id="3f75e-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="3f75e-112">**Attribute**</span></span>|<span data-ttu-id="3f75e-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f75e-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3f75e-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="3f75e-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="3f75e-115">Описывает состояние ответа [на операцию отмены подписки](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="3f75e-115">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="3f75e-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="3f75e-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="3f75e-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="3f75e-117">-  Success</span></span>  <br/><span data-ttu-id="3f75e-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="3f75e-118">-  Warning</span></span>  <br/><span data-ttu-id="3f75e-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="3f75e-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="3f75e-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="3f75e-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="3f75e-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="3f75e-121">**Value**</span></span>|<span data-ttu-id="3f75e-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f75e-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3f75e-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="3f75e-123">**Success**</span></span> <br/> |<span data-ttu-id="3f75e-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="3f75e-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="3f75e-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="3f75e-125">**Warning**</span></span> <br/> | <span data-ttu-id="3f75e-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="3f75e-126">Describes a request that was not processed.</span></span> <span data-ttu-id="3f75e-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="3f75e-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="3f75e-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="3f75e-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="3f75e-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="3f75e-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="3f75e-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="3f75e-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="3f75e-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="3f75e-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="3f75e-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="3f75e-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="3f75e-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="3f75e-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="3f75e-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="3f75e-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="3f75e-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="3f75e-135">**Error**</span></span> <br/> | <span data-ttu-id="3f75e-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="3f75e-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="3f75e-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="3f75e-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="3f75e-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="3f75e-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="3f75e-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="3f75e-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="3f75e-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="3f75e-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="3f75e-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="3f75e-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="3f75e-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="3f75e-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="3f75e-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="3f75e-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="3f75e-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="3f75e-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3f75e-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3f75e-145">Child elements</span></span>

|<span data-ttu-id="3f75e-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3f75e-146">**Element**</span></span>|<span data-ttu-id="3f75e-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f75e-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f75e-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="3f75e-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3f75e-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="3f75e-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3f75e-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="3f75e-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3f75e-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="3f75e-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="3f75e-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="3f75e-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3f75e-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="3f75e-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="3f75e-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="3f75e-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="3f75e-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="3f75e-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3f75e-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="3f75e-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f75e-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3f75e-157">Parent elements</span></span>

|<span data-ttu-id="3f75e-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3f75e-158">**Element**</span></span>|<span data-ttu-id="3f75e-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f75e-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f75e-160">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="3f75e-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="3f75e-161">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f75e-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3f75e-162">Примечания</span><span class="sxs-lookup"><span data-stu-id="3f75e-162">Remarks</span></span>

<span data-ttu-id="3f75e-163">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3f75e-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f75e-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3f75e-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f75e-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3f75e-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3f75e-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3f75e-166">Schema Name</span></span>  <br/> |<span data-ttu-id="3f75e-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3f75e-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3f75e-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3f75e-168">Validation File</span></span>  <br/> |<span data-ttu-id="3f75e-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3f75e-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3f75e-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3f75e-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f75e-171">False</span><span class="sxs-lookup"><span data-stu-id="3f75e-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f75e-172">См. также</span><span class="sxs-lookup"><span data-stu-id="3f75e-172">See also</span></span>

- [<span data-ttu-id="3f75e-173">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="3f75e-173">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="3f75e-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3f75e-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

