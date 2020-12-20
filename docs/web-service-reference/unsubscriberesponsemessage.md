---
title: UnsubscribeResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnsubscribeResponseMessage
api_type:
- schema
ms.assetid: 92c53b13-0ca1-4b44-b925-b23682e9417c
description: Элемент UnsubscribeResponseMessage содержит состояние и результаты одного запроса операции Unsubscribe.
ms.openlocfilehash: e5b42404d09e6367c134934409ec2a45351e135e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467167"
---
# <a name="unsubscriberesponsemessage"></a><span data-ttu-id="150c7-103">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="150c7-103">UnsubscribeResponseMessage</span></span>

<span data-ttu-id="150c7-104">Элемент **UnsubscribeResponseMessage** содержит состояние и результаты одного запроса [операции Unsubscribe](unsubscribe-operation.md).</span><span class="sxs-lookup"><span data-stu-id="150c7-104">The **UnsubscribeResponseMessage** element contains the status and result of a single [Unsubscribe operation](unsubscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="150c7-105">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="150c7-105">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
- [<span data-ttu-id="150c7-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="150c7-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="150c7-107">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="150c7-107">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
  
```xml
<UnsubscribeResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UnsubscribeResponseMessage>
```

 <span data-ttu-id="150c7-108">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="150c7-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="150c7-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="150c7-109">Attributes and elements</span></span>

<span data-ttu-id="150c7-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="150c7-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="150c7-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="150c7-111">Attributes</span></span>

|<span data-ttu-id="150c7-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="150c7-112">**Attribute**</span></span>|<span data-ttu-id="150c7-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="150c7-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="150c7-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="150c7-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="150c7-115">Описывает состояние отклика [операции Unsubscribe](unsubscribe-operation.md).</span><span class="sxs-lookup"><span data-stu-id="150c7-115">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="150c7-116">Для данного атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="150c7-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="150c7-117">–  Success</span><span class="sxs-lookup"><span data-stu-id="150c7-117">-  Success</span></span>  <br/><span data-ttu-id="150c7-118">–  Warning</span><span class="sxs-lookup"><span data-stu-id="150c7-118">-  Warning</span></span>  <br/><span data-ttu-id="150c7-119">–  Error</span><span class="sxs-lookup"><span data-stu-id="150c7-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="150c7-120">Значения атрибута ResponseClass</span><span class="sxs-lookup"><span data-stu-id="150c7-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="150c7-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="150c7-121">**Value**</span></span>|<span data-ttu-id="150c7-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="150c7-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="150c7-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="150c7-123">**Success**</span></span> <br/> |<span data-ttu-id="150c7-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="150c7-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="150c7-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="150c7-125">**Warning**</span></span> <br/> | <span data-ttu-id="150c7-126">Описывает необработанный запрос.</span><span class="sxs-lookup"><span data-stu-id="150c7-126">Describes a request that was not processed.</span></span> <span data-ttu-id="150c7-127">Предупреждение может возвращаться, если произошла ошибка при обработке элемента запроса и невозможности обработки последующих элементов.</span><span class="sxs-lookup"><span data-stu-id="150c7-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="150c7-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="150c7-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="150c7-129">– Хранилище Exchange находится в автономном режиме при обработке пакета.</span><span class="sxs-lookup"><span data-stu-id="150c7-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="150c7-130">– Доменные службы Active Directory (AD DS) находятся в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="150c7-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="150c7-131">– Почтовые ящики перемещены.</span><span class="sxs-lookup"><span data-stu-id="150c7-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="150c7-132">– База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="150c7-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="150c7-133">– Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="150c7-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="150c7-134">– Превышена квота</span><span class="sxs-lookup"><span data-stu-id="150c7-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="150c7-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="150c7-135">**Error**</span></span> <br/> | <span data-ttu-id="150c7-136">Описывает запрос, который невозможно выполнить.</span><span class="sxs-lookup"><span data-stu-id="150c7-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="150c7-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="150c7-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="150c7-138">– Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="150c7-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="150c7-139">– Атрибуты или элементы находятся вне диапазона</span><span class="sxs-lookup"><span data-stu-id="150c7-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="150c7-140">– Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="150c7-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="150c7-141">– Атрибут или элемент недопустим в контексте</span><span class="sxs-lookup"><span data-stu-id="150c7-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="150c7-142">– Попытка неавторизованного доступа любым клиентом</span><span class="sxs-lookup"><span data-stu-id="150c7-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="150c7-143">– Сбой на стороне сервера в ответ на допустимый клиентский вызов</span><span class="sxs-lookup"><span data-stu-id="150c7-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="150c7-144">Сведения об ошибке доступны в элементах [ResponseCode](responsecode.md) и [MessageText](messagetext.md).</span><span class="sxs-lookup"><span data-stu-id="150c7-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="150c7-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="150c7-145">Child elements</span></span>

|<span data-ttu-id="150c7-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="150c7-146">**Element**</span></span>|<span data-ttu-id="150c7-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="150c7-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="150c7-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="150c7-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="150c7-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="150c7-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="150c7-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="150c7-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="150c7-151">Предоставляет код ошибки, определяющий конкретную ошибку, с которой столкнулся запрос.</span><span class="sxs-lookup"><span data-stu-id="150c7-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="150c7-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="150c7-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="150c7-153">В настоящее время не используется и зарезервирован для последующего применения.</span><span class="sxs-lookup"><span data-stu-id="150c7-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="150c7-154">Содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="150c7-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="150c7-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="150c7-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="150c7-156">Предоставляет дополнительные сведения об отклике с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="150c7-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="150c7-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="150c7-157">Parent elements</span></span>

|<span data-ttu-id="150c7-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="150c7-158">**Element**</span></span>|<span data-ttu-id="150c7-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="150c7-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="150c7-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="150c7-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="150c7-161">Содержит сообщения отклика для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="150c7-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="150c7-162">Примечания</span><span class="sxs-lookup"><span data-stu-id="150c7-162">Remarks</span></span>

<span data-ttu-id="150c7-163">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2010, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="150c7-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="150c7-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="150c7-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="150c7-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="150c7-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="150c7-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="150c7-166">Schema Name</span></span>  <br/> |<span data-ttu-id="150c7-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="150c7-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="150c7-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="150c7-168">Validation File</span></span>  <br/> |<span data-ttu-id="150c7-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="150c7-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="150c7-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="150c7-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="150c7-171">False</span><span class="sxs-lookup"><span data-stu-id="150c7-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="150c7-172">См. также</span><span class="sxs-lookup"><span data-stu-id="150c7-172">See also</span></span>

- [<span data-ttu-id="150c7-173">Операция Unsubscribe</span><span class="sxs-lookup"><span data-stu-id="150c7-173">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="150c7-174">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="150c7-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

