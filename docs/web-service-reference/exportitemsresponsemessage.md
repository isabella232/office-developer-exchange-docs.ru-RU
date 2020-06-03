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
ms.openlocfilehash: 3265836ce6d9d6ef97a4e598bbb3f50e7c5047c6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468948"
---
# <a name="exportitemsresponsemessage"></a><span data-ttu-id="1a439-103">експортитемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="1a439-103">ExportItemsResponseMessage</span></span>

<span data-ttu-id="1a439-104">Элемент **експортитемсреспонсемессаже** содержит состояние и результаты запроса на экспорт одного элемента почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1a439-104">The **ExportItemsResponseMessage** element contains the status and results of a request to export a single mailbox item.</span></span> 
  
- [<span data-ttu-id="1a439-105">експортитемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="1a439-105">ExportItemsResponse</span></span>](exportitemsresponse.md)  
- [<span data-ttu-id="1a439-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="1a439-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="1a439-107">експортитемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="1a439-107">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
  
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

<span data-ttu-id="1a439-108">**експортитемсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="1a439-108">**ExportItemsResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1a439-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1a439-109">Attributes and elements</span></span>

<span data-ttu-id="1a439-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1a439-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a439-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1a439-111">Attributes</span></span>

|<span data-ttu-id="1a439-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="1a439-112">**Attribute**</span></span>|<span data-ttu-id="1a439-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a439-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a439-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="1a439-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1a439-115">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="1a439-115">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="1a439-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="1a439-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="1a439-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="1a439-117">-  Success</span></span>  <br/><span data-ttu-id="1a439-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="1a439-118">-  Warning</span></span>  <br/><span data-ttu-id="1a439-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="1a439-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1a439-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="1a439-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="1a439-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="1a439-121">**Value**</span></span>|<span data-ttu-id="1a439-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a439-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a439-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="1a439-123">**Success**</span></span> <br/> |<span data-ttu-id="1a439-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="1a439-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1a439-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="1a439-125">**Warning**</span></span> <br/> | <span data-ttu-id="1a439-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="1a439-126">Describes a request that was not processed.</span></span> <span data-ttu-id="1a439-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="1a439-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="1a439-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="1a439-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="1a439-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="1a439-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1a439-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="1a439-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="1a439-131">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="1a439-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="1a439-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="1a439-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1a439-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="1a439-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="1a439-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="1a439-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="1a439-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="1a439-135">**Error**</span></span> <br/> | <span data-ttu-id="1a439-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="1a439-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="1a439-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="1a439-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="1a439-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="1a439-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="1a439-139">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="1a439-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="1a439-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="1a439-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="1a439-141">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="1a439-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="1a439-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="1a439-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="1a439-143">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="1a439-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="1a439-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="1a439-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1a439-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1a439-145">Child elements</span></span>

|<span data-ttu-id="1a439-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1a439-146">**Element**</span></span>|<span data-ttu-id="1a439-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a439-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a439-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="1a439-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1a439-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="1a439-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1a439-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="1a439-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1a439-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="1a439-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1a439-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="1a439-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1a439-153">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="1a439-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="1a439-154">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="1a439-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1a439-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="1a439-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1a439-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="1a439-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="1a439-157">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="1a439-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1a439-158">Содержит идентификатор элемента экспортируемого элемента.</span><span class="sxs-lookup"><span data-stu-id="1a439-158">Contains the item identifier of an exported item.</span></span>  <br/> |
|[<span data-ttu-id="1a439-159">Data (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="1a439-159">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="1a439-160">Содержит содержимое экспортированного элемента.</span><span class="sxs-lookup"><span data-stu-id="1a439-160">Contains the contents of an exported item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a439-161">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1a439-161">Parent elements</span></span>

|<span data-ttu-id="1a439-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1a439-162">**Element**</span></span>|<span data-ttu-id="1a439-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a439-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a439-164">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="1a439-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1a439-165">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a439-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a439-166">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1a439-166">Text value</span></span>

<span data-ttu-id="1a439-167">Нет.</span><span class="sxs-lookup"><span data-stu-id="1a439-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1a439-168">Примечания</span><span class="sxs-lookup"><span data-stu-id="1a439-168">Remarks</span></span>

<span data-ttu-id="1a439-169">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1a439-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a439-170">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1a439-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a439-171">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1a439-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1a439-172">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1a439-172">Schema Name</span></span>  <br/> |<span data-ttu-id="1a439-173">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="1a439-173">Message schema</span></span>  <br/> |
|<span data-ttu-id="1a439-174">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1a439-174">Validation File</span></span>  <br/> |<span data-ttu-id="1a439-175">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1a439-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a439-176">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1a439-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a439-177">False</span><span class="sxs-lookup"><span data-stu-id="1a439-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a439-178">См. также</span><span class="sxs-lookup"><span data-stu-id="1a439-178">See also</span></span>

- [<span data-ttu-id="1a439-179">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="1a439-179">ExportItems operation</span></span>](exportitems-operation.md) 
- [<span data-ttu-id="1a439-180">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="1a439-180">UploadItems operation</span></span>](uploaditems-operation.md)

