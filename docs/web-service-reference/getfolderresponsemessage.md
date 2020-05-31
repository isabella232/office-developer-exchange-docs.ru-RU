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
ms.openlocfilehash: a6b67907dba311a3ce482ff8f524378fb4be9694
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762798"
---
# <a name="getfolderresponsemessage"></a><span data-ttu-id="11d05-103">жетфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="11d05-103">GetFolderResponseMessage</span></span>

<span data-ttu-id="11d05-104">Элемент **жетфолдерреспонсемессаже** содержит состояние и результат запроса операции получения одного [каталога](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="11d05-104">The **GetFolderResponseMessage** element contains the status and result of a single [GetFolder operation](getfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="11d05-105">жетфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="11d05-105">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="11d05-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="11d05-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="11d05-107">жетфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="11d05-107">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
  
```xml
<GetFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</GetFolderResponseMessage>
```

 <span data-ttu-id="11d05-108">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="11d05-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11d05-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="11d05-109">Attributes and elements</span></span>

<span data-ttu-id="11d05-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="11d05-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11d05-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="11d05-111">Attributes</span></span>

|<span data-ttu-id="11d05-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="11d05-112">**Attribute**</span></span>|<span data-ttu-id="11d05-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11d05-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="11d05-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="11d05-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="11d05-115">Описывает состояние ответа операции " [операция с папкой](getfolder-operation.md) ".</span><span class="sxs-lookup"><span data-stu-id="11d05-115">Describes the status of a [GetFolder operation](getfolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="11d05-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="11d05-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="11d05-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="11d05-117">-  Success</span></span>  <br/><span data-ttu-id="11d05-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="11d05-118">-  Warning</span></span>  <br/><span data-ttu-id="11d05-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="11d05-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="11d05-120">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="11d05-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="11d05-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="11d05-121">**Value**</span></span>|<span data-ttu-id="11d05-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11d05-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="11d05-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="11d05-123">**Success**</span></span> <br/> |<span data-ttu-id="11d05-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="11d05-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="11d05-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="11d05-125">**Warning**</span></span> <br/> | <span data-ttu-id="11d05-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="11d05-126">Describes a request that was not processed.</span></span> <span data-ttu-id="11d05-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="11d05-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="11d05-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="11d05-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="11d05-129">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="11d05-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="11d05-130">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="11d05-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="11d05-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="11d05-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="11d05-132">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="11d05-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="11d05-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="11d05-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="11d05-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="11d05-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="11d05-135">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="11d05-135">**Error**</span></span> <br/> | <span data-ttu-id="11d05-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="11d05-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="11d05-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="11d05-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="11d05-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="11d05-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="11d05-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="11d05-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="11d05-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="11d05-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="11d05-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="11d05-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="11d05-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="11d05-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="11d05-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="11d05-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="11d05-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="11d05-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="11d05-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="11d05-145">Child elements</span></span>

|<span data-ttu-id="11d05-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="11d05-146">**Element**</span></span>|<span data-ttu-id="11d05-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11d05-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11d05-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="11d05-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="11d05-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="11d05-149">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="11d05-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="11d05-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="11d05-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="11d05-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="11d05-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="11d05-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="11d05-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="11d05-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="11d05-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="11d05-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="11d05-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="11d05-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="11d05-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="11d05-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="11d05-157">Folders</span><span class="sxs-lookup"><span data-stu-id="11d05-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="11d05-158">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="11d05-158">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11d05-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="11d05-159">Parent elements</span></span>

|<span data-ttu-id="11d05-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="11d05-160">**Element**</span></span>|<span data-ttu-id="11d05-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11d05-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11d05-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="11d05-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="11d05-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="11d05-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="11d05-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="11d05-164">Remarks</span></span>

<span data-ttu-id="11d05-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="11d05-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11d05-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="11d05-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11d05-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="11d05-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="11d05-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="11d05-168">Schema Name</span></span>  <br/> |<span data-ttu-id="11d05-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="11d05-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="11d05-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="11d05-170">Validation File</span></span>  <br/> |<span data-ttu-id="11d05-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="11d05-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="11d05-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="11d05-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="11d05-173">False</span><span class="sxs-lookup"><span data-stu-id="11d05-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11d05-174">См. также</span><span class="sxs-lookup"><span data-stu-id="11d05-174">See also</span></span>

- [<span data-ttu-id="11d05-175">GetFolder</span><span class="sxs-lookup"><span data-stu-id="11d05-175">GetFolder</span></span>](getfolder.md)
- [<span data-ttu-id="11d05-176">жетфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="11d05-176">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="11d05-177">Операция GetFolder</span><span class="sxs-lookup"><span data-stu-id="11d05-177">GetFolder operation</span></span>](getfolder-operation.md)

