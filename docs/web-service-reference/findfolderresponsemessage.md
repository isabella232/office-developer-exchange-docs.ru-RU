---
title: FindFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolderResponseMessage
api_type:
- schema
ms.assetid: 538d64fe-51ae-41d2-bfab-91698678aa1b
description: Элемент FindFolderResponseMessage содержит состояние и результат одного запроса FindFolder операции.
ms.openlocfilehash: 5623e5e538e617e5bd4bbc4444328ac83d7b8065
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762567"
---
# <a name="findfolderresponsemessage"></a><span data-ttu-id="07b66-103">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="07b66-103">FindFolderResponseMessage</span></span>

<span data-ttu-id="07b66-104">Элемент **FindFolderResponseMessage** содержит состояние и результат одного запроса [FindFolder операции](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="07b66-104">The **FindFolderResponseMessage** element contains the status and result of a single [FindFolder operation](findfolder-operation.md) request.</span></span> 
  
[<span data-ttu-id="07b66-105">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="07b66-105">FindFolderResponse</span></span>](findfolderresponse.md)
  
[<span data-ttu-id="07b66-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="07b66-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="07b66-107">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="07b66-107">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
  
```xml
<FindFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindFolderResponseMessage>
```

 <span data-ttu-id="07b66-108">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="07b66-108">**FindFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07b66-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="07b66-109">Attributes and elements</span></span>

<span data-ttu-id="07b66-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="07b66-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07b66-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="07b66-111">Attributes</span></span>

|<span data-ttu-id="07b66-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="07b66-112">**Attribute**</span></span>|<span data-ttu-id="07b66-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07b66-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="07b66-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="07b66-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="07b66-115">Описание состояния ответа [FindFolder операции](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="07b66-115">Describes the status of a [FindFolder operation](findfolder-operation.md) response.</span></span><br/><br/> <span data-ttu-id="07b66-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="07b66-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="07b66-117">-Success</span><span class="sxs-lookup"><span data-stu-id="07b66-117">-  Success</span></span>  <br/><span data-ttu-id="07b66-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="07b66-118">-  Warning</span></span>  <br/><span data-ttu-id="07b66-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="07b66-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="07b66-120">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="07b66-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="07b66-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="07b66-121">**Value**</span></span>|<span data-ttu-id="07b66-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07b66-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="07b66-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="07b66-123">**Success**</span></span> <br/> |<span data-ttu-id="07b66-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="07b66-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="07b66-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="07b66-125">**Warning**</span></span> <br/> | <span data-ttu-id="07b66-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="07b66-126">Describes a request that was not processed.</span></span> <span data-ttu-id="07b66-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="07b66-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="07b66-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="07b66-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="07b66-129">-В хранилище Exchange переходит в автономный режим во время пакета.</span><span class="sxs-lookup"><span data-stu-id="07b66-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="07b66-130">-Доменных служб active Directory (AD DS) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="07b66-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="07b66-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="07b66-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="07b66-132">-База данных сообщений (MDB) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="07b66-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="07b66-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="07b66-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="07b66-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="07b66-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="07b66-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="07b66-135">**Error**</span></span> <br/> | <span data-ttu-id="07b66-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="07b66-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="07b66-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="07b66-137">The following are examples of sources of errors:</span></span>  <br/><span data-ttu-id="07b66-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="07b66-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="07b66-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="07b66-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="07b66-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="07b66-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="07b66-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="07b66-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="07b66-142">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="07b66-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="07b66-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="07b66-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="07b66-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="07b66-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="07b66-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="07b66-145">Child elements</span></span>

|<span data-ttu-id="07b66-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="07b66-146">**Element**</span></span>|<span data-ttu-id="07b66-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07b66-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07b66-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="07b66-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="07b66-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="07b66-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="07b66-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="07b66-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="07b66-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="07b66-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="07b66-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="07b66-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="07b66-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="07b66-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="07b66-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="07b66-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="07b66-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="07b66-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="07b66-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="07b66-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="07b66-157">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="07b66-157">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="07b66-158">Содержит результаты поиска в одной корневой папке во время [операции FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="07b66-158">Contains the results from a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07b66-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="07b66-159">Parent elements</span></span>

|<span data-ttu-id="07b66-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="07b66-160">**Element**</span></span>|<span data-ttu-id="07b66-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07b66-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07b66-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="07b66-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="07b66-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="07b66-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07b66-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="07b66-164">Remarks</span></span>

<span data-ttu-id="07b66-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="07b66-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07b66-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="07b66-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07b66-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="07b66-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="07b66-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="07b66-168">Schema name</span></span>  <br/> |<span data-ttu-id="07b66-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="07b66-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="07b66-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="07b66-170">Validation file</span></span>  <br/> |<span data-ttu-id="07b66-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="07b66-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="07b66-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="07b66-172">Can be empty</span></span>  <br/> |<span data-ttu-id="07b66-173">False</span><span class="sxs-lookup"><span data-stu-id="07b66-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07b66-174">См. также</span><span class="sxs-lookup"><span data-stu-id="07b66-174">See also</span></span>

- [<span data-ttu-id="07b66-175">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="07b66-175">FindFolder operation</span></span>](findfolder-operation.md)
- [<span data-ttu-id="07b66-176">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="07b66-176">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

