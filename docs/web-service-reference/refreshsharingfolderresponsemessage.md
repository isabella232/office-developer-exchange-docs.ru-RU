---
title: рефрешшарингфолдерреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolderResponseMessage
api_type:
- schema
ms.assetid: 53ee65bd-cf75-4e04-9b27-eff1b040ae82
description: Элемент Рефрешшарингфолдерреспонсемессаже содержит состояние и результат одного запроса операции RefreshSharingFolder.
ms.openlocfilehash: 9dbb66c294439f33a9307d51c03dd1cd127e95e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835052"
---
# <a name="refreshsharingfolderresponsemessage"></a><span data-ttu-id="aeb33-103">рефрешшарингфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="aeb33-103">RefreshSharingFolderResponseMessage</span></span>

<span data-ttu-id="aeb33-104">Элемент **рефрешшарингфолдерреспонсемессаже** содержит состояние и результат одного запроса [операции RefreshSharingFolder](refreshsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="aeb33-104">The **RefreshSharingFolderResponseMessage** element contains the status and result of a single [RefreshSharingFolder operation](refreshsharingfolder-operation.md) request.</span></span> 
  
```xml
<RefreshSharingFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponseMessage>
```

 <span data-ttu-id="aeb33-105">**рефрешшарингфолдерреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="aeb33-105">**RefreshSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aeb33-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aeb33-106">Attributes and elements</span></span>

<span data-ttu-id="aeb33-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="aeb33-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aeb33-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aeb33-108">Attributes</span></span>

|<span data-ttu-id="aeb33-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="aeb33-109">**Attribute**</span></span>|<span data-ttu-id="aeb33-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aeb33-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aeb33-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="aeb33-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="aeb33-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="aeb33-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="aeb33-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="aeb33-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="aeb33-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="aeb33-114">-  Success</span></span>  <br/><span data-ttu-id="aeb33-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="aeb33-115">-  Warning</span></span>  <br/><span data-ttu-id="aeb33-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="aeb33-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="aeb33-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="aeb33-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="aeb33-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="aeb33-118">**Value**</span></span>|<span data-ttu-id="aeb33-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aeb33-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aeb33-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="aeb33-120">**Success**</span></span> <br/> |<span data-ttu-id="aeb33-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="aeb33-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="aeb33-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="aeb33-122">**Warning**</span></span> <br/> | <span data-ttu-id="aeb33-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="aeb33-123">Describes a request that was not processed.</span></span> <span data-ttu-id="aeb33-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="aeb33-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="aeb33-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="aeb33-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="aeb33-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="aeb33-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="aeb33-127">— Служба каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="aeb33-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="aeb33-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="aeb33-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="aeb33-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="aeb33-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="aeb33-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="aeb33-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="aeb33-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="aeb33-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="aeb33-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="aeb33-132">**Error**</span></span> <br/> | <span data-ttu-id="aeb33-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="aeb33-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="aeb33-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="aeb33-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="aeb33-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="aeb33-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="aeb33-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="aeb33-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="aeb33-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="aeb33-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="aeb33-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="aeb33-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="aeb33-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="aeb33-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="aeb33-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="aeb33-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="aeb33-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="aeb33-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aeb33-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aeb33-142">Child elements</span></span>

|<span data-ttu-id="aeb33-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aeb33-143">**Element**</span></span>|<span data-ttu-id="aeb33-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aeb33-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aeb33-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="aeb33-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="aeb33-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="aeb33-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="aeb33-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="aeb33-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="aeb33-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="aeb33-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="aeb33-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="aeb33-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="aeb33-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="aeb33-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="aeb33-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="aeb33-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="aeb33-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="aeb33-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="aeb33-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="aeb33-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aeb33-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aeb33-154">Parent elements</span></span>

|<span data-ttu-id="aeb33-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aeb33-155">**Element**</span></span>|<span data-ttu-id="aeb33-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aeb33-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aeb33-157">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="aeb33-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="aeb33-158">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="aeb33-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aeb33-159">Примечания</span><span class="sxs-lookup"><span data-stu-id="aeb33-159">Remarks</span></span>

<span data-ttu-id="aeb33-160">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="aeb33-160">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aeb33-161">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aeb33-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aeb33-162">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aeb33-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aeb33-163">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aeb33-163">Schema Name</span></span>  <br/> |<span data-ttu-id="aeb33-164">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="aeb33-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aeb33-165">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aeb33-165">Validation File</span></span>  <br/> |<span data-ttu-id="aeb33-166">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="aeb33-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aeb33-167">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aeb33-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="aeb33-168">False</span><span class="sxs-lookup"><span data-stu-id="aeb33-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aeb33-169">См. также</span><span class="sxs-lookup"><span data-stu-id="aeb33-169">See also</span></span>

- [<span data-ttu-id="aeb33-170">Операция RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="aeb33-170">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md)
- [<span data-ttu-id="aeb33-171">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aeb33-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

