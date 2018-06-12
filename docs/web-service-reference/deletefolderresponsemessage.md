---
title: DeleteFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderResponseMessage
api_type:
- schema
ms.assetid: de4c63ff-80b2-40c2-bc06-ef0c23beacd4
description: Элемент DeleteFolderResponseMessage содержит состояние и результат одного запроса DeleteFolder операции.
ms.openlocfilehash: 5601fe2e48ad002e0fab60d812e7d70c7398f3ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762038"
---
# <a name="deletefolderresponsemessage"></a><span data-ttu-id="02213-103">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="02213-103">DeleteFolderResponseMessage</span></span>

<span data-ttu-id="02213-104">Элемент **DeleteFolderResponseMessage** содержит состояние и результат одного запроса [DeleteFolder операции](deletefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="02213-104">The **DeleteFolderResponseMessage** element contains the status and result of a single [DeleteFolder operation](deletefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="02213-105">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="02213-105">DeleteFolderResponse</span></span>](deletefolderresponse.md)  
- [<span data-ttu-id="02213-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="02213-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="02213-107">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="02213-107">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
  
```xml
<DeleteFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteFolderResponseMessage>
```

 <span data-ttu-id="02213-108">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="02213-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02213-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02213-109">Attributes and elements</span></span>

<span data-ttu-id="02213-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="02213-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02213-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="02213-111">Attributes</span></span>

|<span data-ttu-id="02213-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="02213-112">**Attribute**</span></span>|<span data-ttu-id="02213-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02213-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="02213-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="02213-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="02213-115">Описание состояния ответа [операции DeleteFolder](deletefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="02213-115">Describes the status of a [DeleteFolder operation](deletefolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="02213-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="02213-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="02213-117">-Success</span><span class="sxs-lookup"><span data-stu-id="02213-117">-  Success</span></span>  <br/><span data-ttu-id="02213-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="02213-118">-  Warning</span></span>  <br/><span data-ttu-id="02213-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="02213-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="02213-120">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="02213-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="02213-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="02213-121">**Value**</span></span>|<span data-ttu-id="02213-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02213-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="02213-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="02213-123">**Success**</span></span> <br/> |<span data-ttu-id="02213-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="02213-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="02213-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="02213-125">**Warning**</span></span> <br/> | <span data-ttu-id="02213-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="02213-126">Describes a request that was not processed.</span></span> <span data-ttu-id="02213-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="02213-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="02213-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="02213-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="02213-129">-В хранилище Exchange переходит в автономный режим во время пакета.</span><span class="sxs-lookup"><span data-stu-id="02213-129">- The Exchange store goes offline during the batch.</span></span><br/><span data-ttu-id="02213-130">-Доменных служб active Directory (AD DS) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="02213-130">- Active Directory Domain Services (AD DS) goes offline.</span></span><br/><span data-ttu-id="02213-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="02213-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="02213-132">-База данных сообщений (MDB) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="02213-132">- The message database (MDB) goes offline.</span></span><br/><span data-ttu-id="02213-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="02213-133">- A password is expired.</span></span><br/><span data-ttu-id="02213-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="02213-134">- A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="02213-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="02213-135">**Error**</span></span> <br/> | <span data-ttu-id="02213-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="02213-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="02213-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="02213-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="02213-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02213-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="02213-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="02213-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="02213-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="02213-140">- Unknown tag</span></span><br/><span data-ttu-id="02213-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="02213-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="02213-142">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="02213-142">- Unauthorized access attempt by any client</span></span><br/><span data-ttu-id="02213-143">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="02213-143">- Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="02213-144">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="02213-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="02213-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="02213-145">Child elements</span></span>

|<span data-ttu-id="02213-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="02213-146">**Element**</span></span>|<span data-ttu-id="02213-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02213-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02213-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="02213-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="02213-149">Текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="02213-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="02213-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="02213-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="02213-151">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="02213-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="02213-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="02213-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="02213-153">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="02213-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="02213-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="02213-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="02213-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="02213-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="02213-156">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="02213-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02213-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="02213-157">Parent elements</span></span>

|<span data-ttu-id="02213-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="02213-158">**Element**</span></span>|<span data-ttu-id="02213-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02213-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02213-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="02213-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="02213-161">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="02213-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="02213-162">Замечания</span><span class="sxs-lookup"><span data-stu-id="02213-162">Remarks</span></span>

<span data-ttu-id="02213-163">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="02213-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02213-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="02213-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02213-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="02213-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="02213-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="02213-166">Schema Name</span></span>  <br/> |<span data-ttu-id="02213-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="02213-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="02213-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="02213-168">Validation File</span></span>  <br/> |<span data-ttu-id="02213-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="02213-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02213-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="02213-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="02213-171">False</span><span class="sxs-lookup"><span data-stu-id="02213-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02213-172">См. также</span><span class="sxs-lookup"><span data-stu-id="02213-172">See also</span></span>

- [<span data-ttu-id="02213-173">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="02213-173">DeleteFolder operation</span></span>](deletefolder-operation.md)
- [<span data-ttu-id="02213-174">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="02213-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="02213-175">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="02213-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="02213-176">Удаление папок</span><span class="sxs-lookup"><span data-stu-id="02213-176">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)
