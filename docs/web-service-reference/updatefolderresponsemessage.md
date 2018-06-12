---
title: UpdateFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolderResponseMessage
api_type:
- schema
ms.assetid: 914bb683-49ee-44a2-b59d-ef560244dfb8
description: Элемент UpdateFolderResponseMessage содержит состояние и результат обновления, определенные в элементе FolderChange UpdateFolder операция запроса.
ms.openlocfilehash: 4cd00232bcc233f6534d844418f523c248ce54bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840340"
---
# <a name="updatefolderresponsemessage"></a><span data-ttu-id="a2da5-103">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a2da5-103">UpdateFolderResponseMessage</span></span>

<span data-ttu-id="a2da5-104">Элемент **UpdateFolderResponseMessage** содержит состояние и результат обновления, определенные в элементе [FolderChange](folderchange.md) [UpdateFolder операции](updatefolder-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="a2da5-104">The **UpdateFolderResponseMessage** element contains the status and result of updates defined by the [FolderChange](folderchange.md) element of an [UpdateFolder operation](updatefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="a2da5-105">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a2da5-105">UpdateFolderResponse</span></span>](updatefolderresponse.md) 
- [<span data-ttu-id="a2da5-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a2da5-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="a2da5-107">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a2da5-107">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
  
```xml
<UpdateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</UpdateFolderResponseMessage>
```

 <span data-ttu-id="a2da5-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a2da5-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2da5-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2da5-109">Attributes and elements</span></span>

<span data-ttu-id="a2da5-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a2da5-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2da5-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2da5-111">Attributes</span></span>

|<span data-ttu-id="a2da5-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a2da5-112">**Attribute**</span></span>|<span data-ttu-id="a2da5-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2da5-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a2da5-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="a2da5-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a2da5-115">Описание состояния ответа [операции UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a2da5-115">Describes the status of an [UpdateFolder operation](updatefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="a2da5-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="a2da5-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="a2da5-117">-Success</span><span class="sxs-lookup"><span data-stu-id="a2da5-117">-  Success</span></span>  <br/><span data-ttu-id="a2da5-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="a2da5-118">-  Warning</span></span>  <br/><span data-ttu-id="a2da5-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="a2da5-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a2da5-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a2da5-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="a2da5-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a2da5-121">**Value**</span></span>|<span data-ttu-id="a2da5-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2da5-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a2da5-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="a2da5-123">**Success**</span></span> <br/> |<span data-ttu-id="a2da5-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="a2da5-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a2da5-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="a2da5-125">**Warning**</span></span> <br/> | <span data-ttu-id="a2da5-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="a2da5-126">Describes a request that was not processed.</span></span> <span data-ttu-id="a2da5-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="a2da5-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="a2da5-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="a2da5-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="a2da5-129">-В хранилище Exchange находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="a2da5-129">-  The Exchange store is offline.</span></span>  <br/><span data-ttu-id="a2da5-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="a2da5-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="a2da5-131">-Переместить почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a2da5-131">-  A mailbox is moved.</span></span>  <br/><span data-ttu-id="a2da5-132">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="a2da5-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="a2da5-133">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="a2da5-133">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="a2da5-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="a2da5-134">**Error**</span></span> <br/> | <span data-ttu-id="a2da5-135">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="a2da5-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="a2da5-136">Ниже приведены примеры источников для ошибки:</span><span class="sxs-lookup"><span data-stu-id="a2da5-136">The following are examples of sources for errors:</span></span>  <br/><br/><span data-ttu-id="a2da5-137">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2da5-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="a2da5-138">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="a2da5-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="a2da5-139">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="a2da5-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="a2da5-140">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="a2da5-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="a2da5-141">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="a2da5-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a2da5-142">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="a2da5-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="a2da5-143">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="a2da5-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a2da5-144">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2da5-144">Child elements</span></span>

|<span data-ttu-id="a2da5-145">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2da5-145">**Element**</span></span>|<span data-ttu-id="a2da5-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2da5-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2da5-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="a2da5-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a2da5-148">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="a2da5-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a2da5-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a2da5-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a2da5-150">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="a2da5-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a2da5-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a2da5-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a2da5-152">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="a2da5-152">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="a2da5-153">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="a2da5-153">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a2da5-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a2da5-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a2da5-155">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="a2da5-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a2da5-156">Папки</span><span class="sxs-lookup"><span data-stu-id="a2da5-156">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a2da5-157">Содержит набор папок, используемых в папке операции.</span><span class="sxs-lookup"><span data-stu-id="a2da5-157">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2da5-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2da5-158">Parent elements</span></span>

|<span data-ttu-id="a2da5-159">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2da5-159">**Element**</span></span>|<span data-ttu-id="a2da5-160">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2da5-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2da5-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a2da5-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a2da5-162">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2da5-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2da5-163">Замечания</span><span class="sxs-lookup"><span data-stu-id="a2da5-163">Remarks</span></span>

<span data-ttu-id="a2da5-164">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a2da5-164">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2da5-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a2da5-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2da5-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a2da5-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a2da5-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a2da5-167">Schema Name</span></span>  <br/> |<span data-ttu-id="a2da5-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a2da5-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a2da5-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a2da5-169">Validation File</span></span>  <br/> |<span data-ttu-id="a2da5-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a2da5-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a2da5-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a2da5-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2da5-172">False</span><span class="sxs-lookup"><span data-stu-id="a2da5-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2da5-173">См. также</span><span class="sxs-lookup"><span data-stu-id="a2da5-173">See also</span></span>

- [<span data-ttu-id="a2da5-174">Операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="a2da5-174">UpdateFolder operation</span></span>](updatefolder-operation.md)

