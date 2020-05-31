---
title: упдатефолдерреспонсемессаже
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
description: Элемент Упдатефолдерреспонсемессаже содержит состояние и результат обновлений, определенных элементом Фолдерчанже запроса операции операцию UpdateFolder.
ms.openlocfilehash: 4cd00232bcc233f6534d844418f523c248ce54bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840340"
---
# <a name="updatefolderresponsemessage"></a><span data-ttu-id="4ce9c-103">упдатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="4ce9c-103">UpdateFolderResponseMessage</span></span>

<span data-ttu-id="4ce9c-104">Элемент **упдатефолдерреспонсемессаже** содержит состояние и результат обновлений, определенных элементом [Фолдерчанже](folderchange.md) запроса [операции операцию UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4ce9c-104">The **UpdateFolderResponseMessage** element contains the status and result of updates defined by the [FolderChange](folderchange.md) element of an [UpdateFolder operation](updatefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="4ce9c-105">упдатефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="4ce9c-105">UpdateFolderResponse</span></span>](updatefolderresponse.md) 
- [<span data-ttu-id="4ce9c-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="4ce9c-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="4ce9c-107">упдатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="4ce9c-107">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
  
```xml
<UpdateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</UpdateFolderResponseMessage>
```

 <span data-ttu-id="4ce9c-108">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ce9c-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4ce9c-109">Attributes and elements</span></span>

<span data-ttu-id="4ce9c-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ce9c-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4ce9c-111">Attributes</span></span>

|<span data-ttu-id="4ce9c-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-112">**Attribute**</span></span>|<span data-ttu-id="4ce9c-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4ce9c-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4ce9c-115">Описывает состояние ответа [операции операцию UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4ce9c-115">Describes the status of an [UpdateFolder operation](updatefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="4ce9c-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="4ce9c-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="4ce9c-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="4ce9c-117">-  Success</span></span>  <br/><span data-ttu-id="4ce9c-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="4ce9c-118">-  Warning</span></span>  <br/><span data-ttu-id="4ce9c-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="4ce9c-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4ce9c-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="4ce9c-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="4ce9c-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-121">**Value**</span></span>|<span data-ttu-id="4ce9c-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4ce9c-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-123">**Success**</span></span> <br/> |<span data-ttu-id="4ce9c-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4ce9c-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-125">**Warning**</span></span> <br/> | <span data-ttu-id="4ce9c-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-126">Describes a request that was not processed.</span></span> <span data-ttu-id="4ce9c-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="4ce9c-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="4ce9c-129">— Хранилище Exchange находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-129">-  The Exchange store is offline.</span></span>  <br/><span data-ttu-id="4ce9c-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4ce9c-131">— Почтовый ящик перемещается.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-131">-  A mailbox is moved.</span></span>  <br/><span data-ttu-id="4ce9c-132">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="4ce9c-133">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-133">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="4ce9c-134">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-134">**Error**</span></span> <br/> | <span data-ttu-id="4ce9c-135">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4ce9c-136">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-136">The following are examples of sources for errors:</span></span>  <br/><br/><span data-ttu-id="4ce9c-137">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="4ce9c-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4ce9c-138">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="4ce9c-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="4ce9c-139">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="4ce9c-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="4ce9c-140">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="4ce9c-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="4ce9c-141">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="4ce9c-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4ce9c-142">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="4ce9c-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="4ce9c-143">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="4ce9c-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4ce9c-144">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4ce9c-144">Child elements</span></span>

|<span data-ttu-id="4ce9c-145">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-145">**Element**</span></span>|<span data-ttu-id="4ce9c-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ce9c-147">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="4ce9c-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4ce9c-148">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4ce9c-149">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="4ce9c-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4ce9c-150">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4ce9c-151">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="4ce9c-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4ce9c-152">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-152">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4ce9c-153">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-153">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4ce9c-154">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="4ce9c-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4ce9c-155">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4ce9c-156">Folders</span><span class="sxs-lookup"><span data-stu-id="4ce9c-156">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4ce9c-157">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-157">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ce9c-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4ce9c-158">Parent elements</span></span>

|<span data-ttu-id="4ce9c-159">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-159">**Element**</span></span>|<span data-ttu-id="4ce9c-160">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ce9c-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ce9c-161">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="4ce9c-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4ce9c-162">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4ce9c-163">Примечания</span><span class="sxs-lookup"><span data-stu-id="4ce9c-163">Remarks</span></span>

<span data-ttu-id="4ce9c-164">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4ce9c-164">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ce9c-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4ce9c-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ce9c-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4ce9c-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ce9c-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4ce9c-167">Schema Name</span></span>  <br/> |<span data-ttu-id="4ce9c-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4ce9c-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4ce9c-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4ce9c-169">Validation File</span></span>  <br/> |<span data-ttu-id="4ce9c-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4ce9c-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ce9c-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4ce9c-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ce9c-172">False</span><span class="sxs-lookup"><span data-stu-id="4ce9c-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ce9c-173">См. также</span><span class="sxs-lookup"><span data-stu-id="4ce9c-173">See also</span></span>

- [<span data-ttu-id="4ce9c-174">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="4ce9c-174">UpdateFolder operation</span></span>](updatefolder-operation.md)

