---
title: упдатеитемреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItemResponseMessage
api_type:
- schema
ms.assetid: dc585b05-5afc-4c74-8763-5a54f9a650ec
description: Элемент Упдатеитемреспонсемессаже содержит состояние и результат одного запроса операции UpdateItem.
ms.openlocfilehash: ef25dcf26e06f199587cef885d8cbc9e93b52bdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457944"
---
# <a name="updateitemresponsemessage"></a><span data-ttu-id="db1b1-103">упдатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="db1b1-103">UpdateItemResponseMessage</span></span>

<span data-ttu-id="db1b1-104">Элемент **упдатеитемреспонсемессаже** содержит состояние и результат одного запроса [операции UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="db1b1-104">The **UpdateItemResponseMessage** element contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="db1b1-105">упдатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="db1b1-105">UpdateItemResponse</span></span>](updateitemresponse.md)
- [<span data-ttu-id="db1b1-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="db1b1-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="db1b1-107">упдатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="db1b1-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
```xml
<UpdateItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
   <ConflictResults/>
</UpdateItemResponseMessage>
```

 <span data-ttu-id="db1b1-108">**итеминфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="db1b1-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db1b1-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="db1b1-109">Attributes and elements</span></span>

<span data-ttu-id="db1b1-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="db1b1-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db1b1-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="db1b1-111">Attributes</span></span>

|<span data-ttu-id="db1b1-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="db1b1-112">**Attribute**</span></span>|<span data-ttu-id="db1b1-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db1b1-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="db1b1-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="db1b1-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="db1b1-115">Описывает состояние ответа [операции UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="db1b1-115">Describes the status of an [UpdateItem operation](updateitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="db1b1-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="db1b1-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="db1b1-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="db1b1-117">-  Success</span></span>  <br/><span data-ttu-id="db1b1-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="db1b1-118">-  Warning</span></span>  <br/><span data-ttu-id="db1b1-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="db1b1-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="db1b1-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="db1b1-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="db1b1-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="db1b1-121">**Value**</span></span>|<span data-ttu-id="db1b1-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db1b1-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="db1b1-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="db1b1-123">**Success**</span></span> <br/> |<span data-ttu-id="db1b1-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="db1b1-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="db1b1-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="db1b1-125">**Warning**</span></span> <br/> | <span data-ttu-id="db1b1-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="db1b1-126">Describes a request that was not processed.</span></span> <span data-ttu-id="db1b1-127">Если при обработке элемента в запросе возникла ошибка, а последующие элементы не были обработаны, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="db1b1-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="db1b1-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="db1b1-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="db1b1-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="db1b1-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="db1b1-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="db1b1-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="db1b1-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="db1b1-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="db1b1-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="db1b1-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="db1b1-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="db1b1-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="db1b1-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="db1b1-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="db1b1-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="db1b1-135">**Error**</span></span> <br/> | <span data-ttu-id="db1b1-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="db1b1-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="db1b1-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="db1b1-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="db1b1-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="db1b1-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="db1b1-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="db1b1-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="db1b1-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="db1b1-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="db1b1-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="db1b1-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="db1b1-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="db1b1-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="db1b1-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="db1b1-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="db1b1-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="db1b1-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="db1b1-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="db1b1-145">Child elements</span></span>

|<span data-ttu-id="db1b1-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db1b1-146">**Element**</span></span>|<span data-ttu-id="db1b1-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db1b1-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db1b1-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="db1b1-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="db1b1-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="db1b1-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="db1b1-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="db1b1-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="db1b1-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="db1b1-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="db1b1-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="db1b1-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="db1b1-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="db1b1-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="db1b1-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="db1b1-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="db1b1-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="db1b1-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="db1b1-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="db1b1-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="db1b1-157">Items</span><span class="sxs-lookup"><span data-stu-id="db1b1-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="db1b1-158">Содержит массив обновленных элементов.</span><span class="sxs-lookup"><span data-stu-id="db1b1-158">Contains an array of updated items.</span></span>  <br/> |
|[<span data-ttu-id="db1b1-159">конфликтресултс</span><span class="sxs-lookup"><span data-stu-id="db1b1-159">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="db1b1-160">Содержит количество конфликтов в отклике [операции UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="db1b1-160">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db1b1-161">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="db1b1-161">Parent elements</span></span>

|<span data-ttu-id="db1b1-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db1b1-162">**Element**</span></span>|<span data-ttu-id="db1b1-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db1b1-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db1b1-164">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="db1b1-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="db1b1-165">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="db1b1-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="db1b1-166">Примечания</span><span class="sxs-lookup"><span data-stu-id="db1b1-166">Remarks</span></span>

<span data-ttu-id="db1b1-167">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="db1b1-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db1b1-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="db1b1-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db1b1-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="db1b1-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="db1b1-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="db1b1-170">Schema Name</span></span>  <br/> |<span data-ttu-id="db1b1-171">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="db1b1-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="db1b1-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="db1b1-172">Validation File</span></span>  <br/> |<span data-ttu-id="db1b1-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="db1b1-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db1b1-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="db1b1-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="db1b1-175">False</span><span class="sxs-lookup"><span data-stu-id="db1b1-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db1b1-176">См. также</span><span class="sxs-lookup"><span data-stu-id="db1b1-176">See also</span></span>

- [<span data-ttu-id="db1b1-177">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="db1b1-177">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="db1b1-178">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="db1b1-178">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="db1b1-179">Обновление задач</span><span class="sxs-lookup"><span data-stu-id="db1b1-179">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

