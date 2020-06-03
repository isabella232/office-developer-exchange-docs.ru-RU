---
title: жетфолдерреспонсемессаже
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
description: Элемент Жетфолдерреспонсемессаже содержит состояние и результат запроса операции получения одного каталога.
ms.openlocfilehash: ddf23790e804c3f0562f65ebaa3cb591433eab69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456460"
---
# <a name="getfolderresponsemessage"></a><span data-ttu-id="ff7ea-103">жетфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ff7ea-103">GetFolderResponseMessage</span></span>

<span data-ttu-id="ff7ea-104">Элемент **жетфолдерреспонсемессаже** содержит состояние и результат запроса операции получения одного [каталога](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ff7ea-104">The **GetFolderResponseMessage** element contains the status and result of a single [GetFolder operation](getfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="ff7ea-105">жетфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="ff7ea-105">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="ff7ea-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="ff7ea-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="ff7ea-107">жетфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ff7ea-107">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
  
```xml
<GetFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</GetFolderResponseMessage>
```

 <span data-ttu-id="ff7ea-108">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff7ea-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ff7ea-109">Attributes and elements</span></span>

<span data-ttu-id="ff7ea-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff7ea-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ff7ea-111">Attributes</span></span>

|<span data-ttu-id="ff7ea-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-112">**Attribute**</span></span>|<span data-ttu-id="ff7ea-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ff7ea-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ff7ea-115">Описывает состояние ответа операции " [операция с папкой](getfolder-operation.md) ".</span><span class="sxs-lookup"><span data-stu-id="ff7ea-115">Describes the status of a [GetFolder operation](getfolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="ff7ea-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="ff7ea-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="ff7ea-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="ff7ea-117">-  Success</span></span>  <br/><span data-ttu-id="ff7ea-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="ff7ea-118">-  Warning</span></span>  <br/><span data-ttu-id="ff7ea-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="ff7ea-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="ff7ea-120">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="ff7ea-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="ff7ea-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-121">**Value**</span></span>|<span data-ttu-id="ff7ea-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ff7ea-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-123">**Success**</span></span> <br/> |<span data-ttu-id="ff7ea-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ff7ea-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-125">**Warning**</span></span> <br/> | <span data-ttu-id="ff7ea-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-126">Describes a request that was not processed.</span></span> <span data-ttu-id="ff7ea-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="ff7ea-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="ff7ea-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="ff7ea-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="ff7ea-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="ff7ea-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="ff7ea-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="ff7ea-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="ff7ea-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-135">**Error**</span></span> <br/> | <span data-ttu-id="ff7ea-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="ff7ea-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="ff7ea-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="ff7ea-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ff7ea-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="ff7ea-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="ff7ea-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="ff7ea-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="ff7ea-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="ff7ea-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="ff7ea-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="ff7ea-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="ff7ea-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="ff7ea-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="ff7ea-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="ff7ea-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ff7ea-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ff7ea-145">Child elements</span></span>

|<span data-ttu-id="ff7ea-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-146">**Element**</span></span>|<span data-ttu-id="ff7ea-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff7ea-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="ff7ea-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ff7ea-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-149">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ff7ea-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="ff7ea-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ff7ea-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ff7ea-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="ff7ea-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ff7ea-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="ff7ea-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ff7ea-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="ff7ea-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ff7ea-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ff7ea-157">Folders</span><span class="sxs-lookup"><span data-stu-id="ff7ea-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ff7ea-158">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-158">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff7ea-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ff7ea-159">Parent elements</span></span>

|<span data-ttu-id="ff7ea-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-160">**Element**</span></span>|<span data-ttu-id="ff7ea-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ff7ea-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff7ea-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="ff7ea-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ff7ea-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ff7ea-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="ff7ea-164">Remarks</span></span>

<span data-ttu-id="ff7ea-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ff7ea-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff7ea-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ff7ea-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff7ea-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ff7ea-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff7ea-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ff7ea-168">Schema Name</span></span>  <br/> |<span data-ttu-id="ff7ea-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ff7ea-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff7ea-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ff7ea-170">Validation File</span></span>  <br/> |<span data-ttu-id="ff7ea-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ff7ea-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff7ea-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ff7ea-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff7ea-173">False</span><span class="sxs-lookup"><span data-stu-id="ff7ea-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff7ea-174">См. также</span><span class="sxs-lookup"><span data-stu-id="ff7ea-174">See also</span></span>

- [<span data-ttu-id="ff7ea-175">GetFolder</span><span class="sxs-lookup"><span data-stu-id="ff7ea-175">GetFolder</span></span>](getfolder.md)
- [<span data-ttu-id="ff7ea-176">жетфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="ff7ea-176">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="ff7ea-177">Операция GetFolder</span><span class="sxs-lookup"><span data-stu-id="ff7ea-177">GetFolder operation</span></span>](getfolder-operation.md)

