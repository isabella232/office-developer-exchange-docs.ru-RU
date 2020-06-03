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
ms.openlocfilehash: fd69df45d7e1d6538a977b79711baa769413ea66
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526216"
---
# <a name="emptyfolderresponsemessage"></a><span data-ttu-id="d83ce-103">емптифолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="d83ce-103">EmptyFolderResponseMessage</span></span>

<span data-ttu-id="d83ce-104">Элемент **емптифолдерреспонсемессаже** содержит состояние и результат одного запроса [EmptyFolder](emptyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="d83ce-104">The **EmptyFolderResponseMessage** element contains the status and result of a single [EmptyFolder](emptyfolder.md) request.</span></span> 
  
```XML
<EmptyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</EmptyFolderResponseMessage>
```

 <span data-ttu-id="d83ce-105">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="d83ce-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d83ce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d83ce-106">Attributes and elements</span></span>

<span data-ttu-id="d83ce-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d83ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d83ce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d83ce-108">Attributes</span></span>

|<span data-ttu-id="d83ce-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d83ce-109">**Attribute**</span></span>|<span data-ttu-id="d83ce-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d83ce-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d83ce-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="d83ce-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d83ce-112">Описывает состояние ответа [операции EmptyFolder](emptyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d83ce-112">Describes the status of an [EmptyFolder operation](emptyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="d83ce-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d83ce-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="d83ce-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="d83ce-114">-  Success</span></span>  <br/><span data-ttu-id="d83ce-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="d83ce-115">-  Warning</span></span>  <br/><span data-ttu-id="d83ce-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="d83ce-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d83ce-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="d83ce-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="d83ce-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d83ce-118">**Value**</span></span>|<span data-ttu-id="d83ce-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d83ce-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d83ce-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="d83ce-120">**Success**</span></span> <br/> |<span data-ttu-id="d83ce-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="d83ce-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d83ce-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="d83ce-122">**Warning**</span></span> <br/> | <span data-ttu-id="d83ce-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="d83ce-123">Describes a request that was not processed.</span></span> <span data-ttu-id="d83ce-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="d83ce-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="d83ce-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="d83ce-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="d83ce-126">— Хранилище Exchange в пакетном режиме переключается в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="d83ce-126">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="d83ce-127">-Доменные службы Active Directory (AD DS) переключаются в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="d83ce-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="d83ce-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="d83ce-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="d83ce-129">— База данных сообщений (MDB) переводится в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="d83ce-129">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="d83ce-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="d83ce-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="d83ce-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="d83ce-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="d83ce-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="d83ce-132">**Error**</span></span> <br/> | <span data-ttu-id="d83ce-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="d83ce-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="d83ce-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="d83ce-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d83ce-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="d83ce-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d83ce-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="d83ce-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="d83ce-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="d83ce-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="d83ce-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="d83ce-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="d83ce-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="d83ce-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d83ce-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="d83ce-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="d83ce-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="d83ce-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d83ce-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d83ce-142">Child elements</span></span>

|<span data-ttu-id="d83ce-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d83ce-143">**Element**</span></span>|<span data-ttu-id="d83ce-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d83ce-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d83ce-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="d83ce-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d83ce-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="d83ce-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d83ce-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="d83ce-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d83ce-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="d83ce-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d83ce-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="d83ce-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d83ce-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="d83ce-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d83ce-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="d83ce-151">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d83ce-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="d83ce-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d83ce-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d83ce-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d83ce-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d83ce-154">Parent elements</span></span>

|<span data-ttu-id="d83ce-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d83ce-155">**Element**</span></span>|<span data-ttu-id="d83ce-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d83ce-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d83ce-157">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="d83ce-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d83ce-158">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="d83ce-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d83ce-159">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d83ce-159">Text value</span></span>

<span data-ttu-id="d83ce-160">Нет.</span><span class="sxs-lookup"><span data-stu-id="d83ce-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d83ce-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="d83ce-161">Remarks</span></span>

<span data-ttu-id="d83ce-162">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d83ce-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d83ce-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d83ce-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d83ce-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d83ce-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d83ce-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d83ce-165">Schema Name</span></span>  <br/> |<span data-ttu-id="d83ce-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d83ce-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d83ce-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d83ce-167">Validation File</span></span>  <br/> |<span data-ttu-id="d83ce-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d83ce-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d83ce-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d83ce-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="d83ce-170">False</span><span class="sxs-lookup"><span data-stu-id="d83ce-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d83ce-171">См. также</span><span class="sxs-lookup"><span data-stu-id="d83ce-171">See also</span></span>

- [<span data-ttu-id="d83ce-172">Операция EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="d83ce-172">EmptyFolder operation</span></span>](emptyfolder-operation.md)
- [<span data-ttu-id="d83ce-173">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="d83ce-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="d83ce-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d83ce-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

