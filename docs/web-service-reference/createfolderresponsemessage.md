---
title: креатефолдерреспонсемессаже
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
description: Элемент Креатефолдерреспонсемессаже содержит состояние и результат одного запроса операции CreateFolder.
ms.openlocfilehash: c587cca1f935b295a0ed30ab2210de40af28d06d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761884"
---
# <a name="createfolderresponsemessage"></a><span data-ttu-id="87da6-103">креатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="87da6-103">CreateFolderResponseMessage</span></span>

<span data-ttu-id="87da6-104">Элемент **креатефолдерреспонсемессаже** содержит состояние и результат одного запроса [операции CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="87da6-104">The **CreateFolderResponseMessage** element contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span> 
  
```xml
<CreateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateFolderResponseMessage>
```

<span data-ttu-id="87da6-105">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="87da6-105">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="87da6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="87da6-106">Attributes and elements</span></span>

<span data-ttu-id="87da6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="87da6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87da6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="87da6-108">Attributes</span></span>

|<span data-ttu-id="87da6-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="87da6-109">**Attribute**</span></span>|<span data-ttu-id="87da6-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="87da6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="87da6-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="87da6-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="87da6-112">Описывает состояние ответа [операции CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="87da6-112">Describes the status of a [CreateFolder operation](createfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="87da6-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="87da6-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="87da6-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="87da6-114">-  Success</span></span>  <br/><span data-ttu-id="87da6-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="87da6-115">-  Warning</span></span>  <br/><span data-ttu-id="87da6-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="87da6-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="87da6-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="87da6-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="87da6-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="87da6-118">**Value**</span></span>|<span data-ttu-id="87da6-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="87da6-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="87da6-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="87da6-120">**Success**</span></span> <br/> |<span data-ttu-id="87da6-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="87da6-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="87da6-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="87da6-122">**Warning**</span></span> <br/> | <span data-ttu-id="87da6-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="87da6-123">Describes a request that was not processed.</span></span> <span data-ttu-id="87da6-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="87da6-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="87da6-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="87da6-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="87da6-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="87da6-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="87da6-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="87da6-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="87da6-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="87da6-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="87da6-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="87da6-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="87da6-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="87da6-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="87da6-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="87da6-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="87da6-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="87da6-132">**Error**</span></span> <br/> | <span data-ttu-id="87da6-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="87da6-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="87da6-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="87da6-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="87da6-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="87da6-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="87da6-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="87da6-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="87da6-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="87da6-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="87da6-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="87da6-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="87da6-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="87da6-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="87da6-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="87da6-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="87da6-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="87da6-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="87da6-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="87da6-142">Child elements</span></span>

|<span data-ttu-id="87da6-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="87da6-143">**Element**</span></span>|<span data-ttu-id="87da6-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="87da6-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87da6-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="87da6-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="87da6-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="87da6-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="87da6-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="87da6-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="87da6-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="87da6-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="87da6-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="87da6-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="87da6-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="87da6-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="87da6-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="87da6-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="87da6-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="87da6-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="87da6-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="87da6-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="87da6-154">Folders</span><span class="sxs-lookup"><span data-stu-id="87da6-154">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="87da6-155">Содержит массив созданных папок.</span><span class="sxs-lookup"><span data-stu-id="87da6-155">Contains an array of created folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="87da6-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="87da6-156">Parent elements</span></span>

|<span data-ttu-id="87da6-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="87da6-157">**Element**</span></span>|<span data-ttu-id="87da6-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="87da6-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87da6-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="87da6-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="87da6-160">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="87da6-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="87da6-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="87da6-161">Remarks</span></span>

<span data-ttu-id="87da6-162">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="87da6-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87da6-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="87da6-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87da6-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="87da6-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="87da6-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="87da6-165">Schema Name</span></span>  <br/> |<span data-ttu-id="87da6-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="87da6-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="87da6-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="87da6-167">Validation File</span></span>  <br/> |<span data-ttu-id="87da6-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="87da6-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="87da6-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="87da6-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="87da6-170">False</span><span class="sxs-lookup"><span data-stu-id="87da6-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87da6-171">См. также</span><span class="sxs-lookup"><span data-stu-id="87da6-171">See also</span></span>

- [<span data-ttu-id="87da6-172">Операция CreateFolder</span><span class="sxs-lookup"><span data-stu-id="87da6-172">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="87da6-173">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="87da6-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="87da6-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="87da6-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

