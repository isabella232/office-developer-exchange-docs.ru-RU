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
ms.openlocfilehash: bd25a82641259e1546bad6eef5c2f6f8f03e98cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458672"
---
# <a name="getitemresponsemessage"></a><span data-ttu-id="1437d-103">жетитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="1437d-103">GetItemResponseMessage</span></span>

<span data-ttu-id="1437d-104">Элемент **жетитемреспонсемессаже** содержит состояние и результат одного запроса [операции GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1437d-104">The **GetItemResponseMessage** element contains the status and result of a single [GetItem operation](getitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="1437d-105">жетитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="1437d-105">GetItemResponse</span></span>](getitemresponse.md) 
- [<span data-ttu-id="1437d-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="1437d-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="1437d-107">жетитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="1437d-107">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

<span data-ttu-id="1437d-108">**итеминфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="1437d-108">**ItemInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1437d-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1437d-109">Attributes and elements</span></span>

<span data-ttu-id="1437d-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1437d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1437d-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1437d-111">Attributes</span></span>

|<span data-ttu-id="1437d-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="1437d-112">**Attribute**</span></span>|<span data-ttu-id="1437d-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1437d-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1437d-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="1437d-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1437d-115">Описывает состояние ответа [операции GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1437d-115">Describes the status of a [GetItem operation](getitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="1437d-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="1437d-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="1437d-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="1437d-117">- Success</span></span><br/><span data-ttu-id="1437d-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="1437d-118">- Warning</span></span><br/><span data-ttu-id="1437d-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="1437d-119">- Error</span></span> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1437d-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="1437d-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="1437d-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="1437d-121">**Value**</span></span>|<span data-ttu-id="1437d-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1437d-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1437d-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="1437d-123">**Success**</span></span> <br/> |<span data-ttu-id="1437d-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="1437d-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1437d-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="1437d-125">**Warning**</span></span> <br/> | <span data-ttu-id="1437d-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="1437d-126">Describes a request that was not processed.</span></span> <span data-ttu-id="1437d-127">Если при обработке элемента в запросе возникла ошибка, а последующие элементы не были обработаны, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="1437d-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="1437d-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="1437d-128">The following are examples of sources for warnings:</span></span><br/><br/><span data-ttu-id="1437d-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="1437d-129">- The Exchange store is offline during the batch.</span></span><br/><span data-ttu-id="1437d-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="1437d-130">- Active Directory Domain Services (AD DS) is offline.</span></span><br/><span data-ttu-id="1437d-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="1437d-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="1437d-132">-MDB находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="1437d-132">- MDB is offline.</span></span><br/><span data-ttu-id="1437d-133">-Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="1437d-133">- Password is expired.</span></span>  <br/><span data-ttu-id="1437d-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="1437d-134">- Quota is exceeded.</span></span> |
|<span data-ttu-id="1437d-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="1437d-135">**Error**</span></span> <br/> | <span data-ttu-id="1437d-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="1437d-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="1437d-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="1437d-137">The following are examples of sources for errors:</span></span><br/><br/><span data-ttu-id="1437d-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="1437d-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="1437d-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="1437d-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="1437d-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="1437d-140">- Unknown tag</span></span><br/><span data-ttu-id="1437d-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="1437d-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="1437d-142">— Несанкционированный доступ попытался любому клиенту</span><span class="sxs-lookup"><span data-stu-id="1437d-142">- Unauthorized access attempted by any client</span></span><br/><span data-ttu-id="1437d-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="1437d-143">- Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="1437d-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="1437d-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="1437d-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1437d-145">Child elements</span></span>

|<span data-ttu-id="1437d-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1437d-146">**Element**</span></span>|<span data-ttu-id="1437d-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1437d-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1437d-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="1437d-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1437d-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="1437d-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1437d-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="1437d-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1437d-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="1437d-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1437d-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="1437d-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1437d-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="1437d-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="1437d-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="1437d-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1437d-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="1437d-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1437d-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="1437d-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="1437d-157">Items</span><span class="sxs-lookup"><span data-stu-id="1437d-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="1437d-158">Содержит массив возвращаемых элементов.</span><span class="sxs-lookup"><span data-stu-id="1437d-158">Contains an array of returned items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1437d-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1437d-159">Parent elements</span></span>

|<span data-ttu-id="1437d-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1437d-160">**Element**</span></span>|<span data-ttu-id="1437d-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1437d-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1437d-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="1437d-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1437d-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1437d-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1437d-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="1437d-164">Remarks</span></span>

<span data-ttu-id="1437d-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1437d-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1437d-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1437d-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1437d-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1437d-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1437d-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1437d-168">Schema Name</span></span>  <br/> |<span data-ttu-id="1437d-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1437d-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1437d-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1437d-170">Validation File</span></span>  <br/> |<span data-ttu-id="1437d-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1437d-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1437d-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1437d-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="1437d-173">False</span><span class="sxs-lookup"><span data-stu-id="1437d-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1437d-174">См. также</span><span class="sxs-lookup"><span data-stu-id="1437d-174">See also</span></span>

- [<span data-ttu-id="1437d-175">GetItem</span><span class="sxs-lookup"><span data-stu-id="1437d-175">GetItem</span></span>](getitem.md)
- [<span data-ttu-id="1437d-176">Операция GetItem</span><span class="sxs-lookup"><span data-stu-id="1437d-176">GetItem operation</span></span>](getitem-operation.md)

