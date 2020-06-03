---
title: мовеитемреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItemResponseMessage
api_type:
- schema
ms.assetid: 1efacb2c-cb76-44ad-b0be-bb47bf2553be
description: Элемент Мовеитемреспонсемессаже содержит состояние и результат одного запроса операции MoveItem.
ms.openlocfilehash: fd96c34840acd5b6137a2a5d50980dc86202629f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530396"
---
# <a name="moveitemresponsemessage"></a><span data-ttu-id="e577b-103">мовеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="e577b-103">MoveItemResponseMessage</span></span>

<span data-ttu-id="e577b-104">Элемент **мовеитемреспонсемессаже** содержит состояние и результат одного запроса [операции MoveItem](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e577b-104">The **MoveItemResponseMessage** element contains the status and result of a single [MoveItem operation](moveitem-operation.md) request.</span></span> 
  
```xml
<MoveItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</MoveItemResponseMessage>
```

 <span data-ttu-id="e577b-105">**итеминфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e577b-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e577b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e577b-106">Attributes and elements</span></span>

<span data-ttu-id="e577b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e577b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e577b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e577b-108">Attributes</span></span>

|<span data-ttu-id="e577b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e577b-109">**Attribute**</span></span>|<span data-ttu-id="e577b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e577b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e577b-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="e577b-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e577b-112">Описывает состояние ответа [операции MoveItem](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e577b-112">Describes the status of a [MoveItem operation](moveitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="e577b-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="e577b-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="e577b-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="e577b-114">-  Success</span></span>  <br/><span data-ttu-id="e577b-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="e577b-115">-  Warning</span></span>  <br/><span data-ttu-id="e577b-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="e577b-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="e577b-117">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="e577b-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="e577b-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e577b-118">**Value**</span></span>|<span data-ttu-id="e577b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e577b-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e577b-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="e577b-120">**Success**</span></span> <br/> |<span data-ttu-id="e577b-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="e577b-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e577b-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="e577b-122">**Warning**</span></span> <br/> | <span data-ttu-id="e577b-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="e577b-123">Describes a request that was not processed.</span></span> <span data-ttu-id="e577b-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="e577b-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="e577b-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="e577b-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="e577b-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="e577b-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="e577b-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="e577b-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="e577b-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="e577b-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="e577b-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="e577b-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="e577b-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="e577b-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="e577b-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="e577b-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="e577b-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="e577b-132">**Error**</span></span> <br/> | <span data-ttu-id="e577b-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="e577b-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e577b-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="e577b-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e577b-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="e577b-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e577b-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="e577b-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="e577b-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="e577b-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="e577b-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="e577b-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="e577b-139">— Любой неавторизованный доступ пытается выполнить любой клиент</span><span class="sxs-lookup"><span data-stu-id="e577b-139">-  Any unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="e577b-140">— Любой сбой на стороне сервера в ответ на действительный вызов на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="e577b-140">-  Any server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="e577b-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e577b-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e577b-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e577b-142">Child elements</span></span>

|<span data-ttu-id="e577b-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e577b-143">**Element**</span></span>|<span data-ttu-id="e577b-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e577b-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e577b-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="e577b-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e577b-146">Текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="e577b-146">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e577b-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="e577b-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e577b-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="e577b-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e577b-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="e577b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e577b-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="e577b-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e577b-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="e577b-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e577b-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="e577b-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e577b-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e577b-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e577b-154">Items</span><span class="sxs-lookup"><span data-stu-id="e577b-154">Items</span></span>](items.md) <br/> |<span data-ttu-id="e577b-155">Содержит массив перемещенных элементов.</span><span class="sxs-lookup"><span data-stu-id="e577b-155">Contains an array of moved items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e577b-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e577b-156">Parent elements</span></span>

|<span data-ttu-id="e577b-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e577b-157">**Element**</span></span>|<span data-ttu-id="e577b-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e577b-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e577b-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="e577b-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e577b-160">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e577b-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e577b-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="e577b-161">Remarks</span></span>

<span data-ttu-id="e577b-162">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e577b-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e577b-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e577b-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e577b-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e577b-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e577b-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e577b-165">Schema Name</span></span>  <br/> |<span data-ttu-id="e577b-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e577b-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e577b-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e577b-167">Validation File</span></span>  <br/> |<span data-ttu-id="e577b-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e577b-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e577b-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e577b-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="e577b-170">False</span><span class="sxs-lookup"><span data-stu-id="e577b-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e577b-171">См. также</span><span class="sxs-lookup"><span data-stu-id="e577b-171">See also</span></span>

- [<span data-ttu-id="e577b-172">Операция MoveItem</span><span class="sxs-lookup"><span data-stu-id="e577b-172">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="e577b-173">MoveItem</span><span class="sxs-lookup"><span data-stu-id="e577b-173">MoveItem</span></span>](moveitem.md)

