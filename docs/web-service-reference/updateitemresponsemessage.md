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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457944"
---
# <a name="updateitemresponsemessage"></a><span data-ttu-id="7179a-103">упдатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="7179a-103">UpdateItemResponseMessage</span></span>

<span data-ttu-id="7179a-104">Элемент **упдатеитемреспонсемессаже** содержит состояние и результат одного запроса [операции UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7179a-104">The **UpdateItemResponseMessage** element contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="7179a-105">упдатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="7179a-105">UpdateItemResponse</span></span>](updateitemresponse.md)
- [<span data-ttu-id="7179a-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="7179a-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="7179a-107">упдатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="7179a-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
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

 <span data-ttu-id="7179a-108">**итеминфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="7179a-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7179a-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7179a-109">Attributes and elements</span></span>

<span data-ttu-id="7179a-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7179a-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7179a-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7179a-111">Attributes</span></span>

|<span data-ttu-id="7179a-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7179a-112">**Attribute**</span></span>|<span data-ttu-id="7179a-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7179a-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7179a-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="7179a-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7179a-115">Описывает состояние ответа [операции UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7179a-115">Describes the status of an [UpdateItem operation](updateitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="7179a-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="7179a-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="7179a-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="7179a-117">-  Success</span></span>  <br/><span data-ttu-id="7179a-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="7179a-118">-  Warning</span></span>  <br/><span data-ttu-id="7179a-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="7179a-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="7179a-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="7179a-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="7179a-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7179a-121">**Value**</span></span>|<span data-ttu-id="7179a-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7179a-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7179a-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="7179a-123">**Success**</span></span> <br/> |<span data-ttu-id="7179a-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="7179a-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7179a-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="7179a-125">**Warning**</span></span> <br/> | <span data-ttu-id="7179a-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="7179a-126">Describes a request that was not processed.</span></span> <span data-ttu-id="7179a-127">Если при обработке элемента в запросе возникла ошибка, а последующие элементы не были обработаны, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="7179a-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="7179a-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="7179a-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="7179a-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="7179a-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="7179a-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="7179a-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="7179a-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="7179a-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="7179a-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="7179a-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="7179a-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="7179a-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="7179a-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="7179a-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="7179a-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="7179a-135">**Error**</span></span> <br/> | <span data-ttu-id="7179a-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="7179a-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="7179a-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="7179a-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="7179a-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="7179a-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7179a-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="7179a-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="7179a-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="7179a-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="7179a-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="7179a-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="7179a-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="7179a-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7179a-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="7179a-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="7179a-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="7179a-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7179a-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7179a-145">Child elements</span></span>

|<span data-ttu-id="7179a-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7179a-146">**Element**</span></span>|<span data-ttu-id="7179a-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7179a-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7179a-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="7179a-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7179a-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="7179a-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7179a-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="7179a-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7179a-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="7179a-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7179a-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="7179a-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7179a-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="7179a-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7179a-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="7179a-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7179a-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="7179a-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7179a-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="7179a-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7179a-157">Items</span><span class="sxs-lookup"><span data-stu-id="7179a-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="7179a-158">Содержит массив обновленных элементов.</span><span class="sxs-lookup"><span data-stu-id="7179a-158">Contains an array of updated items.</span></span>  <br/> |
|[<span data-ttu-id="7179a-159">конфликтресултс</span><span class="sxs-lookup"><span data-stu-id="7179a-159">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="7179a-160">Содержит количество конфликтов в отклике [операции UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7179a-160">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7179a-161">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7179a-161">Parent elements</span></span>

|<span data-ttu-id="7179a-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7179a-162">**Element**</span></span>|<span data-ttu-id="7179a-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7179a-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7179a-164">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="7179a-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7179a-165">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="7179a-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7179a-166">Примечания</span><span class="sxs-lookup"><span data-stu-id="7179a-166">Remarks</span></span>

<span data-ttu-id="7179a-167">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7179a-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7179a-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7179a-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7179a-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7179a-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7179a-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7179a-170">Schema Name</span></span>  <br/> |<span data-ttu-id="7179a-171">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7179a-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7179a-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7179a-172">Validation File</span></span>  <br/> |<span data-ttu-id="7179a-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7179a-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7179a-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7179a-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="7179a-175">False</span><span class="sxs-lookup"><span data-stu-id="7179a-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7179a-176">См. также</span><span class="sxs-lookup"><span data-stu-id="7179a-176">See also</span></span>

- [<span data-ttu-id="7179a-177">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="7179a-177">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="7179a-178">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="7179a-178">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="7179a-179">Обновление задач</span><span class="sxs-lookup"><span data-stu-id="7179a-179">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

