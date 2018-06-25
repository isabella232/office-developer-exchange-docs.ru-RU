---
title: UpdateUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 27728e57-5a9b-4314-ad64-df7869098f62
description: Элемент UpdateUserConfigurationResponseMessage содержит состояние и результат одного запроса UpdateUserConfiguration операции.
ms.openlocfilehash: db26bb4bc821ac9a09c350009ab8132466e759bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840387"
---
# <a name="updateuserconfigurationresponsemessage"></a><span data-ttu-id="96f39-103">UpdateUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="96f39-103">UpdateUserConfigurationResponseMessage</span></span>

<span data-ttu-id="96f39-104">Элемент **UpdateUserConfigurationResponseMessage** содержит состояние и результат одного запроса UpdateUserConfiguration операции.</span><span class="sxs-lookup"><span data-stu-id="96f39-104">The **UpdateUserConfigurationResponseMessage** element contains the status and result of a single UpdateUserConfiguration operation request.</span></span> 
  
```xml
<UpdateUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateUserConfigurationResponseMessage>
```

 <span data-ttu-id="96f39-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="96f39-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96f39-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="96f39-106">Attributes and elements</span></span>

<span data-ttu-id="96f39-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="96f39-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96f39-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="96f39-108">Attributes</span></span>

|<span data-ttu-id="96f39-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="96f39-109">**Attribute**</span></span>|<span data-ttu-id="96f39-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="96f39-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="96f39-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="96f39-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="96f39-112">Описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="96f39-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="96f39-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="96f39-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="96f39-114">-Success</span><span class="sxs-lookup"><span data-stu-id="96f39-114">-  Success</span></span>  <br/><span data-ttu-id="96f39-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="96f39-115">-  Warning</span></span>  <br/><span data-ttu-id="96f39-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="96f39-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="96f39-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="96f39-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="96f39-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="96f39-118">**Value**</span></span>|<span data-ttu-id="96f39-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="96f39-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="96f39-120">**Успех**</span><span class="sxs-lookup"><span data-stu-id="96f39-120">**Success**</span></span> <br/> |<span data-ttu-id="96f39-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="96f39-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="96f39-122">**Предупреждение**</span><span class="sxs-lookup"><span data-stu-id="96f39-122">**Warning**</span></span> <br/> | <span data-ttu-id="96f39-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="96f39-123">Describes a request that was not processed.</span></span> <span data-ttu-id="96f39-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="96f39-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="96f39-125">Ниже приведены примеры источников предупреждений:</span><span class="sxs-lookup"><span data-stu-id="96f39-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="96f39-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="96f39-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="96f39-127">-К службе каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="96f39-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="96f39-128">-Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="96f39-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="96f39-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="96f39-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="96f39-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="96f39-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="96f39-131">-Квоту превышена.</span><span class="sxs-lookup"><span data-stu-id="96f39-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="96f39-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="96f39-132">**Error**</span></span> <br/> | <span data-ttu-id="96f39-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="96f39-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="96f39-134">Ниже приведены примеры источников ошибок:</span><span class="sxs-lookup"><span data-stu-id="96f39-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="96f39-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="96f39-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="96f39-136">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="96f39-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="96f39-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="96f39-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="96f39-138">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="96f39-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="96f39-139">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="96f39-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="96f39-140">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="96f39-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="96f39-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="96f39-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="96f39-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="96f39-142">Child elements</span></span>

|<span data-ttu-id="96f39-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="96f39-143">**Element**</span></span>|<span data-ttu-id="96f39-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="96f39-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96f39-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="96f39-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="96f39-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="96f39-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="96f39-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="96f39-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="96f39-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="96f39-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="96f39-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="96f39-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="96f39-150">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="96f39-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="96f39-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="96f39-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="96f39-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="96f39-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="96f39-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="96f39-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96f39-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="96f39-154">Parent elements</span></span>

|<span data-ttu-id="96f39-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="96f39-155">**Element**</span></span>|<span data-ttu-id="96f39-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="96f39-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96f39-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="96f39-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="96f39-158">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="96f39-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="96f39-159">Замечания</span><span class="sxs-lookup"><span data-stu-id="96f39-159">Remarks</span></span>

<span data-ttu-id="96f39-160">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="96f39-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96f39-161">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="96f39-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96f39-162">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="96f39-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96f39-163">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="96f39-163">Schema Name</span></span>  <br/> |<span data-ttu-id="96f39-164">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="96f39-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="96f39-165">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="96f39-165">Validation File</span></span>  <br/> |<span data-ttu-id="96f39-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96f39-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96f39-167">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="96f39-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="96f39-168">False</span><span class="sxs-lookup"><span data-stu-id="96f39-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96f39-169">См. также</span><span class="sxs-lookup"><span data-stu-id="96f39-169">See also</span></span>

- [<span data-ttu-id="96f39-170">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="96f39-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

