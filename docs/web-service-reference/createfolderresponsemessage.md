---
title: CreateFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolderResponseMessage
api_type:
- schema
ms.assetid: 1301dd15-b008-4fd9-8c89-b15a20b186e2
description: Элемент CreateFolderResponseMessage содержит состояние и результат одного запроса CreateFolder операции.
ms.openlocfilehash: c587cca1f935b295a0ed30ab2210de40af28d06d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761884"
---
# <a name="createfolderresponsemessage"></a><span data-ttu-id="bf32b-103">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bf32b-103">CreateFolderResponseMessage</span></span>

<span data-ttu-id="bf32b-104">Элемент **CreateFolderResponseMessage** содержит состояние и результат одного запроса [CreateFolder операции](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bf32b-104">The **CreateFolderResponseMessage** element contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span> 
  
```xml
<CreateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateFolderResponseMessage>
```

<span data-ttu-id="bf32b-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bf32b-105">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bf32b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bf32b-106">Attributes and elements</span></span>

<span data-ttu-id="bf32b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bf32b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf32b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bf32b-108">Attributes</span></span>

|<span data-ttu-id="bf32b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bf32b-109">**Attribute**</span></span>|<span data-ttu-id="bf32b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf32b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bf32b-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="bf32b-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bf32b-112">Описание состояния ответа [CreateFolder операции](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bf32b-112">Describes the status of a [CreateFolder operation](createfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="bf32b-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="bf32b-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="bf32b-114">-Success</span><span class="sxs-lookup"><span data-stu-id="bf32b-114">-  Success</span></span>  <br/><span data-ttu-id="bf32b-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="bf32b-115">-  Warning</span></span>  <br/><span data-ttu-id="bf32b-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="bf32b-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="bf32b-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="bf32b-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="bf32b-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="bf32b-118">**Value**</span></span>|<span data-ttu-id="bf32b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf32b-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bf32b-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="bf32b-120">**Success**</span></span> <br/> |<span data-ttu-id="bf32b-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="bf32b-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bf32b-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="bf32b-122">**Warning**</span></span> <br/> | <span data-ttu-id="bf32b-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="bf32b-123">Describes a request that was not processed.</span></span> <span data-ttu-id="bf32b-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="bf32b-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="bf32b-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="bf32b-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="bf32b-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="bf32b-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="bf32b-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="bf32b-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="bf32b-128">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="bf32b-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="bf32b-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="bf32b-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="bf32b-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="bf32b-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="bf32b-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="bf32b-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="bf32b-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="bf32b-132">**Error**</span></span> <br/> | <span data-ttu-id="bf32b-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="bf32b-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="bf32b-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="bf32b-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="bf32b-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bf32b-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="bf32b-136">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="bf32b-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="bf32b-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="bf32b-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="bf32b-138">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="bf32b-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="bf32b-139">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="bf32b-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="bf32b-140">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="bf32b-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="bf32b-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="bf32b-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bf32b-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bf32b-142">Child elements</span></span>

|<span data-ttu-id="bf32b-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bf32b-143">**Element**</span></span>|<span data-ttu-id="bf32b-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf32b-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf32b-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="bf32b-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bf32b-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="bf32b-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bf32b-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bf32b-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bf32b-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="bf32b-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bf32b-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bf32b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bf32b-150">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="bf32b-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="bf32b-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="bf32b-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bf32b-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="bf32b-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bf32b-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="bf32b-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="bf32b-154">Папки</span><span class="sxs-lookup"><span data-stu-id="bf32b-154">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bf32b-155">Содержит массив созданные папки.</span><span class="sxs-lookup"><span data-stu-id="bf32b-155">Contains an array of created folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bf32b-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bf32b-156">Parent elements</span></span>

|<span data-ttu-id="bf32b-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bf32b-157">**Element**</span></span>|<span data-ttu-id="bf32b-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf32b-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf32b-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bf32b-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bf32b-160">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf32b-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bf32b-161">Замечания</span><span class="sxs-lookup"><span data-stu-id="bf32b-161">Remarks</span></span>

<span data-ttu-id="bf32b-162">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bf32b-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf32b-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bf32b-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf32b-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bf32b-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bf32b-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bf32b-165">Schema Name</span></span>  <br/> |<span data-ttu-id="bf32b-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bf32b-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bf32b-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bf32b-167">Validation File</span></span>  <br/> |<span data-ttu-id="bf32b-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bf32b-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bf32b-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bf32b-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="bf32b-170">False</span><span class="sxs-lookup"><span data-stu-id="bf32b-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf32b-171">См. также</span><span class="sxs-lookup"><span data-stu-id="bf32b-171">See also</span></span>

- [<span data-ttu-id="bf32b-172">CreateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="bf32b-172">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="bf32b-173">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="bf32b-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="bf32b-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bf32b-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

