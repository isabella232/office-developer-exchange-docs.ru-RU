---
title: мовефолдерреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolderResponseMessage
api_type:
- schema
ms.assetid: 54917251-96af-44c2-ae90-d545f0a16e2e
description: Элемент Мовефолдерреспонсемессаже содержит состояние и результат одного запроса операции MoveFolder.
ms.openlocfilehash: 634fec89445b49d1c8c42541f2fc50d07b5a1acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467475"
---
# <a name="movefolderresponsemessage"></a><span data-ttu-id="71428-103">мовефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="71428-103">MoveFolderResponseMessage</span></span>

<span data-ttu-id="71428-104">Элемент **мовефолдерреспонсемессаже** содержит состояние и результат одного запроса [операции MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="71428-104">The **MoveFolderResponseMessage** element contains the status and result of a single [MoveFolder operation](movefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="71428-105">мовефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="71428-105">MoveFolderResponse</span></span>](movefolderresponse.md)
- [<span data-ttu-id="71428-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="71428-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="71428-107">мовефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="71428-107">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
  
```xml
<MoveFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</MoveFolderResponseMessage>
```

 <span data-ttu-id="71428-108">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="71428-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71428-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="71428-109">Attributes and elements</span></span>

<span data-ttu-id="71428-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="71428-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71428-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="71428-111">Attributes</span></span>

|<span data-ttu-id="71428-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="71428-112">**Attribute**</span></span>|<span data-ttu-id="71428-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71428-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71428-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="71428-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="71428-115">Описывает состояние ответа [операции MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="71428-115">Describes the status of a [MoveFolder operation](movefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="71428-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="71428-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="71428-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="71428-117">-  Success</span></span>  <br/><span data-ttu-id="71428-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="71428-118">-  Warning</span></span>  <br/><span data-ttu-id="71428-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="71428-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="71428-120">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="71428-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="71428-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="71428-121">**Value**</span></span>|<span data-ttu-id="71428-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71428-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71428-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="71428-123">**Success**</span></span> <br/> |<span data-ttu-id="71428-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="71428-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="71428-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="71428-125">**Warning**</span></span> <br/> | <span data-ttu-id="71428-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="71428-126">Describes a request that was not processed.</span></span> <span data-ttu-id="71428-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="71428-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="71428-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="71428-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="71428-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="71428-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="71428-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="71428-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="71428-131">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="71428-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="71428-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="71428-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="71428-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="71428-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="71428-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="71428-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="71428-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="71428-135">**Error**</span></span> <br/> | <span data-ttu-id="71428-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="71428-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="71428-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="71428-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="71428-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="71428-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="71428-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="71428-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="71428-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="71428-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="71428-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="71428-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="71428-142">— Любой клиент пытается получить любой несанкционированный доступ.</span><span class="sxs-lookup"><span data-stu-id="71428-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="71428-143">— Любой сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="71428-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="71428-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="71428-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="71428-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="71428-145">Child elements</span></span>

|<span data-ttu-id="71428-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71428-146">**Element**</span></span>|<span data-ttu-id="71428-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71428-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71428-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="71428-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="71428-149">Текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="71428-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="71428-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="71428-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="71428-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="71428-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="71428-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="71428-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="71428-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="71428-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="71428-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="71428-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="71428-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="71428-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="71428-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="71428-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="71428-157">Folders</span><span class="sxs-lookup"><span data-stu-id="71428-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="71428-158">Содержит массив перемещенных папок.</span><span class="sxs-lookup"><span data-stu-id="71428-158">Contains an array of moved folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71428-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="71428-159">Parent elements</span></span>

|<span data-ttu-id="71428-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71428-160">**Element**</span></span>|<span data-ttu-id="71428-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71428-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71428-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="71428-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="71428-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="71428-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="71428-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="71428-164">Remarks</span></span>

<span data-ttu-id="71428-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="71428-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71428-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="71428-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71428-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="71428-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="71428-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="71428-168">Schema Name</span></span>  <br/> |<span data-ttu-id="71428-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="71428-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="71428-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="71428-170">Validation File</span></span>  <br/> |<span data-ttu-id="71428-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="71428-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="71428-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="71428-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="71428-173">False</span><span class="sxs-lookup"><span data-stu-id="71428-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71428-174">См. также</span><span class="sxs-lookup"><span data-stu-id="71428-174">See also</span></span>

- [<span data-ttu-id="71428-175">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="71428-175">MoveFolder</span></span>](movefolder.md)
- [<span data-ttu-id="71428-176">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="71428-176">MoveFolder operation</span></span>](movefolder-operation.md)

