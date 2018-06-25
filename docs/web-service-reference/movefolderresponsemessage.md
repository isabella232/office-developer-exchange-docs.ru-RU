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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834496"
---
# <a name="movefolderresponsemessage"></a><span data-ttu-id="dbaba-103">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dbaba-103">MoveFolderResponseMessage</span></span>

<span data-ttu-id="dbaba-104">Элемент **MoveFolderResponseMessage** содержит состояние и результат одного запроса [MoveFolder операции](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dbaba-104">The **MoveFolderResponseMessage** element contains the status and result of a single [MoveFolder operation](movefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="dbaba-105">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="dbaba-105">MoveFolderResponse</span></span>](movefolderresponse.md)
- [<span data-ttu-id="dbaba-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dbaba-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="dbaba-107">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dbaba-107">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
  
```xml
<MoveFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</MoveFolderResponseMessage>
```

 <span data-ttu-id="dbaba-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="dbaba-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbaba-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dbaba-109">Attributes and elements</span></span>

<span data-ttu-id="dbaba-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dbaba-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbaba-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dbaba-111">Attributes</span></span>

|<span data-ttu-id="dbaba-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="dbaba-112">**Attribute**</span></span>|<span data-ttu-id="dbaba-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dbaba-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dbaba-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="dbaba-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="dbaba-115">Описание состояния ответа [операции MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dbaba-115">Describes the status of a [MoveFolder operation](movefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="dbaba-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="dbaba-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="dbaba-117">-Success</span><span class="sxs-lookup"><span data-stu-id="dbaba-117">-  Success</span></span>  <br/><span data-ttu-id="dbaba-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="dbaba-118">-  Warning</span></span>  <br/><span data-ttu-id="dbaba-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="dbaba-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="dbaba-120">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="dbaba-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="dbaba-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="dbaba-121">**Value**</span></span>|<span data-ttu-id="dbaba-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dbaba-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dbaba-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="dbaba-123">**Success**</span></span> <br/> |<span data-ttu-id="dbaba-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="dbaba-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="dbaba-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="dbaba-125">**Warning**</span></span> <br/> | <span data-ttu-id="dbaba-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="dbaba-126">Describes a request that was not processed.</span></span> <span data-ttu-id="dbaba-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="dbaba-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="dbaba-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="dbaba-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="dbaba-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="dbaba-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="dbaba-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="dbaba-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="dbaba-131">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="dbaba-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="dbaba-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="dbaba-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="dbaba-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="dbaba-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="dbaba-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="dbaba-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="dbaba-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="dbaba-135">**Error**</span></span> <br/> | <span data-ttu-id="dbaba-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="dbaba-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="dbaba-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="dbaba-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="dbaba-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dbaba-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="dbaba-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="dbaba-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="dbaba-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="dbaba-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="dbaba-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="dbaba-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="dbaba-142">-Любая попытка несанкционированного доступа любого клиента</span><span class="sxs-lookup"><span data-stu-id="dbaba-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="dbaba-143">-Любые ошибки на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="dbaba-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="dbaba-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="dbaba-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dbaba-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dbaba-145">Child elements</span></span>

|<span data-ttu-id="dbaba-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dbaba-146">**Element**</span></span>|<span data-ttu-id="dbaba-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dbaba-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbaba-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="dbaba-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="dbaba-149">Текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="dbaba-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="dbaba-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dbaba-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="dbaba-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="dbaba-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="dbaba-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="dbaba-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="dbaba-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="dbaba-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="dbaba-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="dbaba-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="dbaba-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="dbaba-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="dbaba-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="dbaba-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="dbaba-157">Папки</span><span class="sxs-lookup"><span data-stu-id="dbaba-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="dbaba-158">Содержит массив перемещенной папки.</span><span class="sxs-lookup"><span data-stu-id="dbaba-158">Contains an array of moved folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dbaba-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dbaba-159">Parent elements</span></span>

|<span data-ttu-id="dbaba-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dbaba-160">**Element**</span></span>|<span data-ttu-id="dbaba-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dbaba-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbaba-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dbaba-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="dbaba-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="dbaba-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dbaba-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="dbaba-164">Remarks</span></span>

<span data-ttu-id="dbaba-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dbaba-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbaba-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dbaba-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbaba-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dbaba-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dbaba-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dbaba-168">Schema Name</span></span>  <br/> |<span data-ttu-id="dbaba-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dbaba-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dbaba-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dbaba-170">Validation File</span></span>  <br/> |<span data-ttu-id="dbaba-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dbaba-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dbaba-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dbaba-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbaba-173">False</span><span class="sxs-lookup"><span data-stu-id="dbaba-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbaba-174">См. также</span><span class="sxs-lookup"><span data-stu-id="dbaba-174">See also</span></span>

- [<span data-ttu-id="dbaba-175">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="dbaba-175">MoveFolder</span></span>](movefolder.md)
- [<span data-ttu-id="dbaba-176">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="dbaba-176">MoveFolder operation</span></span>](movefolder-operation.md)

