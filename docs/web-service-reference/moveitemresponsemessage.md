---
title: MoveItemResponseMessage
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
description: Элемент MoveItemResponseMessage содержит состояние и результат одного запроса MoveItem операции.
ms.openlocfilehash: af1c10391d9b5b761ab87983eea6321d61231152
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834493"
---
# <a name="moveitemresponsemessage"></a><span data-ttu-id="da59a-103">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="da59a-103">MoveItemResponseMessage</span></span>

<span data-ttu-id="da59a-104">Элемент **MoveItemResponseMessage** содержит состояние и результат одного запроса [MoveItem операции](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="da59a-104">The **MoveItemResponseMessage** element contains the status and result of a single [MoveItem operation](moveitem-operation.md) request.</span></span> 
  
```xml
<MoveItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</MoveItemResponseMessage>
```

 <span data-ttu-id="da59a-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="da59a-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da59a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="da59a-106">Attributes and elements</span></span>

<span data-ttu-id="da59a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="da59a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da59a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="da59a-108">Attributes</span></span>

|<span data-ttu-id="da59a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="da59a-109">**Attribute**</span></span>|<span data-ttu-id="da59a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da59a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="da59a-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="da59a-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="da59a-112">Описание состояния ответа [MoveItem операции](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="da59a-112">Describes the status of a [MoveItem operation](moveitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="da59a-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="da59a-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="da59a-114">-Success</span><span class="sxs-lookup"><span data-stu-id="da59a-114">-  Success</span></span>  <br/><span data-ttu-id="da59a-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="da59a-115">-  Warning</span></span>  <br/><span data-ttu-id="da59a-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="da59a-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="da59a-117">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="da59a-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="da59a-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="da59a-118">**Value**</span></span>|<span data-ttu-id="da59a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da59a-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="da59a-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="da59a-120">**Success**</span></span> <br/> |<span data-ttu-id="da59a-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="da59a-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="da59a-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="da59a-122">**Warning**</span></span> <br/> | <span data-ttu-id="da59a-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="da59a-123">Describes a request that was not processed.</span></span> <span data-ttu-id="da59a-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="da59a-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="da59a-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="da59a-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="da59a-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="da59a-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="da59a-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="da59a-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="da59a-128">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="da59a-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="da59a-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="da59a-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="da59a-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="da59a-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="da59a-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="da59a-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="da59a-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="da59a-132">**Error**</span></span> <br/> | <span data-ttu-id="da59a-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="da59a-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="da59a-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="da59a-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="da59a-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="da59a-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="da59a-136">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="da59a-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="da59a-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="da59a-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="da59a-138">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="da59a-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="da59a-139">-Несанкционированного доступа попытка любой клиент</span><span class="sxs-lookup"><span data-stu-id="da59a-139">-  Any unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="da59a-140">-Любые ошибки на сервере в ответ на допустимый вызовов со стороны клиента.</span><span class="sxs-lookup"><span data-stu-id="da59a-140">-  Any server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="da59a-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="da59a-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="da59a-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="da59a-142">Child elements</span></span>

|<span data-ttu-id="da59a-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da59a-143">**Element**</span></span>|<span data-ttu-id="da59a-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da59a-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da59a-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="da59a-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="da59a-146">Текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="da59a-146">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="da59a-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="da59a-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="da59a-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="da59a-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="da59a-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="da59a-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="da59a-150">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="da59a-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="da59a-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="da59a-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="da59a-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="da59a-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="da59a-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="da59a-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="da59a-154">Элементы</span><span class="sxs-lookup"><span data-stu-id="da59a-154">Items</span></span>](items.md) <br/> |<span data-ttu-id="da59a-155">Содержит массив перемещенной элементов.</span><span class="sxs-lookup"><span data-stu-id="da59a-155">Contains an array of moved items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="da59a-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="da59a-156">Parent elements</span></span>

|<span data-ttu-id="da59a-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da59a-157">**Element**</span></span>|<span data-ttu-id="da59a-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da59a-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da59a-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="da59a-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="da59a-160">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da59a-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="da59a-161">Замечания</span><span class="sxs-lookup"><span data-stu-id="da59a-161">Remarks</span></span>

<span data-ttu-id="da59a-162">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="da59a-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da59a-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="da59a-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da59a-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="da59a-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="da59a-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="da59a-165">Schema Name</span></span>  <br/> |<span data-ttu-id="da59a-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="da59a-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="da59a-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="da59a-167">Validation File</span></span>  <br/> |<span data-ttu-id="da59a-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="da59a-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="da59a-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="da59a-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="da59a-170">False</span><span class="sxs-lookup"><span data-stu-id="da59a-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da59a-171">См. также</span><span class="sxs-lookup"><span data-stu-id="da59a-171">See also</span></span>

- [<span data-ttu-id="da59a-172">MoveItem Operation</span><span class="sxs-lookup"><span data-stu-id="da59a-172">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="da59a-173">MoveItem</span><span class="sxs-lookup"><span data-stu-id="da59a-173">MoveItem</span></span>](moveitem.md)

