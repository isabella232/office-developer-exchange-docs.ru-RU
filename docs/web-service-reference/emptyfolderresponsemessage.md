---
title: емптифолдерреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 678dd5ce-8d9e-4939-bf1b-a8e148f4f449
description: Элемент Емптифолдерреспонсемессаже содержит состояние и результат одного запроса EmptyFolder.
ms.openlocfilehash: ebdaac28cdd16a55811276ef0d11c03b00d3897a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762329"
---
# <a name="emptyfolderresponsemessage"></a><span data-ttu-id="5b124-103">емптифолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="5b124-103">EmptyFolderResponseMessage</span></span>

<span data-ttu-id="5b124-104">Элемент **емптифолдерреспонсемессаже** содержит состояние и результат одного запроса [EmptyFolder](emptyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="5b124-104">The **EmptyFolderResponseMessage** element contains the status and result of a single [EmptyFolder](emptyfolder.md) request.</span></span> 
  
```XML
<EmptyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</EmptyFolderResponseMessage>
```

 <span data-ttu-id="5b124-105">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="5b124-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b124-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5b124-106">Attributes and elements</span></span>

<span data-ttu-id="5b124-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5b124-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b124-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5b124-108">Attributes</span></span>

|<span data-ttu-id="5b124-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="5b124-109">**Attribute**</span></span>|<span data-ttu-id="5b124-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5b124-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5b124-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="5b124-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5b124-112">Описывает состояние ответа [операции EmptyFolder](emptyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5b124-112">Describes the status of an [EmptyFolder operation](emptyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="5b124-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="5b124-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="5b124-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="5b124-114">-  Success</span></span>  <br/><span data-ttu-id="5b124-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="5b124-115">-  Warning</span></span>  <br/><span data-ttu-id="5b124-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="5b124-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="5b124-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="5b124-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="5b124-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="5b124-118">**Value**</span></span>|<span data-ttu-id="5b124-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5b124-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5b124-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="5b124-120">**Success**</span></span> <br/> |<span data-ttu-id="5b124-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="5b124-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5b124-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="5b124-122">**Warning**</span></span> <br/> | <span data-ttu-id="5b124-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="5b124-123">Describes a request that was not processed.</span></span> <span data-ttu-id="5b124-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="5b124-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="5b124-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="5b124-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="5b124-126">— Хранилище Exchange в пакетном режиме переключается в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="5b124-126">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="5b124-127">-Доменные службы Active Directory (AD DS) переключаются в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="5b124-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="5b124-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="5b124-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="5b124-129">— База данных сообщений (MDB) переводится в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="5b124-129">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="5b124-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="5b124-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="5b124-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="5b124-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="5b124-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="5b124-132">**Error**</span></span> <br/> | <span data-ttu-id="5b124-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="5b124-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="5b124-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="5b124-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="5b124-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="5b124-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="5b124-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="5b124-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="5b124-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="5b124-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="5b124-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="5b124-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="5b124-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="5b124-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="5b124-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="5b124-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="5b124-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="5b124-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5b124-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5b124-142">Child elements</span></span>

|<span data-ttu-id="5b124-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5b124-143">**Element**</span></span>|<span data-ttu-id="5b124-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5b124-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b124-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="5b124-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5b124-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="5b124-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5b124-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="5b124-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5b124-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="5b124-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5b124-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="5b124-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5b124-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="5b124-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="5b124-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="5b124-151">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5b124-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="5b124-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5b124-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5b124-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5b124-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5b124-154">Parent elements</span></span>

|<span data-ttu-id="5b124-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5b124-155">**Element**</span></span>|<span data-ttu-id="5b124-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5b124-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b124-157">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="5b124-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5b124-158">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b124-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5b124-159">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5b124-159">Text value</span></span>

<span data-ttu-id="5b124-160">Нет.</span><span class="sxs-lookup"><span data-stu-id="5b124-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5b124-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="5b124-161">Remarks</span></span>

<span data-ttu-id="5b124-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b124-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b124-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5b124-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b124-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5b124-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5b124-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5b124-165">Schema Name</span></span>  <br/> |<span data-ttu-id="5b124-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5b124-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5b124-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5b124-167">Validation File</span></span>  <br/> |<span data-ttu-id="5b124-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5b124-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5b124-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5b124-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b124-170">False</span><span class="sxs-lookup"><span data-stu-id="5b124-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b124-171">См. также</span><span class="sxs-lookup"><span data-stu-id="5b124-171">See also</span></span>

- [<span data-ttu-id="5b124-172">Операция EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="5b124-172">EmptyFolder operation</span></span>](emptyfolder-operation.md)
- [<span data-ttu-id="5b124-173">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="5b124-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="5b124-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5b124-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

