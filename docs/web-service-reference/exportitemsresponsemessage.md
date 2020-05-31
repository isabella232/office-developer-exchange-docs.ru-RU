---
title: експортитемсреспонсемессаже
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
description: Элемент Експортитемсреспонсемессаже содержит состояние и результаты запроса на экспорт одного элемента почтового ящика.
ms.openlocfilehash: 99c2ca3f95efff6562ff95350b30fc79c5fb51e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762443"
---
# <a name="exportitemsresponsemessage"></a><span data-ttu-id="19634-103">експортитемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="19634-103">ExportItemsResponseMessage</span></span>

<span data-ttu-id="19634-104">Элемент **експортитемсреспонсемессаже** содержит состояние и результаты запроса на экспорт одного элемента почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="19634-104">The **ExportItemsResponseMessage** element contains the status and results of a request to export a single mailbox item.</span></span> 
  
- [<span data-ttu-id="19634-105">експортитемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="19634-105">ExportItemsResponse</span></span>](exportitemsresponse.md)  
- [<span data-ttu-id="19634-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="19634-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="19634-107">експортитемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="19634-107">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
  
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

<span data-ttu-id="19634-108">**експортитемсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="19634-108">**ExportItemsResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="19634-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="19634-109">Attributes and elements</span></span>

<span data-ttu-id="19634-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="19634-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19634-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="19634-111">Attributes</span></span>

|<span data-ttu-id="19634-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="19634-112">**Attribute**</span></span>|<span data-ttu-id="19634-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="19634-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="19634-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="19634-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="19634-115">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="19634-115">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="19634-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="19634-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="19634-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="19634-117">-  Success</span></span>  <br/><span data-ttu-id="19634-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="19634-118">-  Warning</span></span>  <br/><span data-ttu-id="19634-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="19634-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="19634-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="19634-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="19634-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="19634-121">**Value**</span></span>|<span data-ttu-id="19634-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="19634-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="19634-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="19634-123">**Success**</span></span> <br/> |<span data-ttu-id="19634-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="19634-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="19634-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="19634-125">**Warning**</span></span> <br/> | <span data-ttu-id="19634-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="19634-126">Describes a request that was not processed.</span></span> <span data-ttu-id="19634-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="19634-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="19634-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="19634-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="19634-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="19634-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="19634-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="19634-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="19634-131">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="19634-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="19634-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="19634-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="19634-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="19634-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="19634-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="19634-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="19634-135">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="19634-135">**Error**</span></span> <br/> | <span data-ttu-id="19634-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="19634-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="19634-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="19634-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="19634-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="19634-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="19634-139">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="19634-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="19634-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="19634-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="19634-141">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="19634-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="19634-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="19634-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="19634-143">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="19634-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="19634-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="19634-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="19634-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="19634-145">Child elements</span></span>

|<span data-ttu-id="19634-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="19634-146">**Element**</span></span>|<span data-ttu-id="19634-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="19634-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19634-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="19634-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="19634-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="19634-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="19634-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="19634-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="19634-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="19634-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="19634-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="19634-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="19634-153">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="19634-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="19634-154">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="19634-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="19634-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="19634-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="19634-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="19634-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="19634-157">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="19634-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="19634-158">Содержит идентификатор элемента экспортируемого элемента.</span><span class="sxs-lookup"><span data-stu-id="19634-158">Contains the item identifier of an exported item.</span></span>  <br/> |
|[<span data-ttu-id="19634-159">Data (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="19634-159">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="19634-160">Содержит содержимое экспортированного элемента.</span><span class="sxs-lookup"><span data-stu-id="19634-160">Contains the contents of an exported item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="19634-161">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="19634-161">Parent elements</span></span>

|<span data-ttu-id="19634-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="19634-162">**Element**</span></span>|<span data-ttu-id="19634-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="19634-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19634-164">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="19634-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="19634-165">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="19634-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19634-166">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="19634-166">Text value</span></span>

<span data-ttu-id="19634-167">Нет.</span><span class="sxs-lookup"><span data-stu-id="19634-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="19634-168">Примечания</span><span class="sxs-lookup"><span data-stu-id="19634-168">Remarks</span></span>

<span data-ttu-id="19634-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="19634-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19634-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="19634-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19634-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="19634-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="19634-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="19634-172">Schema Name</span></span>  <br/> |<span data-ttu-id="19634-173">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="19634-173">Message schema</span></span>  <br/> |
|<span data-ttu-id="19634-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="19634-174">Validation File</span></span>  <br/> |<span data-ttu-id="19634-175">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="19634-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="19634-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="19634-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="19634-177">False</span><span class="sxs-lookup"><span data-stu-id="19634-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19634-178">См. также</span><span class="sxs-lookup"><span data-stu-id="19634-178">See also</span></span>

- [<span data-ttu-id="19634-179">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="19634-179">ExportItems operation</span></span>](exportitems-operation.md) 
- [<span data-ttu-id="19634-180">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="19634-180">UploadItems operation</span></span>](uploaditems-operation.md)

