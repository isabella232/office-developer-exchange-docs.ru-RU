---
title: сендитемреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponseMessage
api_type:
- schema
ms.assetid: 264f6a2f-c8cc-4c96-86e1-1aabb6f9d8ab
description: Элемент Сендитемреспонсемессаже содержит состояние и результат одного запроса операции SendItem.
ms.openlocfilehash: 70355aa2b46303bfceafa2cfe89f1c84896f3158
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835344"
---
# <a name="senditemresponsemessage"></a><span data-ttu-id="f5ff1-103">сендитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f5ff1-103">SendItemResponseMessage</span></span>

<span data-ttu-id="f5ff1-104">Элемент **сендитемреспонсемессаже** содержит состояние и результат одного запроса [операции SendItem](senditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f5ff1-104">The **SendItemResponseMessage** element contains the status and result of a single [SendItem operation](senditem-operation.md) request.</span></span> 
  
```xml
<SendItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SendItemResponseMessage>
```

 <span data-ttu-id="f5ff1-105">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5ff1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f5ff1-106">Attributes and elements</span></span>

<span data-ttu-id="f5ff1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5ff1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f5ff1-108">Attributes</span></span>

|<span data-ttu-id="f5ff1-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-109">**Attribute**</span></span>|<span data-ttu-id="f5ff1-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f5ff1-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f5ff1-112">Описывает состояние ответа [операции SendItem](senditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f5ff1-112">Describes the status of a [SendItem operation](senditem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="f5ff1-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="f5ff1-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="f5ff1-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="f5ff1-114">-  Success</span></span>  <br/><span data-ttu-id="f5ff1-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="f5ff1-115">-  Warning</span></span>  <br/><span data-ttu-id="f5ff1-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="f5ff1-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f5ff1-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="f5ff1-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="f5ff1-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-118">**Value**</span></span>|<span data-ttu-id="f5ff1-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f5ff1-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-120">**Success**</span></span> <br/> |<span data-ttu-id="f5ff1-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f5ff1-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-122">**Warning**</span></span> <br/> | <span data-ttu-id="f5ff1-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-123">Describes a request that was not processed.</span></span> <span data-ttu-id="f5ff1-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="f5ff1-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="f5ff1-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f5ff1-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f5ff1-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="f5ff1-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f5ff1-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="f5ff1-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="f5ff1-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-132">**Error**</span></span> <br/> | <span data-ttu-id="f5ff1-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f5ff1-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-134">The following are examples of sources of errors:</span></span>  <br/> <br/><span data-ttu-id="f5ff1-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="f5ff1-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f5ff1-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="f5ff1-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f5ff1-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="f5ff1-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="f5ff1-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="f5ff1-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="f5ff1-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="f5ff1-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f5ff1-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="f5ff1-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="f5ff1-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f5ff1-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f5ff1-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f5ff1-142">Child elements</span></span>

|<span data-ttu-id="f5ff1-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-143">**Element**</span></span>|<span data-ttu-id="f5ff1-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5ff1-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="f5ff1-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f5ff1-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f5ff1-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="f5ff1-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f5ff1-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f5ff1-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="f5ff1-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f5ff1-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="f5ff1-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f5ff1-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="f5ff1-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f5ff1-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5ff1-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f5ff1-154">Parent elements</span></span>

|<span data-ttu-id="f5ff1-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-155">**Element**</span></span>|<span data-ttu-id="f5ff1-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5ff1-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5ff1-157">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f5ff1-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f5ff1-158">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f5ff1-159">Примечания</span><span class="sxs-lookup"><span data-stu-id="f5ff1-159">Remarks</span></span>

<span data-ttu-id="f5ff1-160">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f5ff1-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5ff1-161">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f5ff1-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5ff1-162">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f5ff1-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f5ff1-163">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f5ff1-163">Schema Name</span></span>  <br/> |<span data-ttu-id="f5ff1-164">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f5ff1-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f5ff1-165">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f5ff1-165">Validation File</span></span>  <br/> |<span data-ttu-id="f5ff1-166">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f5ff1-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f5ff1-167">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f5ff1-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="f5ff1-168">False</span><span class="sxs-lookup"><span data-stu-id="f5ff1-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5ff1-169">См. также</span><span class="sxs-lookup"><span data-stu-id="f5ff1-169">See also</span></span>

- [<span data-ttu-id="f5ff1-170">Операция SendItem</span><span class="sxs-lookup"><span data-stu-id="f5ff1-170">SendItem operation</span></span>](senditem-operation.md)
- [<span data-ttu-id="f5ff1-171">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f5ff1-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

