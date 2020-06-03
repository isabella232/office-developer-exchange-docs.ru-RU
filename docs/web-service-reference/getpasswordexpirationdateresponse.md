---
title: жетпассвордекспиратиондатереспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: Элемент Жетпассвордекспиратиондатереспонсе определяет ответ на запрос операции GetPasswordExpirationDate.
ms.openlocfilehash: c925b2b37879ba0f8f25b2dd73737ed2f3202555
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530206"
---
# <a name="getpasswordexpirationdateresponse"></a><span data-ttu-id="02ceb-103">жетпассвордекспиратиондатереспонсе</span><span class="sxs-lookup"><span data-stu-id="02ceb-103">GetPasswordExpirationDateResponse</span></span>

<span data-ttu-id="02ceb-104">Элемент **жетпассвордекспиратиондатереспонсе** определяет ответ на запрос операции [GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="02ceb-104">The **GetPasswordExpirationDateResponse** element defines the response to a [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation request.</span></span> 
  
- [<span data-ttu-id="02ceb-105">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="02ceb-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="02ceb-106">жетпассвордекспиратиондатереспонсе</span><span class="sxs-lookup"><span data-stu-id="02ceb-106">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 <span data-ttu-id="02ceb-107">**жетпассвордекспиратиондатереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="02ceb-107">**GetPasswordExpirationDateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02ceb-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02ceb-108">Attributes and elements</span></span>

<span data-ttu-id="02ceb-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="02ceb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02ceb-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="02ceb-110">Attributes</span></span>

|<span data-ttu-id="02ceb-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="02ceb-111">**Attribute**</span></span>|<span data-ttu-id="02ceb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02ceb-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="02ceb-113">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="02ceb-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="02ceb-114">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="02ceb-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="02ceb-115">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="02ceb-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="02ceb-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="02ceb-116">-  Success</span></span>  <br/><span data-ttu-id="02ceb-117">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="02ceb-117">-  Warning</span></span>  <br/><span data-ttu-id="02ceb-118">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="02ceb-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="02ceb-119">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="02ceb-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="02ceb-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="02ceb-120">**Value**</span></span>|<span data-ttu-id="02ceb-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02ceb-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="02ceb-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="02ceb-122">**Success**</span></span> <br/> |<span data-ttu-id="02ceb-123">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="02ceb-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="02ceb-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="02ceb-124">**Warning**</span></span> <br/> | <span data-ttu-id="02ceb-125">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="02ceb-125">Describes a request that was not processed.</span></span> <span data-ttu-id="02ceb-126">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="02ceb-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="02ceb-127">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="02ceb-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="02ceb-128">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="02ceb-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="02ceb-129">-Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="02ceb-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="02ceb-130">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="02ceb-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="02ceb-131">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="02ceb-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="02ceb-132">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="02ceb-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="02ceb-133">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="02ceb-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="02ceb-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="02ceb-134">**Error**</span></span> <br/> | <span data-ttu-id="02ceb-135">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="02ceb-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="02ceb-136">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="02ceb-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="02ceb-137">— Недопустимые атрибуты или элементы.</span><span class="sxs-lookup"><span data-stu-id="02ceb-137">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="02ceb-138">— Атрибуты или элементы, которые выходят за пределы диапазона.</span><span class="sxs-lookup"><span data-stu-id="02ceb-138">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="02ceb-139">— Неизвестный тег.</span><span class="sxs-lookup"><span data-stu-id="02ceb-139">-  An unknown tag.</span></span>  <br/><span data-ttu-id="02ceb-140">— Атрибут или элемент, который не является допустимым в контексте.</span><span class="sxs-lookup"><span data-stu-id="02ceb-140">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="02ceb-141">— Попытки несанкционированного доступа, выполняемые любым клиентом.</span><span class="sxs-lookup"><span data-stu-id="02ceb-141">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="02ceb-142">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="02ceb-142">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="02ceb-143">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="02ceb-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="02ceb-144">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="02ceb-144">Child elements</span></span>

|<span data-ttu-id="02ceb-145">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="02ceb-145">**Element name**</span></span>|<span data-ttu-id="02ceb-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02ceb-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02ceb-147">пассвордекспиратиондате</span><span class="sxs-lookup"><span data-stu-id="02ceb-147">PasswordExpirationDate</span></span>](passwordexpirationdate.md) <br/> |<span data-ttu-id="02ceb-148">Предоставляет срок действия пароля для учетной записи электронной почты, указанной в запросе.</span><span class="sxs-lookup"><span data-stu-id="02ceb-148">Provides the password expiration date for the email account specified in the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02ceb-149">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="02ceb-149">Parent elements</span></span>

|<span data-ttu-id="02ceb-150">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="02ceb-150">**Element name**</span></span>|<span data-ttu-id="02ceb-151">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02ceb-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02ceb-152">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="02ceb-152">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="02ceb-153">Содержит сообщения ответа для запроса веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="02ceb-153">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="02ceb-154">Примечания</span><span class="sxs-lookup"><span data-stu-id="02ceb-154">Remarks</span></span>

<span data-ttu-id="02ceb-155">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="02ceb-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="02ceb-156">Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="02ceb-156">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02ceb-157">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="02ceb-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02ceb-158">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="02ceb-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="02ceb-159">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="02ceb-159">Schema Name</span></span>  <br/> |<span data-ttu-id="02ceb-160">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="02ceb-160">Messages schema</span></span>  <br/> |
|<span data-ttu-id="02ceb-161">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="02ceb-161">Validation File</span></span>  <br/> |<span data-ttu-id="02ceb-162">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="02ceb-162">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02ceb-163">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="02ceb-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="02ceb-164">False</span><span class="sxs-lookup"><span data-stu-id="02ceb-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02ceb-165">См. также</span><span class="sxs-lookup"><span data-stu-id="02ceb-165">See also</span></span>

- [<span data-ttu-id="02ceb-166">Операция GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="02ceb-166">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="02ceb-167">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="02ceb-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

