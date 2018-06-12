---
title: MoveFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolderResponseMessage
api_type:
- schema
ms.assetid: 54917251-96af-44c2-ae90-d545f0a16e2e
description: Элемент MoveFolderResponseMessage содержит состояние и результат одного запроса MoveFolder операции.
ms.openlocfilehash: 777520bf6a093882da95a7bfd466b66acdab957c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834496"
---
# <a name="movefolderresponsemessage"></a><span data-ttu-id="dd38e-103">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dd38e-103">MoveFolderResponseMessage</span></span>

<span data-ttu-id="dd38e-104">Элемент **MoveFolderResponseMessage** содержит состояние и результат одного запроса [MoveFolder операции](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dd38e-104">The **MoveFolderResponseMessage** element contains the status and result of a single [MoveFolder operation](movefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="dd38e-105">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="dd38e-105">MoveFolderResponse</span></span>](movefolderresponse.md)
- [<span data-ttu-id="dd38e-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dd38e-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="dd38e-107">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dd38e-107">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
  
```xml
<MoveFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</MoveFolderResponseMessage>
```

 <span data-ttu-id="dd38e-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="dd38e-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd38e-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dd38e-109">Attributes and elements</span></span>

<span data-ttu-id="dd38e-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dd38e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd38e-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dd38e-111">Attributes</span></span>

|<span data-ttu-id="dd38e-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="dd38e-112">**Attribute**</span></span>|<span data-ttu-id="dd38e-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd38e-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dd38e-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="dd38e-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="dd38e-115">Описание состояния ответа [операции MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dd38e-115">Describes the status of a [MoveFolder operation](movefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="dd38e-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="dd38e-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="dd38e-117">-Success</span><span class="sxs-lookup"><span data-stu-id="dd38e-117">-  Success</span></span>  <br/><span data-ttu-id="dd38e-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="dd38e-118">-  Warning</span></span>  <br/><span data-ttu-id="dd38e-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="dd38e-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="dd38e-120">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="dd38e-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="dd38e-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="dd38e-121">**Value**</span></span>|<span data-ttu-id="dd38e-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd38e-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dd38e-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="dd38e-123">**Success**</span></span> <br/> |<span data-ttu-id="dd38e-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="dd38e-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="dd38e-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="dd38e-125">**Warning**</span></span> <br/> | <span data-ttu-id="dd38e-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="dd38e-126">Describes a request that was not processed.</span></span> <span data-ttu-id="dd38e-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="dd38e-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="dd38e-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="dd38e-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="dd38e-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="dd38e-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="dd38e-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="dd38e-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="dd38e-131">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="dd38e-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="dd38e-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="dd38e-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="dd38e-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="dd38e-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="dd38e-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="dd38e-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="dd38e-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="dd38e-135">**Error**</span></span> <br/> | <span data-ttu-id="dd38e-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="dd38e-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="dd38e-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="dd38e-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="dd38e-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dd38e-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="dd38e-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="dd38e-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="dd38e-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="dd38e-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="dd38e-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="dd38e-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="dd38e-142">-Любая попытка несанкционированного доступа любого клиента</span><span class="sxs-lookup"><span data-stu-id="dd38e-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="dd38e-143">-Любые ошибки на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="dd38e-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="dd38e-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="dd38e-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dd38e-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dd38e-145">Child elements</span></span>

|<span data-ttu-id="dd38e-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dd38e-146">**Element**</span></span>|<span data-ttu-id="dd38e-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd38e-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd38e-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="dd38e-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="dd38e-149">Текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="dd38e-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="dd38e-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dd38e-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="dd38e-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="dd38e-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="dd38e-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="dd38e-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="dd38e-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="dd38e-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="dd38e-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="dd38e-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="dd38e-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="dd38e-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="dd38e-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="dd38e-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="dd38e-157">Папки</span><span class="sxs-lookup"><span data-stu-id="dd38e-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="dd38e-158">Содержит массив перемещенной папки.</span><span class="sxs-lookup"><span data-stu-id="dd38e-158">Contains an array of moved folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dd38e-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dd38e-159">Parent elements</span></span>

|<span data-ttu-id="dd38e-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dd38e-160">**Element**</span></span>|<span data-ttu-id="dd38e-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd38e-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd38e-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dd38e-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dd38e-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd38e-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dd38e-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="dd38e-164">Remarks</span></span>

<span data-ttu-id="dd38e-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dd38e-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd38e-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dd38e-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd38e-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dd38e-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dd38e-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dd38e-168">Schema Name</span></span>  <br/> |<span data-ttu-id="dd38e-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dd38e-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dd38e-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dd38e-170">Validation File</span></span>  <br/> |<span data-ttu-id="dd38e-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dd38e-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dd38e-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dd38e-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd38e-173">False</span><span class="sxs-lookup"><span data-stu-id="dd38e-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd38e-174">См. также</span><span class="sxs-lookup"><span data-stu-id="dd38e-174">See also</span></span>

- [<span data-ttu-id="dd38e-175">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="dd38e-175">MoveFolder</span></span>](movefolder.md)
- [<span data-ttu-id="dd38e-176">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="dd38e-176">MoveFolder operation</span></span>](movefolder-operation.md)

