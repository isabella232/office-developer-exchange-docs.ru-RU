---
title: GetInboxRulesResponse
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
description: Элемент GetInboxRulesResponse определяет ответ на запрос операции GetInboxRules.
ms.openlocfilehash: d84064ab777fe13ded7727381842ddd1ee9d047d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762831"
---
# <a name="getinboxrulesresponse"></a><span data-ttu-id="89397-103">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="89397-103">GetInboxRulesResponse</span></span>

<span data-ttu-id="89397-104">Элемент **GetInboxRulesResponse** определяет ответ на запрос [GetInboxRules операции](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="89397-104">The **GetInboxRulesResponse** element defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="89397-105">**GetInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="89397-105">**GetInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89397-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="89397-106">Attributes and elements</span></span>

<span data-ttu-id="89397-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="89397-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89397-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="89397-108">Attributes</span></span>

|<span data-ttu-id="89397-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="89397-109">**Attribute**</span></span>|<span data-ttu-id="89397-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89397-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="89397-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="89397-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="89397-112">Описание состояния ответа [операции GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="89397-112">Describes the status of a [GetInboxRules operation](getinboxrules-operation.md) response.</span></span> <br/><br/><span data-ttu-id="89397-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="89397-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="89397-114">-Success</span><span class="sxs-lookup"><span data-stu-id="89397-114">-  Success</span></span>  <br/><span data-ttu-id="89397-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="89397-115">-  Warning</span></span>  <br/><span data-ttu-id="89397-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="89397-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="89397-117">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="89397-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="89397-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="89397-118">**Value**</span></span>|<span data-ttu-id="89397-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89397-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="89397-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="89397-120">**Success**</span></span> <br/> |<span data-ttu-id="89397-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="89397-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="89397-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="89397-122">**Warning**</span></span> <br/> | <span data-ttu-id="89397-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="89397-123">Describes a request that was not processed.</span></span> <span data-ttu-id="89397-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="89397-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="89397-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="89397-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="89397-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="89397-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="89397-127">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="89397-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="89397-128">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="89397-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="89397-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="89397-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="89397-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="89397-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="89397-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="89397-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="89397-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="89397-132">**Error**</span></span> <br/> | <span data-ttu-id="89397-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="89397-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="89397-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="89397-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="89397-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="89397-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="89397-136">-Атрибуты или элементы, которые являются вне диапазона</span><span class="sxs-lookup"><span data-stu-id="89397-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="89397-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="89397-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="89397-138">-Атрибута или элемента, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="89397-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="89397-139">-Попытка несанкционированного доступа с любого клиента</span><span class="sxs-lookup"><span data-stu-id="89397-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="89397-140">-Сбой на сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="89397-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="89397-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="89397-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="89397-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="89397-142">Child elements</span></span>

|<span data-ttu-id="89397-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="89397-143">**Element**</span></span>|<span data-ttu-id="89397-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89397-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89397-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="89397-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="89397-146">Текст с описанием состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="89397-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="89397-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="89397-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="89397-148">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="89397-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="89397-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="89397-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="89397-150">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="89397-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="89397-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="89397-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="89397-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="89397-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="89397-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="89397-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="89397-154">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="89397-154">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md) <br/> |<span data-ttu-id="89397-155">Показывает, существует ли правило большого двоичного объекта Microsoft Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="89397-155">Indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="89397-156">InboxRules</span><span class="sxs-lookup"><span data-stu-id="89397-156">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="89397-157">Представляет собой массив из правил в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="89397-157">Represents an array of the rules in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89397-158">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="89397-158">Parent elements</span></span>

<span data-ttu-id="89397-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="89397-159">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="89397-160">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="89397-160">Text value</span></span>

<span data-ttu-id="89397-161">Нет.</span><span class="sxs-lookup"><span data-stu-id="89397-161">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89397-162">Замечания</span><span class="sxs-lookup"><span data-stu-id="89397-162">Remarks</span></span>

<span data-ttu-id="89397-163">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="89397-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89397-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="89397-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89397-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="89397-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89397-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="89397-166">Schema name</span></span>  <br/> |<span data-ttu-id="89397-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="89397-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89397-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="89397-168">Validation file</span></span>  <br/> |<span data-ttu-id="89397-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="89397-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89397-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="89397-170">Can be empty</span></span>  <br/> |<span data-ttu-id="89397-171">False</span><span class="sxs-lookup"><span data-stu-id="89397-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89397-172">См. также</span><span class="sxs-lookup"><span data-stu-id="89397-172">See also</span></span>

- [<span data-ttu-id="89397-173">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="89397-173">GetInboxRules</span></span>](getinboxrules.md)
- [<span data-ttu-id="89397-174">Операция GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="89397-174">GetInboxRules operation</span></span>](getinboxrules-operation.md)

