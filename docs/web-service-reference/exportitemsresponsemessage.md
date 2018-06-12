---
title: ExportItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItemsResponseMessage
api_type:
- schema
ms.assetid: 830fb008-3c45-4988-9041-91a3da3fe689
description: Элемент ExportItemsResponseMessage содержит состояние и результаты запроса на экспорт элемента одного почтового ящика.
ms.openlocfilehash: 99c2ca3f95efff6562ff95350b30fc79c5fb51e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762443"
---
# <a name="exportitemsresponsemessage"></a><span data-ttu-id="366c6-103">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="366c6-103">ExportItemsResponseMessage</span></span>

<span data-ttu-id="366c6-104">Элемент **ExportItemsResponseMessage** содержит состояние и результаты запроса на экспорт элемента одного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="366c6-104">The **ExportItemsResponseMessage** element contains the status and results of a request to export a single mailbox item.</span></span> 
  
- [<span data-ttu-id="366c6-105">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="366c6-105">ExportItemsResponse</span></span>](exportitemsresponse.md)  
- [<span data-ttu-id="366c6-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="366c6-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="366c6-107">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="366c6-107">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
  
```XML
<ExportItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
   <Data/>
</ExportItemsResponseMessage>
```

<span data-ttu-id="366c6-108">**ExportItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="366c6-108">**ExportItemsResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="366c6-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="366c6-109">Attributes and elements</span></span>

<span data-ttu-id="366c6-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="366c6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="366c6-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="366c6-111">Attributes</span></span>

|<span data-ttu-id="366c6-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="366c6-112">**Attribute**</span></span>|<span data-ttu-id="366c6-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="366c6-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="366c6-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="366c6-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="366c6-115">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="366c6-115">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="366c6-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="366c6-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="366c6-117">-Success</span><span class="sxs-lookup"><span data-stu-id="366c6-117">-  Success</span></span>  <br/><span data-ttu-id="366c6-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="366c6-118">-  Warning</span></span>  <br/><span data-ttu-id="366c6-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="366c6-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="366c6-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="366c6-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="366c6-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="366c6-121">**Value**</span></span>|<span data-ttu-id="366c6-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="366c6-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="366c6-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="366c6-123">**Success**</span></span> <br/> |<span data-ttu-id="366c6-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="366c6-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="366c6-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="366c6-125">**Warning**</span></span> <br/> | <span data-ttu-id="366c6-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="366c6-126">Describes a request that was not processed.</span></span> <span data-ttu-id="366c6-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="366c6-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="366c6-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="366c6-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="366c6-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="366c6-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="366c6-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="366c6-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="366c6-131">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="366c6-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="366c6-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="366c6-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="366c6-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="366c6-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="366c6-134">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="366c6-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="366c6-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="366c6-135">**Error**</span></span> <br/> | <span data-ttu-id="366c6-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="366c6-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="366c6-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="366c6-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="366c6-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="366c6-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="366c6-139">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="366c6-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="366c6-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="366c6-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="366c6-141">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="366c6-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="366c6-142">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="366c6-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="366c6-143">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="366c6-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="366c6-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="366c6-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="366c6-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="366c6-145">Child elements</span></span>

|<span data-ttu-id="366c6-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="366c6-146">**Element**</span></span>|<span data-ttu-id="366c6-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="366c6-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="366c6-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="366c6-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="366c6-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="366c6-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="366c6-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="366c6-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="366c6-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="366c6-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="366c6-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="366c6-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="366c6-153">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="366c6-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="366c6-154">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="366c6-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="366c6-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="366c6-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="366c6-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="366c6-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="366c6-157">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="366c6-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="366c6-158">Содержит идентификатор элемента экспортированного элемента.</span><span class="sxs-lookup"><span data-stu-id="366c6-158">Contains the item identifier of an exported item.</span></span>  <br/> |
|[<span data-ttu-id="366c6-159">Данные (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="366c6-159">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="366c6-160">Содержит содержимое экспортируемого объекта.</span><span class="sxs-lookup"><span data-stu-id="366c6-160">Contains the contents of an exported item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="366c6-161">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="366c6-161">Parent elements</span></span>

|<span data-ttu-id="366c6-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="366c6-162">**Element**</span></span>|<span data-ttu-id="366c6-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="366c6-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="366c6-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="366c6-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="366c6-165">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="366c6-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="366c6-166">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="366c6-166">Text value</span></span>

<span data-ttu-id="366c6-167">Нет.</span><span class="sxs-lookup"><span data-stu-id="366c6-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="366c6-168">Замечания</span><span class="sxs-lookup"><span data-stu-id="366c6-168">Remarks</span></span>

<span data-ttu-id="366c6-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="366c6-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="366c6-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="366c6-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="366c6-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="366c6-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="366c6-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="366c6-172">Schema Name</span></span>  <br/> |<span data-ttu-id="366c6-173">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="366c6-173">Message schema</span></span>  <br/> |
|<span data-ttu-id="366c6-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="366c6-174">Validation File</span></span>  <br/> |<span data-ttu-id="366c6-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="366c6-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="366c6-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="366c6-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="366c6-177">False</span><span class="sxs-lookup"><span data-stu-id="366c6-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="366c6-178">См. также</span><span class="sxs-lookup"><span data-stu-id="366c6-178">See also</span></span>

- [<span data-ttu-id="366c6-179">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="366c6-179">ExportItems operation</span></span>](exportitems-operation.md) 
- [<span data-ttu-id="366c6-180">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="366c6-180">UploadItems operation</span></span>](uploaditems-operation.md)

