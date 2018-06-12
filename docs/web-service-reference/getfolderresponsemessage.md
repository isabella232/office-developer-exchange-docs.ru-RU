---
title: GetFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolderResponseMessage
api_type:
- schema
ms.assetid: 51359863-d110-4c12-b89f-aba5e3e40c1d
description: Элемент GetFolderResponseMessage содержит состояние и результат одного запроса GetFolder операции.
ms.openlocfilehash: a6b67907dba311a3ce482ff8f524378fb4be9694
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762798"
---
# <a name="getfolderresponsemessage"></a><span data-ttu-id="4fff5-103">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4fff5-103">GetFolderResponseMessage</span></span>

<span data-ttu-id="4fff5-104">Элемент **GetFolderResponseMessage** содержит состояние и результат одного запроса [GetFolder операции](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4fff5-104">The **GetFolderResponseMessage** element contains the status and result of a single [GetFolder operation](getfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="4fff5-105">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="4fff5-105">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="4fff5-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4fff5-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="4fff5-107">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4fff5-107">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
  
```xml
<GetFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</GetFolderResponseMessage>
```

 <span data-ttu-id="4fff5-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4fff5-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fff5-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4fff5-109">Attributes and elements</span></span>

<span data-ttu-id="4fff5-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4fff5-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fff5-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4fff5-111">Attributes</span></span>

|<span data-ttu-id="4fff5-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4fff5-112">**Attribute**</span></span>|<span data-ttu-id="4fff5-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4fff5-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4fff5-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4fff5-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4fff5-115">Описание состояния ответа [GetFolder операции](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4fff5-115">Describes the status of a [GetFolder operation](getfolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="4fff5-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="4fff5-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="4fff5-117">-Success</span><span class="sxs-lookup"><span data-stu-id="4fff5-117">-  Success</span></span>  <br/><span data-ttu-id="4fff5-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="4fff5-118">-  Warning</span></span>  <br/><span data-ttu-id="4fff5-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="4fff5-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="4fff5-120">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="4fff5-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="4fff5-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4fff5-121">**Value**</span></span>|<span data-ttu-id="4fff5-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4fff5-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4fff5-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="4fff5-123">**Success**</span></span> <br/> |<span data-ttu-id="4fff5-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="4fff5-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4fff5-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="4fff5-125">**Warning**</span></span> <br/> | <span data-ttu-id="4fff5-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="4fff5-126">Describes a request that was not processed.</span></span> <span data-ttu-id="4fff5-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="4fff5-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="4fff5-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="4fff5-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="4fff5-129">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="4fff5-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="4fff5-130">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4fff5-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4fff5-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="4fff5-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="4fff5-132">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4fff5-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="4fff5-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="4fff5-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="4fff5-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="4fff5-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="4fff5-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="4fff5-135">**Error**</span></span> <br/> | <span data-ttu-id="4fff5-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="4fff5-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4fff5-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="4fff5-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4fff5-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4fff5-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4fff5-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="4fff5-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="4fff5-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="4fff5-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="4fff5-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="4fff5-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="4fff5-142">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="4fff5-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4fff5-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="4fff5-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="4fff5-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="4fff5-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4fff5-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4fff5-145">Child elements</span></span>

|<span data-ttu-id="4fff5-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4fff5-146">**Element**</span></span>|<span data-ttu-id="4fff5-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4fff5-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fff5-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="4fff5-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4fff5-149">Текст с описанием состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="4fff5-149">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4fff5-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4fff5-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4fff5-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="4fff5-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4fff5-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4fff5-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4fff5-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="4fff5-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4fff5-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="4fff5-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4fff5-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4fff5-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4fff5-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="4fff5-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4fff5-157">Папки</span><span class="sxs-lookup"><span data-stu-id="4fff5-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4fff5-158">Содержит набор папок, используемых в операциях папки.</span><span class="sxs-lookup"><span data-stu-id="4fff5-158">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4fff5-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4fff5-159">Parent elements</span></span>

|<span data-ttu-id="4fff5-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4fff5-160">**Element**</span></span>|<span data-ttu-id="4fff5-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4fff5-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fff5-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4fff5-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4fff5-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fff5-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4fff5-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="4fff5-164">Remarks</span></span>

<span data-ttu-id="4fff5-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4fff5-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fff5-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4fff5-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fff5-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4fff5-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4fff5-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4fff5-168">Schema Name</span></span>  <br/> |<span data-ttu-id="4fff5-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4fff5-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4fff5-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4fff5-170">Validation File</span></span>  <br/> |<span data-ttu-id="4fff5-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4fff5-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4fff5-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4fff5-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="4fff5-173">False</span><span class="sxs-lookup"><span data-stu-id="4fff5-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fff5-174">См. также</span><span class="sxs-lookup"><span data-stu-id="4fff5-174">See also</span></span>

- [<span data-ttu-id="4fff5-175">GetFolder</span><span class="sxs-lookup"><span data-stu-id="4fff5-175">GetFolder</span></span>](getfolder.md)
- [<span data-ttu-id="4fff5-176">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="4fff5-176">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="4fff5-177">GetFolder Operation</span><span class="sxs-lookup"><span data-stu-id="4fff5-177">GetFolder operation</span></span>](getfolder-operation.md)

