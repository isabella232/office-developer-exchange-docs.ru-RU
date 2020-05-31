---
title: жетитемреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: Элемент Жетитемреспонсемессаже содержит состояние и результат одного запроса операции GetItem.
ms.openlocfilehash: 0c8527258d4637ede053e189dfb918b910c859d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762842"
---
# <a name="getitemresponsemessage"></a><span data-ttu-id="4e852-103">жетитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="4e852-103">GetItemResponseMessage</span></span>

<span data-ttu-id="4e852-104">Элемент **жетитемреспонсемессаже** содержит состояние и результат одного запроса [операции GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4e852-104">The **GetItemResponseMessage** element contains the status and result of a single [GetItem operation](getitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="4e852-105">жетитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="4e852-105">GetItemResponse</span></span>](getitemresponse.md) 
- [<span data-ttu-id="4e852-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="4e852-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="4e852-107">жетитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="4e852-107">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

<span data-ttu-id="4e852-108">**итеминфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="4e852-108">**ItemInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4e852-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4e852-109">Attributes and elements</span></span>

<span data-ttu-id="4e852-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4e852-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e852-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4e852-111">Attributes</span></span>

|<span data-ttu-id="4e852-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4e852-112">**Attribute**</span></span>|<span data-ttu-id="4e852-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e852-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4e852-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="4e852-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4e852-115">Описывает состояние ответа [операции GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4e852-115">Describes the status of a [GetItem operation](getitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="4e852-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="4e852-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="4e852-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="4e852-117">- Success</span></span><br/><span data-ttu-id="4e852-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="4e852-118">- Warning</span></span><br/><span data-ttu-id="4e852-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="4e852-119">- Error</span></span> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4e852-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="4e852-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="4e852-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4e852-121">**Value**</span></span>|<span data-ttu-id="4e852-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e852-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4e852-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="4e852-123">**Success**</span></span> <br/> |<span data-ttu-id="4e852-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="4e852-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4e852-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="4e852-125">**Warning**</span></span> <br/> | <span data-ttu-id="4e852-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="4e852-126">Describes a request that was not processed.</span></span> <span data-ttu-id="4e852-127">Если при обработке элемента в запросе возникла ошибка, а последующие элементы не были обработаны, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="4e852-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="4e852-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="4e852-128">The following are examples of sources for warnings:</span></span><br/><br/><span data-ttu-id="4e852-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="4e852-129">- The Exchange store is offline during the batch.</span></span><br/><span data-ttu-id="4e852-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4e852-130">- Active Directory Domain Services (AD DS) is offline.</span></span><br/><span data-ttu-id="4e852-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="4e852-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="4e852-132">-MDB находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4e852-132">- MDB is offline.</span></span><br/><span data-ttu-id="4e852-133">-Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="4e852-133">- Password is expired.</span></span>  <br/><span data-ttu-id="4e852-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="4e852-134">- Quota is exceeded.</span></span> |
|<span data-ttu-id="4e852-135">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="4e852-135">**Error**</span></span> <br/> | <span data-ttu-id="4e852-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="4e852-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="4e852-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="4e852-137">The following are examples of sources for errors:</span></span><br/><br/><span data-ttu-id="4e852-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="4e852-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="4e852-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="4e852-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="4e852-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="4e852-140">- Unknown tag</span></span><br/><span data-ttu-id="4e852-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="4e852-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="4e852-142">— Несанкционированный доступ попытался любому клиенту</span><span class="sxs-lookup"><span data-stu-id="4e852-142">- Unauthorized access attempted by any client</span></span><br/><span data-ttu-id="4e852-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="4e852-143">- Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="4e852-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="4e852-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="4e852-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4e852-145">Child elements</span></span>

|<span data-ttu-id="4e852-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4e852-146">**Element**</span></span>|<span data-ttu-id="4e852-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e852-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e852-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="4e852-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4e852-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="4e852-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4e852-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="4e852-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4e852-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="4e852-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4e852-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="4e852-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4e852-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="4e852-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4e852-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="4e852-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4e852-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="4e852-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4e852-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4e852-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4e852-157">Items</span><span class="sxs-lookup"><span data-stu-id="4e852-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="4e852-158">Содержит массив возвращаемых элементов.</span><span class="sxs-lookup"><span data-stu-id="4e852-158">Contains an array of returned items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4e852-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4e852-159">Parent elements</span></span>

|<span data-ttu-id="4e852-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4e852-160">**Element**</span></span>|<span data-ttu-id="4e852-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e852-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e852-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="4e852-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4e852-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e852-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4e852-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="4e852-164">Remarks</span></span>

<span data-ttu-id="4e852-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4e852-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e852-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4e852-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e852-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4e852-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4e852-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4e852-168">Schema Name</span></span>  <br/> |<span data-ttu-id="4e852-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4e852-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4e852-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4e852-170">Validation File</span></span>  <br/> |<span data-ttu-id="4e852-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4e852-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4e852-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4e852-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="4e852-173">False</span><span class="sxs-lookup"><span data-stu-id="4e852-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e852-174">См. также</span><span class="sxs-lookup"><span data-stu-id="4e852-174">See also</span></span>

- [<span data-ttu-id="4e852-175">GetItem</span><span class="sxs-lookup"><span data-stu-id="4e852-175">GetItem</span></span>](getitem.md)
- [<span data-ttu-id="4e852-176">Операция GetItem</span><span class="sxs-lookup"><span data-stu-id="4e852-176">GetItem operation</span></span>](getitem-operation.md)

