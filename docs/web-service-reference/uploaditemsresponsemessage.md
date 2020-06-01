---
title: уплоадитемсреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItemsResponseMessage
api_type:
- schema
ms.assetid: 03febd08-c015-4009-b291-1b4296182ffe
description: Элемент Уплоадитемсреспонсемессаже содержит состояние и результаты запроса на отправку одного элемента почтового ящика.
ms.openlocfilehash: 4049772c560f3d54a31351fe1fbed77fe5780bf8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468497"
---
# <a name="uploaditemsresponsemessage"></a><span data-ttu-id="b45c6-103">уплоадитемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="b45c6-103">UploadItemsResponseMessage</span></span>

<span data-ttu-id="b45c6-104">Элемент **уплоадитемсреспонсемессаже** содержит состояние и результаты запроса на отправку одного элемента почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b45c6-104">The **UploadItemsResponseMessage** element contains the status and results of a request to upload a single mailbox item.</span></span> 
  
- [<span data-ttu-id="b45c6-105">уплоадитемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="b45c6-105">UploadItemsResponse</span></span>](uploaditemsresponse.md) 
- [<span data-ttu-id="b45c6-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="b45c6-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="b45c6-107">уплоадитемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="b45c6-107">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
  
```XML
<UploadItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
</UploadItemsResponseMessage>
```

 <span data-ttu-id="b45c6-108">**уплоадитемсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="b45c6-108">**UploadItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b45c6-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b45c6-109">Attributes and elements</span></span>

<span data-ttu-id="b45c6-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b45c6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b45c6-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b45c6-111">Attributes</span></span>

|<span data-ttu-id="b45c6-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b45c6-112">**Attribute**</span></span>|<span data-ttu-id="b45c6-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b45c6-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b45c6-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="b45c6-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b45c6-115">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="b45c6-115">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="b45c6-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="b45c6-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="b45c6-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="b45c6-117">-  Success</span></span>  <br/><span data-ttu-id="b45c6-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="b45c6-118">-  Warning</span></span>  <br/><span data-ttu-id="b45c6-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="b45c6-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b45c6-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="b45c6-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="b45c6-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b45c6-121">**Value**</span></span>|<span data-ttu-id="b45c6-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b45c6-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b45c6-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="b45c6-123">**Success**</span></span> <br/> |<span data-ttu-id="b45c6-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="b45c6-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b45c6-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="b45c6-125">**Warning**</span></span> <br/> | <span data-ttu-id="b45c6-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="b45c6-126">Describes a request that was not processed.</span></span> <span data-ttu-id="b45c6-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="b45c6-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b45c6-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="b45c6-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b45c6-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="b45c6-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b45c6-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="b45c6-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="b45c6-131">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="b45c6-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="b45c6-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="b45c6-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b45c6-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="b45c6-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="b45c6-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="b45c6-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="b45c6-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="b45c6-135">**Error**</span></span> <br/> | <span data-ttu-id="b45c6-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="b45c6-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b45c6-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="b45c6-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b45c6-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="b45c6-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b45c6-139">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="b45c6-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="b45c6-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="b45c6-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="b45c6-141">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="b45c6-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="b45c6-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="b45c6-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b45c6-143">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="b45c6-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="b45c6-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b45c6-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b45c6-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b45c6-145">Child elements</span></span>

|<span data-ttu-id="b45c6-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b45c6-146">**Element**</span></span>|<span data-ttu-id="b45c6-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b45c6-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b45c6-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="b45c6-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b45c6-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="b45c6-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b45c6-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b45c6-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b45c6-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="b45c6-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b45c6-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="b45c6-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b45c6-153">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="b45c6-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="b45c6-154">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="b45c6-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b45c6-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="b45c6-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b45c6-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="b45c6-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b45c6-157">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="b45c6-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b45c6-158">Содержит идентификатор элемента отправленного элемента.</span><span class="sxs-lookup"><span data-stu-id="b45c6-158">Contains the item identifier of an uploaded item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b45c6-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b45c6-159">Parent elements</span></span>

|<span data-ttu-id="b45c6-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b45c6-160">**Element**</span></span>|<span data-ttu-id="b45c6-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b45c6-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b45c6-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="b45c6-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b45c6-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="b45c6-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b45c6-164">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b45c6-164">Text value</span></span>

<span data-ttu-id="b45c6-165">Нет.</span><span class="sxs-lookup"><span data-stu-id="b45c6-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b45c6-166">Примечания</span><span class="sxs-lookup"><span data-stu-id="b45c6-166">Remarks</span></span>

<span data-ttu-id="b45c6-167">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b45c6-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b45c6-168">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b45c6-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b45c6-169">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b45c6-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b45c6-170">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b45c6-170">Schema Name</span></span>  <br/> |<span data-ttu-id="b45c6-171">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="b45c6-171">Message schema</span></span>  <br/> |
|<span data-ttu-id="b45c6-172">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b45c6-172">Validation File</span></span>  <br/> |<span data-ttu-id="b45c6-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b45c6-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b45c6-174">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b45c6-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="b45c6-175">False</span><span class="sxs-lookup"><span data-stu-id="b45c6-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b45c6-176">См. также</span><span class="sxs-lookup"><span data-stu-id="b45c6-176">See also</span></span>

- [<span data-ttu-id="b45c6-177">Операция ExportItems</span><span class="sxs-lookup"><span data-stu-id="b45c6-177">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="b45c6-178">Операция UploadItems</span><span class="sxs-lookup"><span data-stu-id="b45c6-178">UploadItems operation</span></span>](uploaditems-operation.md)
- [<span data-ttu-id="b45c6-179">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b45c6-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

