---
title: ResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessage
api_type:
- schema
ms.assetid: bf57265a-d354-4cd7-bbfc-d93e19cbede6
description: Элемент ResponseMessage содержит описательные сведения о состоянии ответа для одной сущности в запросе.
ms.openlocfilehash: 69f1f6f12d10044045b72dd644536e742c479b9e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835191"
---
# <a name="responsemessage"></a><span data-ttu-id="d5721-103">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d5721-103">ResponseMessage</span></span>

<span data-ttu-id="d5721-104">Элемент **ResponseMessage** содержит описательные сведения о состоянии ответа для одной сущности в запросе.</span><span class="sxs-lookup"><span data-stu-id="d5721-104">The **ResponseMessage** element provides descriptive information about the response status for a single entity within a request.</span></span> 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 <span data-ttu-id="d5721-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5721-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d5721-106">Attributes and elements</span></span>

<span data-ttu-id="d5721-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d5721-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5721-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d5721-108">Attributes</span></span>

|<span data-ttu-id="d5721-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d5721-109">**Attribute**</span></span>|<span data-ttu-id="d5721-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d5721-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d5721-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d5721-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d5721-112">Представляет состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d5721-112">Represents the status of the response.</span></span> <br/><br/><span data-ttu-id="d5721-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="d5721-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d5721-114">-Success</span><span class="sxs-lookup"><span data-stu-id="d5721-114">-  Success</span></span>  <br/><span data-ttu-id="d5721-115">-Предупреждение</span><span class="sxs-lookup"><span data-stu-id="d5721-115">-  Warning</span></span>  <br/><span data-ttu-id="d5721-116">-Ошибка</span><span class="sxs-lookup"><span data-stu-id="d5721-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d5721-117">Значения атрибутов ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d5721-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="d5721-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d5721-118">**Value**</span></span>|<span data-ttu-id="d5721-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d5721-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d5721-120">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="d5721-120">Success</span></span>  <br/> |<span data-ttu-id="d5721-121">Описание запроса, который будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="d5721-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d5721-122">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="d5721-122">Warning</span></span>  <br/> | <span data-ttu-id="d5721-123">Описание запроса, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="d5721-123">Describes a request that was not processed.</span></span> <span data-ttu-id="d5721-124">Предупреждение может быть возвращено, если произошла ошибка при обработке элемента в запросе и последующих элементов не удалось обработать.</span><span class="sxs-lookup"><span data-stu-id="d5721-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d5721-125">Ниже приведены возможные причины возникновения предупреждения.</span><span class="sxs-lookup"><span data-stu-id="d5721-125">The following are some possible causes for warnings:</span></span>  <br/><br/><span data-ttu-id="d5721-126">-В хранилище Exchange будут недоступны во время пакета.</span><span class="sxs-lookup"><span data-stu-id="d5721-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d5721-127">-К службе каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d5721-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="d5721-128">-Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="d5721-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="d5721-129">-База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="d5721-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d5721-130">-Пароль просрочен.</span><span class="sxs-lookup"><span data-stu-id="d5721-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="d5721-131">-Превышено квоту.</span><span class="sxs-lookup"><span data-stu-id="d5721-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="d5721-132">Ошибка</span><span class="sxs-lookup"><span data-stu-id="d5721-132">Error</span></span>  <br/> | <span data-ttu-id="d5721-133">Описание запроса, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="d5721-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d5721-134">Ниже приведены возможные причины возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="d5721-134">The following are some possible causes for errors:</span></span>  <br/><br/><span data-ttu-id="d5721-135">-Недопустимый атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d5721-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d5721-136">-Атрибуты или элементы вне диапазона</span><span class="sxs-lookup"><span data-stu-id="d5721-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="d5721-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="d5721-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="d5721-138">-Атрибут или элемент не допускается в контексте</span><span class="sxs-lookup"><span data-stu-id="d5721-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="d5721-139">— Попытка доступа не санкционировано любой клиент</span><span class="sxs-lookup"><span data-stu-id="d5721-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d5721-140">-Сбой сервере в ответ на допустимый вызовов со стороны клиента</span><span class="sxs-lookup"><span data-stu-id="d5721-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="d5721-141">Сведения об ошибке можно найти в [ResponseCode](responsecode.md) и [MessageText](messagetext.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="d5721-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d5721-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d5721-142">Child elements</span></span>

