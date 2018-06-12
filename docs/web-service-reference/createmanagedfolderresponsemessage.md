---
title: CreateManagedFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolderResponseMessage
api_type:
- schema
ms.assetid: a72eefc3-ef0b-4b44-a74b-e6907b5b5f68
description: Элемент CreateManagedFolderResponseMessage содержит состояние и результат одного запроса CreateManagedFolder операции.
ms.openlocfilehash: e561cac949ebebc647b16578c6acbcd6132eeef7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761914"
---
# <a name="createmanagedfolderresponsemessage"></a><span data-ttu-id="d2a06-103">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d2a06-103">CreateManagedFolderResponseMessage</span></span>

<span data-ttu-id="d2a06-104">Элемент **CreateManagedFolderResponseMessage** содержит состояние и результат одного запроса [CreateManagedFolder операции](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d2a06-104">The **CreateManagedFolderResponseMessage** element contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="d2a06-105">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="d2a06-105">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)  
- [<span data-ttu-id="d2a06-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d2a06-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="d2a06-107">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d2a06-107">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
  
```xml
<CreateManagedFolderResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateManagedFolderResponseMessage>
```

<span data-ttu-id="d2a06-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d2a06-108">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d2a06-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d2a06-109">Attributes and elements</span></span>

<span data-ttu-id="d2a06-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d2a06-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2a06-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d2a06-111">Attributes</span></span>

|<span data-ttu-id="d2a06-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d2a06-112">**Attribute**</span></span>|<span data-ttu-id="d2a06-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d2a06-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2a06-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d2a06-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d2a06-115">Описание состояния ответа [операции CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d2a06-115">Describes the status of a [CreateManagedFolder operation](createmanagedfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="d2a06-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d2a06-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="d2a06-117">-Success</span><span class="sxs-lookup"><span data-stu-id="d2a06-117">-  Success</span></span>  <br/><span data-ttu-id="d2a06-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="d2a06-118">-  Warning</span></span>  <br/><span data-ttu-id="d2a06-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="d2a06-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d2a06-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d2a06-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="d2a06-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d2a06-121">**Value**</span></span>|<span data-ttu-id="d2a06-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d2a06-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2a06-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="d2a06-123">**Success**</span></span> <br/> |<span data-ttu-id="d2a06-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="d2a06-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d2a06-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="d2a06-125">**Warning**</span></span> <br/> | <span data-ttu-id="d2a06-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="d2a06-126">Describes a request that was not processed.</span></span> <span data-ttu-id="d2a06-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="d2a06-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="d2a06-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="d2a06-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="d2a06-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="d2a06-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d2a06-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d2a06-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d2a06-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="d2a06-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="d2a06-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d2a06-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d2a06-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="d2a06-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="d2a06-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="d2a06-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="d2a06-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="d2a06-135">**Error**</span></span> <br/> | <span data-ttu-id="d2a06-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="d2a06-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="d2a06-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="d2a06-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d2a06-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d2a06-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d2a06-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="d2a06-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="d2a06-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="d2a06-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="d2a06-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="d2a06-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="d2a06-142">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="d2a06-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d2a06-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="d2a06-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="d2a06-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="d2a06-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d2a06-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d2a06-145">Child elements</span></span>

|<span data-ttu-id="d2a06-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d2a06-146">**Element**</span></span>|<span data-ttu-id="d2a06-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d2a06-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2a06-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="d2a06-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d2a06-149">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d2a06-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d2a06-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d2a06-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d2a06-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="d2a06-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d2a06-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d2a06-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d2a06-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="d2a06-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d2a06-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="d2a06-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d2a06-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d2a06-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d2a06-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="d2a06-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d2a06-157">Папки</span><span class="sxs-lookup"><span data-stu-id="d2a06-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d2a06-158">Содержит массив созданные управляемые папки.</span><span class="sxs-lookup"><span data-stu-id="d2a06-158">Contains an array of created managed folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2a06-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d2a06-159">Parent elements</span></span>

|<span data-ttu-id="d2a06-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d2a06-160">**Element**</span></span>|<span data-ttu-id="d2a06-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d2a06-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2a06-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d2a06-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d2a06-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2a06-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2a06-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="d2a06-164">Remarks</span></span>

<span data-ttu-id="d2a06-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d2a06-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2a06-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d2a06-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2a06-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d2a06-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d2a06-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d2a06-168">Schema Name</span></span>  <br/> |<span data-ttu-id="d2a06-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d2a06-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d2a06-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d2a06-170">Validation File</span></span>  <br/> |<span data-ttu-id="d2a06-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d2a06-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d2a06-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d2a06-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2a06-173">False</span><span class="sxs-lookup"><span data-stu-id="d2a06-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2a06-174">См. также</span><span class="sxs-lookup"><span data-stu-id="d2a06-174">See also</span></span>

- [<span data-ttu-id="d2a06-175">Операция CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="d2a06-175">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
- [<span data-ttu-id="d2a06-176">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="d2a06-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="d2a06-177">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d2a06-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

