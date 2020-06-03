---
title: креатеманажедфолдерреспонсемессаже
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
description: Элемент Креатеманажедфолдерреспонсемессаже содержит состояние и результат одного запроса операции CreateManagedFolder.
ms.openlocfilehash: 03ebcaeb79b2fac20882d2cea3d1e24b42dd472f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467706"
---
# <a name="createmanagedfolderresponsemessage"></a><span data-ttu-id="e7799-103">креатеманажедфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="e7799-103">CreateManagedFolderResponseMessage</span></span>

<span data-ttu-id="e7799-104">Элемент **креатеманажедфолдерреспонсемессаже** содержит состояние и результат одного запроса [операции CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e7799-104">The **CreateManagedFolderResponseMessage** element contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="e7799-105">креатеманажедфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="e7799-105">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)  
- [<span data-ttu-id="e7799-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="e7799-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="e7799-107">креатеманажедфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="e7799-107">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
  
```xml
<CreateManagedFolderResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateManagedFolderResponseMessage>
```

<span data-ttu-id="e7799-108">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e7799-108">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e7799-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e7799-109">Attributes and elements</span></span>

<span data-ttu-id="e7799-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e7799-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7799-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e7799-111">Attributes</span></span>

|<span data-ttu-id="e7799-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e7799-112">**Attribute**</span></span>|<span data-ttu-id="e7799-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7799-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7799-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="e7799-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e7799-115">Описывает состояние ответа [операции CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e7799-115">Describes the status of a [CreateManagedFolder operation](createmanagedfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="e7799-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="e7799-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="e7799-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="e7799-117">-  Success</span></span>  <br/><span data-ttu-id="e7799-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="e7799-118">-  Warning</span></span>  <br/><span data-ttu-id="e7799-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="e7799-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="e7799-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="e7799-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="e7799-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e7799-121">**Value**</span></span>|<span data-ttu-id="e7799-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7799-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7799-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="e7799-123">**Success**</span></span> <br/> |<span data-ttu-id="e7799-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="e7799-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e7799-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="e7799-125">**Warning**</span></span> <br/> | <span data-ttu-id="e7799-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="e7799-126">Describes a request that was not processed.</span></span> <span data-ttu-id="e7799-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="e7799-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="e7799-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="e7799-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="e7799-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="e7799-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="e7799-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="e7799-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="e7799-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="e7799-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="e7799-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="e7799-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="e7799-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="e7799-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="e7799-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="e7799-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="e7799-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="e7799-135">**Error**</span></span> <br/> | <span data-ttu-id="e7799-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="e7799-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="e7799-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="e7799-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e7799-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="e7799-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e7799-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="e7799-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="e7799-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="e7799-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="e7799-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="e7799-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="e7799-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="e7799-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="e7799-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="e7799-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="e7799-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e7799-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e7799-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e7799-145">Child elements</span></span>

|<span data-ttu-id="e7799-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e7799-146">**Element**</span></span>|<span data-ttu-id="e7799-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7799-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7799-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="e7799-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e7799-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="e7799-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e7799-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="e7799-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e7799-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="e7799-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e7799-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="e7799-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e7799-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="e7799-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e7799-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="e7799-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e7799-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="e7799-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e7799-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e7799-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e7799-157">Folders</span><span class="sxs-lookup"><span data-stu-id="e7799-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e7799-158">Содержит массив созданных управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="e7799-158">Contains an array of created managed folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7799-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e7799-159">Parent elements</span></span>

|<span data-ttu-id="e7799-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e7799-160">**Element**</span></span>|<span data-ttu-id="e7799-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e7799-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7799-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="e7799-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e7799-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7799-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e7799-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="e7799-164">Remarks</span></span>

<span data-ttu-id="e7799-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e7799-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7799-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e7799-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7799-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e7799-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e7799-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e7799-168">Schema Name</span></span>  <br/> |<span data-ttu-id="e7799-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e7799-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e7799-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e7799-170">Validation File</span></span>  <br/> |<span data-ttu-id="e7799-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e7799-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e7799-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e7799-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7799-173">False</span><span class="sxs-lookup"><span data-stu-id="e7799-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7799-174">См. также</span><span class="sxs-lookup"><span data-stu-id="e7799-174">See also</span></span>

- [<span data-ttu-id="e7799-175">Операция CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="e7799-175">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
- [<span data-ttu-id="e7799-176">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="e7799-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="e7799-177">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e7799-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

