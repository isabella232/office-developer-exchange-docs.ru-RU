---
title: ResolveNamesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNamesResponseMessage
api_type:
- schema
ms.assetid: edcdaf58-ef63-412e-8c58-409213e6ab0d
description: Элемент ResolveNamesResponseMessage содержит состояние и результат операции запроса ResolveNames.
ms.openlocfilehash: 953a1f0b19c078d969ffe175c22df02b58c5e939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835170"
---
# <a name="resolvenamesresponsemessage"></a><span data-ttu-id="e3871-103">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e3871-103">ResolveNamesResponseMessage</span></span>

<span data-ttu-id="e3871-104">Элемент **ResolveNamesResponseMessage** содержит состояние и результат [операции ResolveNames](resolvenames-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="e3871-104">The **ResolveNamesResponseMessage** element contains the status and result of a [ResolveNames operation](resolvenames-operation.md) request.</span></span> 
  
- [<span data-ttu-id="e3871-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="e3871-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md) 
- [<span data-ttu-id="e3871-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e3871-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="e3871-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e3871-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 <span data-ttu-id="e3871-108">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e3871-108">**ResolveNamesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3871-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e3871-109">Attributes and elements</span></span>

<span data-ttu-id="e3871-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e3871-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3871-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e3871-111">Attributes</span></span>

|<span data-ttu-id="e3871-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e3871-112">**Attribute**</span></span>|<span data-ttu-id="e3871-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3871-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e3871-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="e3871-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e3871-115">Описание состояния ответа [операции ResolveNames](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e3871-115">Describes the status of a [ResolveNames operation](resolvenames-operation.md) response.</span></span> <br/><br/><span data-ttu-id="e3871-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="e3871-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="e3871-117">-Success</span><span class="sxs-lookup"><span data-stu-id="e3871-117">-  Success</span></span>  <br/><span data-ttu-id="e3871-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="e3871-118">-  Warning</span></span>  <br/><span data-ttu-id="e3871-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="e3871-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="e3871-120">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e3871-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="e3871-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e3871-121">**Value**</span></span>|<span data-ttu-id="e3871-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3871-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e3871-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="e3871-123">**Success**</span></span> <br/> |<span data-ttu-id="e3871-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="e3871-124">Describes a request that is fulfilled.</span></span> <span data-ttu-id="e3871-125">Происходит, когда запрошенный имя однозначно идентифицируемый и ответ содержит одного получателя.</span><span class="sxs-lookup"><span data-stu-id="e3871-125">This occurs when the requested name is unambiguous and the response contains a single recipient.</span></span>  <br/> |
|<span data-ttu-id="e3871-126">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="e3871-126">**Warning**</span></span> <br/> | <span data-ttu-id="e3871-127">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="e3871-127">Describes a request that was not processed.</span></span> <span data-ttu-id="e3871-128">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="e3871-128">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="e3871-129">Вот пример источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="e3871-129">The following are example of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="e3871-130">-В хранилище Exchange переходит в автономный режим во время пакета.</span><span class="sxs-lookup"><span data-stu-id="e3871-130">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="e3871-131">-Доменных служб active Directory (AD DS) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="e3871-131">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="e3871-132">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="e3871-132">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="e3871-133">-Базы данных почтовых ящиков (MDB) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="e3871-133">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="e3871-134">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="e3871-134">-  A password is expired.</span></span>  <br/><span data-ttu-id="e3871-135">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="e3871-135">-  A quota is exceeded.</span></span>  <br/><span data-ttu-id="e3871-136">— Имя запрошенного является неоднозначным и ответ содержит несколько получателей.</span><span class="sxs-lookup"><span data-stu-id="e3871-136">-  The requested name is ambiguous and the response contains multiple recipients.</span></span>  <br/> |
|<span data-ttu-id="e3871-137">**Error**</span><span class="sxs-lookup"><span data-stu-id="e3871-137">**Error**</span></span> <br/> | <span data-ttu-id="e3871-138">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="e3871-138">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e3871-139">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="e3871-139">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e3871-140">-Указанное имя не может быть разрешен.</span><span class="sxs-lookup"><span data-stu-id="e3871-140">-  The requested name could not be resolved.</span></span>  <br/><span data-ttu-id="e3871-141">-Атрибуты или элементы являются недопустимыми.</span><span class="sxs-lookup"><span data-stu-id="e3871-141">-  Attributes or elements are invalid.</span></span>  <br/><span data-ttu-id="e3871-142">-Атрибуты или элементы находятся вне диапазона.</span><span class="sxs-lookup"><span data-stu-id="e3871-142">-  Attributes or elements are out of range.</span></span>  <br/><span data-ttu-id="e3871-143">-Неизвестно тег.</span><span class="sxs-lookup"><span data-stu-id="e3871-143">-  A tag is unknown.</span></span>  <br/><span data-ttu-id="e3871-144">-Атрибута или элемента не является допустимым в контексте.</span><span class="sxs-lookup"><span data-stu-id="e3871-144">-  An attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="e3871-145">-Произошла попытка несанкционированного доступа с любого клиента.</span><span class="sxs-lookup"><span data-stu-id="e3871-145">-  An unauthorized access attempt by any client occurred.</span></span>  <br/><span data-ttu-id="e3871-146">-На сервере сбой в ответ на допустимый вызовов со стороны клиента.</span><span class="sxs-lookup"><span data-stu-id="e3871-146">-  A server-side failure occurred in response to a valid client-side call.</span></span>  <br/>  <br/><span data-ttu-id="e3871-147">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="e3871-147">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e3871-148">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e3871-148">Child elements</span></span>

|<span data-ttu-id="e3871-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e3871-149">**Element**</span></span>|<span data-ttu-id="e3871-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3871-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3871-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="e3871-151">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e3871-152">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="e3871-152">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e3871-153">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e3871-153">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e3871-154">Предоставляет сведения о запросе.</span><span class="sxs-lookup"><span data-stu-id="e3871-154">Provides error information about the request.</span></span>  <br/> |
|[<span data-ttu-id="e3871-155">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e3871-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e3871-156">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="e3871-156">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e3871-157">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="e3871-157">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e3871-158">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e3871-158">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e3871-159">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="e3871-159">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e3871-160">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="e3871-160">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="e3871-161">Содержит набор разрешений для разрешения неоднозначных псевдонимов.</span><span class="sxs-lookup"><span data-stu-id="e3871-161">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3871-162">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e3871-162">Parent elements</span></span>

|<span data-ttu-id="e3871-163">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e3871-163">**Element**</span></span>|<span data-ttu-id="e3871-164">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3871-164">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3871-165">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e3871-165">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e3871-166">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="e3871-166">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e3871-167">Замечания</span><span class="sxs-lookup"><span data-stu-id="e3871-167">Remarks</span></span>

<span data-ttu-id="e3871-168">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e3871-168">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3871-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e3871-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3871-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e3871-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e3871-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e3871-171">Schema name</span></span>  <br/> |<span data-ttu-id="e3871-172">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e3871-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e3871-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e3871-173">Validation file</span></span>  <br/> |<span data-ttu-id="e3871-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e3871-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e3871-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e3871-175">Can be empty</span></span>  <br/> |<span data-ttu-id="e3871-176">False</span><span class="sxs-lookup"><span data-stu-id="e3871-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3871-177">См. также</span><span class="sxs-lookup"><span data-stu-id="e3871-177">See also</span></span>

- [<span data-ttu-id="e3871-178">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="e3871-178">ResolveNames</span></span>](resolvenames.md)
- [<span data-ttu-id="e3871-179">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="e3871-179">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
- [<span data-ttu-id="e3871-180">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="e3871-180">ResolveNames operation</span></span>](resolvenames-operation.md)

