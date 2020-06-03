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
ms.openlocfilehash: bbe01583072e6203e099d440f2a171012f51e7df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466586"
---
# <a name="updatefolderresponsemessage"></a><span data-ttu-id="38c86-103">упдатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="38c86-103">UpdateFolderResponseMessage</span></span>

<span data-ttu-id="38c86-104">Элемент **упдатефолдерреспонсемессаже** содержит состояние и результат обновлений, определенных элементом [Фолдерчанже](folderchange.md) запроса [операции операцию UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="38c86-104">The **UpdateFolderResponseMessage** element contains the status and result of updates defined by the [FolderChange](folderchange.md) element of an [UpdateFolder operation](updatefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="38c86-105">упдатефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="38c86-105">UpdateFolderResponse</span></span>](updatefolderresponse.md) 
- [<span data-ttu-id="38c86-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="38c86-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="38c86-107">упдатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="38c86-107">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
  
```xml
<UpdateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</UpdateFolderResponseMessage>
```

 <span data-ttu-id="38c86-108">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="38c86-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38c86-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="38c86-109">Attributes and elements</span></span>

<span data-ttu-id="38c86-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="38c86-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38c86-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="38c86-111">Attributes</span></span>

|<span data-ttu-id="38c86-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="38c86-112">**Attribute**</span></span>|<span data-ttu-id="38c86-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38c86-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="38c86-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="38c86-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="38c86-115">Описывает состояние ответа [операции операцию UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="38c86-115">Describes the status of an [UpdateFolder operation](updatefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="38c86-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="38c86-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="38c86-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="38c86-117">-  Success</span></span>  <br/><span data-ttu-id="38c86-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="38c86-118">-  Warning</span></span>  <br/><span data-ttu-id="38c86-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="38c86-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="38c86-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="38c86-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="38c86-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="38c86-121">**Value**</span></span>|<span data-ttu-id="38c86-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38c86-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="38c86-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="38c86-123">**Success**</span></span> <br/> |<span data-ttu-id="38c86-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="38c86-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="38c86-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="38c86-125">**Warning**</span></span> <br/> | <span data-ttu-id="38c86-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="38c86-126">Describes a request that was not processed.</span></span> <span data-ttu-id="38c86-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="38c86-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="38c86-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="38c86-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="38c86-129">— Хранилище Exchange находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="38c86-129">-  The Exchange store is offline.</span></span>  <br/><span data-ttu-id="38c86-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="38c86-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="38c86-131">— Почтовый ящик перемещается.</span><span class="sxs-lookup"><span data-stu-id="38c86-131">-  A mailbox is moved.</span></span>  <br/><span data-ttu-id="38c86-132">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="38c86-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="38c86-133">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="38c86-133">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="38c86-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="38c86-134">**Error**</span></span> <br/> | <span data-ttu-id="38c86-135">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="38c86-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="38c86-136">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="38c86-136">The following are examples of sources for errors:</span></span>  <br/><br/><span data-ttu-id="38c86-137">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="38c86-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="38c86-138">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="38c86-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="38c86-139">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="38c86-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="38c86-140">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="38c86-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="38c86-141">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="38c86-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="38c86-142">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="38c86-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="38c86-143">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="38c86-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="38c86-144">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="38c86-144">Child elements</span></span>

|<span data-ttu-id="38c86-145">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="38c86-145">**Element**</span></span>|<span data-ttu-id="38c86-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38c86-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38c86-147">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="38c86-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="38c86-148">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="38c86-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="38c86-149">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="38c86-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="38c86-150">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="38c86-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="38c86-151">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="38c86-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="38c86-152">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="38c86-152">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="38c86-153">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="38c86-153">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="38c86-154">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="38c86-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="38c86-155">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="38c86-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="38c86-156">Folders</span><span class="sxs-lookup"><span data-stu-id="38c86-156">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="38c86-157">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="38c86-157">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38c86-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="38c86-158">Parent elements</span></span>

|<span data-ttu-id="38c86-159">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="38c86-159">**Element**</span></span>|<span data-ttu-id="38c86-160">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38c86-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38c86-161">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="38c86-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="38c86-162">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="38c86-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="38c86-163">Примечания</span><span class="sxs-lookup"><span data-stu-id="38c86-163">Remarks</span></span>

<span data-ttu-id="38c86-164">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="38c86-164">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38c86-165">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="38c86-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38c86-166">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="38c86-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="38c86-167">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="38c86-167">Schema Name</span></span>  <br/> |<span data-ttu-id="38c86-168">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="38c86-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="38c86-169">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="38c86-169">Validation File</span></span>  <br/> |<span data-ttu-id="38c86-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="38c86-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="38c86-171">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="38c86-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="38c86-172">False</span><span class="sxs-lookup"><span data-stu-id="38c86-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38c86-173">См. также</span><span class="sxs-lookup"><span data-stu-id="38c86-173">See also</span></span>

- [<span data-ttu-id="38c86-174">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="38c86-174">UpdateFolder operation</span></span>](updatefolder-operation.md)

