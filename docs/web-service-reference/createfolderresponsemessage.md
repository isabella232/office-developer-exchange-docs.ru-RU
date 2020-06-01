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
ms.openlocfilehash: 386dd2aa4e114d8382d5c83a3d6da70b1ccbbada
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457531"
---
# <a name="createfolderresponsemessage"></a><span data-ttu-id="2f6fe-103">креатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="2f6fe-103">CreateFolderResponseMessage</span></span>

<span data-ttu-id="2f6fe-104">Элемент **креатефолдерреспонсемессаже** содержит состояние и результат одного запроса [операции CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="2f6fe-104">The **CreateFolderResponseMessage** element contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span> 
  
```xml
<CreateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateFolderResponseMessage>
```

<span data-ttu-id="2f6fe-105">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-105">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2f6fe-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2f6fe-106">Attributes and elements</span></span>

<span data-ttu-id="2f6fe-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f6fe-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2f6fe-108">Attributes</span></span>

|<span data-ttu-id="2f6fe-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-109">**Attribute**</span></span>|<span data-ttu-id="2f6fe-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2f6fe-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="2f6fe-112">Описывает состояние ответа [операции CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="2f6fe-112">Describes the status of a [CreateFolder operation](createfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="2f6fe-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="2f6fe-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="2f6fe-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="2f6fe-114">-  Success</span></span>  <br/><span data-ttu-id="2f6fe-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="2f6fe-115">-  Warning</span></span>  <br/><span data-ttu-id="2f6fe-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="2f6fe-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="2f6fe-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="2f6fe-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="2f6fe-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-118">**Value**</span></span>|<span data-ttu-id="2f6fe-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2f6fe-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-120">**Success**</span></span> <br/> |<span data-ttu-id="2f6fe-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="2f6fe-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-122">**Warning**</span></span> <br/> | <span data-ttu-id="2f6fe-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-123">Describes a request that was not processed.</span></span> <span data-ttu-id="2f6fe-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="2f6fe-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="2f6fe-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="2f6fe-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="2f6fe-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="2f6fe-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="2f6fe-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="2f6fe-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="2f6fe-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-132">**Error**</span></span> <br/> | <span data-ttu-id="2f6fe-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="2f6fe-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="2f6fe-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="2f6fe-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="2f6fe-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="2f6fe-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="2f6fe-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="2f6fe-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="2f6fe-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="2f6fe-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="2f6fe-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="2f6fe-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="2f6fe-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="2f6fe-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="2f6fe-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="2f6fe-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2f6fe-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2f6fe-142">Child elements</span></span>

|<span data-ttu-id="2f6fe-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-143">**Element**</span></span>|<span data-ttu-id="2f6fe-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f6fe-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="2f6fe-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="2f6fe-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="2f6fe-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="2f6fe-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="2f6fe-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="2f6fe-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="2f6fe-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="2f6fe-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="2f6fe-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="2f6fe-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="2f6fe-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="2f6fe-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="2f6fe-154">Folders</span><span class="sxs-lookup"><span data-stu-id="2f6fe-154">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2f6fe-155">Содержит массив созданных папок.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-155">Contains an array of created folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2f6fe-156">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2f6fe-156">Parent elements</span></span>

|<span data-ttu-id="2f6fe-157">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-157">**Element**</span></span>|<span data-ttu-id="2f6fe-158">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2f6fe-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f6fe-159">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="2f6fe-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2f6fe-160">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2f6fe-161">Примечания</span><span class="sxs-lookup"><span data-stu-id="2f6fe-161">Remarks</span></span>

<span data-ttu-id="2f6fe-162">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2f6fe-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f6fe-163">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2f6fe-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f6fe-164">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2f6fe-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2f6fe-165">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2f6fe-165">Schema Name</span></span>  <br/> |<span data-ttu-id="2f6fe-166">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="2f6fe-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2f6fe-167">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2f6fe-167">Validation File</span></span>  <br/> |<span data-ttu-id="2f6fe-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2f6fe-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2f6fe-169">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2f6fe-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="2f6fe-170">False</span><span class="sxs-lookup"><span data-stu-id="2f6fe-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f6fe-171">См. также</span><span class="sxs-lookup"><span data-stu-id="2f6fe-171">See also</span></span>

- [<span data-ttu-id="2f6fe-172">Операция CreateFolder</span><span class="sxs-lookup"><span data-stu-id="2f6fe-172">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="2f6fe-173">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="2f6fe-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="2f6fe-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2f6fe-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

