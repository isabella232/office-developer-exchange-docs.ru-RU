---
title: DeleteItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponseMessage
api_type:
- schema
ms.assetid: c3d34c4d-8d83-4612-aa9e-66f9cc7314df
description: Элемент DeleteItemResponseMessage содержит состояние и результат одного запроса DeleteItem операции.
ms.openlocfilehash: 1f0cc3d49bfa5fba6da32cf65df6b6718ccfbded
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762055"
---
# <a name="deleteitemresponsemessage"></a><span data-ttu-id="8b5c6-103">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8b5c6-103">DeleteItemResponseMessage</span></span>

<span data-ttu-id="8b5c6-104">Элемент **DeleteItemResponseMessage** содержит состояние и результат одного запроса [DeleteItem операции](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="8b5c6-104">The **DeleteItemResponseMessage** element contains the status and result of a single [DeleteItem operation](deleteitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="8b5c6-105">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="8b5c6-105">DeleteItemResponse</span></span>](deleteitemresponse.md) 
- [<span data-ttu-id="8b5c6-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8b5c6-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="8b5c6-107">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8b5c6-107">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 <span data-ttu-id="8b5c6-108">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-108">**DeleteItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b5c6-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8b5c6-109">Attributes and elements</span></span>

<span data-ttu-id="8b5c6-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b5c6-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8b5c6-111">Attributes</span></span>

|<span data-ttu-id="8b5c6-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-112">**Attribute**</span></span>|<span data-ttu-id="8b5c6-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8b5c6-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="8b5c6-115">Описание состояния ответа [DeleteItem операции](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="8b5c6-115">Describes the status of a [DeleteItem operation](deleteitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="8b5c6-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="8b5c6-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="8b5c6-117">-Success</span><span class="sxs-lookup"><span data-stu-id="8b5c6-117">- Success</span></span>  <br/><span data-ttu-id="8b5c6-118">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="8b5c6-118">-  Warning</span></span>  <br/><span data-ttu-id="8b5c6-119">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="8b5c6-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="8b5c6-120">Атрибут ResponseClass</span><span class="sxs-lookup"><span data-stu-id="8b5c6-120">ResponseClass attribute</span></span>

|<span data-ttu-id="8b5c6-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-121">**Value**</span></span>|<span data-ttu-id="8b5c6-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8b5c6-123">**Успех**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-123">**Success**</span></span> <br/> |<span data-ttu-id="8b5c6-124">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="8b5c6-125">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-125">**Warning**</span></span> <br/> | <span data-ttu-id="8b5c6-126">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-126">Describes a request that was not processed.</span></span> <span data-ttu-id="8b5c6-127">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="8b5c6-128">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="8b5c6-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="8b5c6-129">-В хранилище Exchange переходит в автономный режим во время пакета.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="8b5c6-130">-Доменных служб active Directory (AD DS) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="8b5c6-131">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="8b5c6-132">-База данных сообщений (MDB) переходит в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="8b5c6-133">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="8b5c6-134">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="8b5c6-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-135">**Error**</span></span> <br/> | <span data-ttu-id="8b5c6-136">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="8b5c6-137">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="8b5c6-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="8b5c6-138">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8b5c6-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="8b5c6-139">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="8b5c6-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="8b5c6-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="8b5c6-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="8b5c6-141">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="8b5c6-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="8b5c6-142">— Это клиент попытка задать уровень ведения журнала ошибок выше максимальный уровень, которое разрешено администратором</span><span class="sxs-lookup"><span data-stu-id="8b5c6-142">-  A client attempt to set the error logging level above the maximum level that is permitted by the administrator</span></span>  <br/><span data-ttu-id="8b5c6-143">— Это клиент попытка задать уровень серьезности ошибки ниже уровня по умолчанию, которое задано администратором</span><span class="sxs-lookup"><span data-stu-id="8b5c6-143">-  A client attempt to set the severity failure level below the default level that is specified by the administrator</span></span>  <br/><span data-ttu-id="8b5c6-144">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="8b5c6-144">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="8b5c6-145">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="8b5c6-145">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="8b5c6-146">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-146">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8b5c6-147">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8b5c6-147">Child elements</span></span>

|<span data-ttu-id="8b5c6-148">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-148">**Element**</span></span>|<span data-ttu-id="8b5c6-149">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-149">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b5c6-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="8b5c6-150">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8b5c6-151">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-151">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8b5c6-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8b5c6-152">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8b5c6-153">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-153">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="8b5c6-154">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8b5c6-154">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8b5c6-155">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-155">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="8b5c6-156">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-156">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="8b5c6-157">MessageXml</span><span class="sxs-lookup"><span data-stu-id="8b5c6-157">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8b5c6-158">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-158">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b5c6-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8b5c6-159">Parent elements</span></span>

|<span data-ttu-id="8b5c6-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-160">**Element**</span></span>|<span data-ttu-id="8b5c6-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b5c6-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b5c6-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8b5c6-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="8b5c6-163">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8b5c6-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="8b5c6-164">Remarks</span></span>

<span data-ttu-id="8b5c6-165">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="8b5c6-166">Различия версий</span><span class="sxs-lookup"><span data-stu-id="8b5c6-166">Version differences</span></span>

<span data-ttu-id="8b5c6-167">В версиях Exchange, начиная с построения 15.00.0986.00 **DeleteItemResponseMessage** элемент имеет тип **DeleteItemResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-167">In versions of Exchange starting with build 15.00.0986.00, the **DeleteItemResponseMessage** element is of type **DeleteItemResponseMessageType**.</span></span> <span data-ttu-id="8b5c6-168">В предыдущих версиях элемент имеет тип **ResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="8b5c6-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b5c6-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8b5c6-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b5c6-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8b5c6-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8b5c6-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8b5c6-171">Schema Name</span></span>  <br/> |<span data-ttu-id="8b5c6-172">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8b5c6-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8b5c6-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8b5c6-173">Validation File</span></span>  <br/> |<span data-ttu-id="8b5c6-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8b5c6-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8b5c6-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8b5c6-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b5c6-176">False</span><span class="sxs-lookup"><span data-stu-id="8b5c6-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b5c6-177">См. также</span><span class="sxs-lookup"><span data-stu-id="8b5c6-177">See also</span></span>

- [<span data-ttu-id="8b5c6-178">Операция DeleteItem</span><span class="sxs-lookup"><span data-stu-id="8b5c6-178">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="8b5c6-179">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="8b5c6-179">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="8b5c6-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8b5c6-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="8b5c6-181">Удаление элементов (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="8b5c6-181">Deleting Items (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

