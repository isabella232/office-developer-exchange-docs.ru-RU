---
title: жетинбоксрулесреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRulesResponse
api_type:
- schema
ms.assetid: 6d6c1950-c328-489a-94bf-a250fdbd5cd9
description: Элемент Жетинбоксрулесреспонсе определяет ответ на запрос операции GetInboxRules.
ms.openlocfilehash: 0d67d7eaf6ffbeeb790249190a98f252dbdb9c87
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458287"
---
# <a name="getinboxrulesresponse"></a><span data-ttu-id="aa510-103">жетинбоксрулесреспонсе</span><span class="sxs-lookup"><span data-stu-id="aa510-103">GetInboxRulesResponse</span></span>

<span data-ttu-id="aa510-104">Элемент **жетинбоксрулесреспонсе** определяет ответ на запрос [операции GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="aa510-104">The **GetInboxRulesResponse** element defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span> 
  
```XML
<GetInboxRulesResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <OutlookRuleBlobExists/>
   <InboxRules/>
</GetInboxRulesResponse>
```

 <span data-ttu-id="aa510-105">**жетинбоксрулесреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="aa510-105">**GetInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa510-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aa510-106">Attributes and elements</span></span>

<span data-ttu-id="aa510-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="aa510-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa510-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aa510-108">Attributes</span></span>

|<span data-ttu-id="aa510-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="aa510-109">**Attribute**</span></span>|<span data-ttu-id="aa510-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa510-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa510-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="aa510-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="aa510-112">Описывает состояние ответа [операции GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="aa510-112">Describes the status of a [GetInboxRules operation](getinboxrules-operation.md) response.</span></span> <br/><br/><span data-ttu-id="aa510-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="aa510-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="aa510-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="aa510-114">-  Success</span></span>  <br/><span data-ttu-id="aa510-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="aa510-115">-  Warning</span></span>  <br/><span data-ttu-id="aa510-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="aa510-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="aa510-117">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="aa510-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="aa510-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="aa510-118">**Value**</span></span>|<span data-ttu-id="aa510-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa510-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa510-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="aa510-120">**Success**</span></span> <br/> |<span data-ttu-id="aa510-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="aa510-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="aa510-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="aa510-122">**Warning**</span></span> <br/> | <span data-ttu-id="aa510-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="aa510-123">Describes a request that was not processed.</span></span> <span data-ttu-id="aa510-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="aa510-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="aa510-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="aa510-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="aa510-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="aa510-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="aa510-127">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="aa510-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="aa510-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="aa510-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="aa510-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="aa510-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="aa510-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="aa510-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="aa510-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="aa510-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="aa510-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="aa510-132">**Error**</span></span> <br/> | <span data-ttu-id="aa510-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="aa510-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="aa510-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="aa510-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="aa510-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="aa510-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="aa510-136">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="aa510-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="aa510-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="aa510-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="aa510-138">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="aa510-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="aa510-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="aa510-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="aa510-140">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="aa510-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="aa510-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="aa510-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aa510-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aa510-142">Child elements</span></span>

|<span data-ttu-id="aa510-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa510-143">**Element**</span></span>|<span data-ttu-id="aa510-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa510-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa510-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="aa510-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="aa510-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="aa510-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="aa510-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="aa510-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="aa510-148">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="aa510-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="aa510-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="aa510-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="aa510-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="aa510-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="aa510-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="aa510-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="aa510-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="aa510-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="aa510-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="aa510-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="aa510-154">аутлукрулеблобексистс</span><span class="sxs-lookup"><span data-stu-id="aa510-154">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md) <br/> |<span data-ttu-id="aa510-155">Указывает, существует ли большой двоичный объект правила Microsoft Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa510-155">Indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="aa510-156">инбоксрулес</span><span class="sxs-lookup"><span data-stu-id="aa510-156">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="aa510-157">Представляет массив правил в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa510-157">Represents an array of the rules in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa510-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aa510-158">Parent elements</span></span>

<span data-ttu-id="aa510-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aa510-159">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="aa510-160">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="aa510-160">Text value</span></span>

<span data-ttu-id="aa510-161">Нет.</span><span class="sxs-lookup"><span data-stu-id="aa510-161">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aa510-162">Примечания</span><span class="sxs-lookup"><span data-stu-id="aa510-162">Remarks</span></span>

<span data-ttu-id="aa510-163">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa510-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa510-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aa510-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa510-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aa510-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa510-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aa510-166">Schema name</span></span>  <br/> |<span data-ttu-id="aa510-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="aa510-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aa510-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aa510-168">Validation file</span></span>  <br/> |<span data-ttu-id="aa510-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="aa510-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa510-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aa510-170">Can be empty</span></span>  <br/> |<span data-ttu-id="aa510-171">False</span><span class="sxs-lookup"><span data-stu-id="aa510-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa510-172">См. также</span><span class="sxs-lookup"><span data-stu-id="aa510-172">See also</span></span>

- [<span data-ttu-id="aa510-173">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="aa510-173">GetInboxRules</span></span>](getinboxrules.md)
- [<span data-ttu-id="aa510-174">Операция GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="aa510-174">GetInboxRules operation</span></span>](getinboxrules-operation.md)