|<span data-ttu-id="d5721-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d5721-143">**Element**</span></span>|<span data-ttu-id="d5721-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d5721-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5721-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="d5721-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d5721-146">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="d5721-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d5721-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d5721-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d5721-148">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="d5721-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d5721-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d5721-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d5721-150">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="d5721-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d5721-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="d5721-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d5721-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d5721-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d5721-153">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="d5721-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5721-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d5721-154">Parent elements</span></span>

|<span data-ttu-id="d5721-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d5721-155">**Element**</span></span>|<span data-ttu-id="d5721-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d5721-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5721-157">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="d5721-157">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="d5721-158">Содержит сведения о доступности для одного почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="d5721-158">Contains the free/busy information for a single mailbox user.</span></span> <br/> <br/> <span data-ttu-id="d5721-159">Ниже приведен выражение XPath 2.0 для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d5721-159">The following is the XPath 2.0 expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[<span data-ttu-id="d5721-160">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="d5721-160">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="d5721-161">Содержит данные сведения и предложения о ответа для запроса предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="d5721-161">Contains response information and suggestion data for requested meeting suggestions.</span></span>  <br/><br/> <span data-ttu-id="d5721-162">Ниже приведен выражение XPath 2.0 для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d5721-162">The following is the XPath 2.0 expression to this element:</span></span><br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[<span data-ttu-id="d5721-163">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="d5721-163">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="d5721-164">Содержит параметры об отсутствии на работе для пользователя и результатов ответа.</span><span class="sxs-lookup"><span data-stu-id="d5721-164">Contains the response results and the OOF settings for a user.</span></span>  <br/><br/> <span data-ttu-id="d5721-165">Ниже приведен выражение XPath 2.0 для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d5721-165">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[<span data-ttu-id="d5721-166">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="d5721-166">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md) <br/> |<span data-ttu-id="d5721-167">Содержит результат попытки сообщение [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d5721-167">Contains the result of an attempted [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message.</span></span> <br/> <br/> <span data-ttu-id="d5721-168">Ниже приведен выражение XPath 2.0 для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d5721-168">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d5721-169">Замечания</span><span class="sxs-lookup"><span data-stu-id="d5721-169">Remarks</span></span>

<span data-ttu-id="d5721-170">Тип **ResponseMessageType** общими для всех ответов веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5721-170">The **ResponseMessageType** type is common to all Exchange Web Services responses.</span></span> <span data-ttu-id="d5721-171">Тип **ResponseMessageType** только следующих сложных типов:</span><span class="sxs-lookup"><span data-stu-id="d5721-171">The **ResponseMessageType** type is extended by the following complex types:</span></span> 
  
- <span data-ttu-id="d5721-172">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-172">**ApplyConversationActionResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-173">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-173">**AttachmentInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-174">**DeleteAttachmentResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-174">**DeleteAttachmentResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-175">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-175">**DeleteItemResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-176">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-176">**ExpandDLResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-177">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-177">**FindFolderResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-178">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-178">**FindItemResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-179">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-179">**FolderInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-180">**GetEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-180">**GetEventsResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-181">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-181">**ItemInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-182">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-182">**ResolveNamesResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-183">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-183">**SubscribeResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-184">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-184">**SendNotificationResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-185">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-185">**SyncFolderHierarchyResponseMessageType**</span></span>
    
- <span data-ttu-id="d5721-186">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d5721-186">**SyncFolderItemsResponseMessageType**</span></span>
    
<span data-ttu-id="d5721-187">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d5721-187">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="d5721-188">Различия версий</span><span class="sxs-lookup"><span data-stu-id="d5721-188">Version differences</span></span>

<span data-ttu-id="d5721-189">Типы **ApplyConversationActionResponseMessage** и **DeleteItemResponseMessageType** были представлены в Exchange построения 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="d5721-189">The **ApplyConversationActionResponseMessage** and **DeleteItemResponseMessageType** types were introduced in Exchange build 15.00.0986.00.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d5721-190">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d5721-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5721-191">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d5721-191">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d5721-192">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d5721-192">Schema Name</span></span>  <br/> |<span data-ttu-id="d5721-193">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d5721-193">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d5721-194">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d5721-194">Validation File</span></span>  <br/> |<span data-ttu-id="d5721-195">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d5721-195">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d5721-196">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d5721-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5721-197">False</span><span class="sxs-lookup"><span data-stu-id="d5721-197">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5721-198">См. также</span><span class="sxs-lookup"><span data-stu-id="d5721-198">See also</span></span>

- [<span data-ttu-id="d5721-199">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d5721-199">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="d5721-200">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d5721-200">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="d5721-201">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d5721-201">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="d5721-202">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="d5721-202">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

