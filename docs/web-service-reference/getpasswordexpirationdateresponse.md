---
title: GetPasswordExpirationDateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: Элемент GetPasswordExpirationDateResponse определяет ответ на запрос GetPasswordExpirationDate операция операции.
ms.openlocfilehash: 3754a53da53c12479f11c2e32cd15a08cba665fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762888"
---
# <a name="getpasswordexpirationdateresponse"></a><span data-ttu-id="6045a-103">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="6045a-103">GetPasswordExpirationDateResponse</span></span>

<span data-ttu-id="6045a-104">Элемент **GetPasswordExpirationDateResponse** определяет ответ на запрос операции [GetPasswordExpirationDate операции](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6045a-104">The **GetPasswordExpirationDateResponse** element defines the response to a [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation request.</span></span> 
  
- [<span data-ttu-id="6045a-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6045a-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="6045a-106">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="6045a-106">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 <span data-ttu-id="6045a-107">**GetPasswordExpirationDateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6045a-107">**GetPasswordExpirationDateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6045a-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6045a-108">Attributes and elements</span></span>

<span data-ttu-id="6045a-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6045a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6045a-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6045a-110">Attributes</span></span>

|<span data-ttu-id="6045a-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6045a-111">**Attribute**</span></span>|<span data-ttu-id="6045a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6045a-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6045a-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="6045a-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="6045a-114">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="6045a-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="6045a-115">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="6045a-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="6045a-116">-Success</span><span class="sxs-lookup"><span data-stu-id="6045a-116">-  Success</span></span>  <br/><span data-ttu-id="6045a-117">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="6045a-117">-  Warning</span></span>  <br/><span data-ttu-id="6045a-118">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="6045a-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="6045a-119">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="6045a-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="6045a-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="6045a-120">**Value**</span></span>|<span data-ttu-id="6045a-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6045a-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6045a-122">**Успех**</span><span class="sxs-lookup"><span data-stu-id="6045a-122">**Success**</span></span> <br/> |<span data-ttu-id="6045a-123">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="6045a-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="6045a-124">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="6045a-124">**Warning**</span></span> <br/> | <span data-ttu-id="6045a-125">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="6045a-125">Describes a request that was not processed.</span></span> <span data-ttu-id="6045a-126">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="6045a-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="6045a-127">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="6045a-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="6045a-128">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="6045a-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="6045a-129">-Доменных служб active Directory (AD DS) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="6045a-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="6045a-130">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="6045a-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="6045a-131">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="6045a-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="6045a-132">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="6045a-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="6045a-133">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="6045a-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="6045a-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="6045a-134">**Error**</span></span> <br/> | <span data-ttu-id="6045a-135">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="6045a-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="6045a-136">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="6045a-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="6045a-137">-Недопустимых атрибутов и элементов.</span><span class="sxs-lookup"><span data-stu-id="6045a-137">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="6045a-138">-Атрибуты или элементы, которые являются вне диапазона.</span><span class="sxs-lookup"><span data-stu-id="6045a-138">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="6045a-139">— Неизвестный тег.</span><span class="sxs-lookup"><span data-stu-id="6045a-139">-  An unknown tag.</span></span>  <br/><span data-ttu-id="6045a-140">-Атрибута или элемента, который не является допустимым в контексте.</span><span class="sxs-lookup"><span data-stu-id="6045a-140">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="6045a-141">-При попытке несанкционированного доступа с любого клиента.</span><span class="sxs-lookup"><span data-stu-id="6045a-141">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="6045a-142">-На сервере сбой в ответ на допустимый вызовов со стороны клиента.</span><span class="sxs-lookup"><span data-stu-id="6045a-142">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="6045a-143">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="6045a-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6045a-144">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6045a-144">Child elements</span></span>

|<span data-ttu-id="6045a-145">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="6045a-145">**Element name**</span></span>|<span data-ttu-id="6045a-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6045a-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6045a-147">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="6045a-147">PasswordExpirationDate</span></span>](passwordexpirationdate.md) <br/> |<span data-ttu-id="6045a-148">Предоставляет срок действия пароля для учетной записи электронной почты, указанной в запросе.</span><span class="sxs-lookup"><span data-stu-id="6045a-148">Provides the password expiration date for the email account specified in the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6045a-149">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6045a-149">Parent elements</span></span>

|<span data-ttu-id="6045a-150">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="6045a-150">**Element name**</span></span>|<span data-ttu-id="6045a-151">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6045a-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6045a-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6045a-152">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="6045a-153">Содержит сообщения ответа на запрос веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="6045a-153">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6045a-154">Замечания</span><span class="sxs-lookup"><span data-stu-id="6045a-154">Remarks</span></span>

<span data-ttu-id="6045a-155">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6045a-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="6045a-156">Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="6045a-156">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6045a-157">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6045a-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6045a-158">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6045a-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6045a-159">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6045a-159">Schema Name</span></span>  <br/> |<span data-ttu-id="6045a-160">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6045a-160">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6045a-161">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6045a-161">Validation File</span></span>  <br/> |<span data-ttu-id="6045a-162">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6045a-162">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6045a-163">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6045a-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="6045a-164">False</span><span class="sxs-lookup"><span data-stu-id="6045a-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6045a-165">См. также</span><span class="sxs-lookup"><span data-stu-id="6045a-165">See also</span></span>

- [<span data-ttu-id="6045a-166">Операция GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="6045a-166">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="6045a-167">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6045a-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
