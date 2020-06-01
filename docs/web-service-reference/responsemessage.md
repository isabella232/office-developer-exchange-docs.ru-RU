---
title: респонсемессаже
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
description: Элемент Респонсемессаже предоставляет описательные сведения о состоянии отклика для одной сущности в запросе.
ms.openlocfilehash: a7f4240b1e988cb69d67118c6db58db0d7babba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467160"
---
# <a name="responsemessage"></a><span data-ttu-id="8e76f-103">респонсемессаже</span><span class="sxs-lookup"><span data-stu-id="8e76f-103">ResponseMessage</span></span>

<span data-ttu-id="8e76f-104">Элемент **респонсемессаже** предоставляет описательные сведения о состоянии отклика для одной сущности в запросе.</span><span class="sxs-lookup"><span data-stu-id="8e76f-104">The **ResponseMessage** element provides descriptive information about the response status for a single entity within a request.</span></span> 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 <span data-ttu-id="8e76f-105">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e76f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8e76f-106">Attributes and elements</span></span>

<span data-ttu-id="8e76f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8e76f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e76f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8e76f-108">Attributes</span></span>

|<span data-ttu-id="8e76f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8e76f-109">**Attribute**</span></span>|<span data-ttu-id="8e76f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8e76f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8e76f-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="8e76f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="8e76f-112">Представляет состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="8e76f-112">Represents the status of the response.</span></span> <br/><br/><span data-ttu-id="8e76f-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="8e76f-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="8e76f-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="8e76f-114">-  Success</span></span>  <br/><span data-ttu-id="8e76f-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="8e76f-115">-  Warning</span></span>  <br/><span data-ttu-id="8e76f-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="8e76f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="8e76f-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="8e76f-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="8e76f-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="8e76f-118">**Value**</span></span>|<span data-ttu-id="8e76f-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8e76f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8e76f-120">Успешно</span><span class="sxs-lookup"><span data-stu-id="8e76f-120">Success</span></span>  <br/> |<span data-ttu-id="8e76f-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="8e76f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="8e76f-122">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="8e76f-122">Warning</span></span>  <br/> | <span data-ttu-id="8e76f-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="8e76f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="8e76f-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="8e76f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="8e76f-125">Ниже приведены некоторые возможные причины появления предупреждений.</span><span class="sxs-lookup"><span data-stu-id="8e76f-125">The following are some possible causes for warnings:</span></span>  <br/><br/><span data-ttu-id="8e76f-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="8e76f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="8e76f-127">— Служба каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="8e76f-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="8e76f-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="8e76f-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="8e76f-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="8e76f-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="8e76f-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="8e76f-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="8e76f-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="8e76f-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="8e76f-132">Ошибка</span><span class="sxs-lookup"><span data-stu-id="8e76f-132">Error</span></span>  <br/> | <span data-ttu-id="8e76f-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="8e76f-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="8e76f-134">Ниже приведены некоторые возможные причины ошибок.</span><span class="sxs-lookup"><span data-stu-id="8e76f-134">The following are some possible causes for errors:</span></span>  <br/><br/><span data-ttu-id="8e76f-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="8e76f-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="8e76f-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="8e76f-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="8e76f-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="8e76f-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="8e76f-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="8e76f-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="8e76f-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="8e76f-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="8e76f-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="8e76f-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="8e76f-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="8e76f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8e76f-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8e76f-142">Child elements</span></span>

|<span data-ttu-id="8e76f-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8e76f-143">**Element**</span></span>|<span data-ttu-id="8e76f-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8e76f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e76f-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="8e76f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8e76f-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="8e76f-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8e76f-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="8e76f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8e76f-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="8e76f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="8e76f-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="8e76f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8e76f-150">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="8e76f-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="8e76f-151">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="8e76f-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="8e76f-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="8e76f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8e76f-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="8e76f-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8e76f-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8e76f-154">Parent elements</span></span>

|<span data-ttu-id="8e76f-155">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8e76f-155">**Element**</span></span>|<span data-ttu-id="8e76f-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8e76f-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e76f-157">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="8e76f-157">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="8e76f-158">Содержит сведения о доступности для одного пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="8e76f-158">Contains the free/busy information for a single mailbox user.</span></span> <br/> <br/> <span data-ttu-id="8e76f-159">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="8e76f-159">The following is the XPath 2.0 expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[<span data-ttu-id="8e76f-160">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="8e76f-160">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="8e76f-161">Содержит данные ответа и предложения для запрошенных предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="8e76f-161">Contains response information and suggestion data for requested meeting suggestions.</span></span>  <br/><br/> <span data-ttu-id="8e76f-162">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="8e76f-162">The following is the XPath 2.0 expression to this element:</span></span><br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[<span data-ttu-id="8e76f-163">жетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="8e76f-163">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="8e76f-164">Содержит результаты ответа и параметры отсутствия на отсутствие для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e76f-164">Contains the response results and the OOF settings for a user.</span></span>  <br/><br/> <span data-ttu-id="8e76f-165">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="8e76f-165">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[<span data-ttu-id="8e76f-166">сетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="8e76f-166">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md) <br/> |<span data-ttu-id="8e76f-167">Содержит результат предпринятого сообщения [сетусеруфсеттингсрекуест](setuseroofsettingsrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="8e76f-167">Contains the result of an attempted [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message.</span></span> <br/> <br/> <span data-ttu-id="8e76f-168">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="8e76f-168">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8e76f-169">Примечания</span><span class="sxs-lookup"><span data-stu-id="8e76f-169">Remarks</span></span>

<span data-ttu-id="8e76f-170">Тип **респонсемессажетипе** является общим для всех ответов на веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e76f-170">The **ResponseMessageType** type is common to all Exchange Web Services responses.</span></span> <span data-ttu-id="8e76f-171">Тип **респонсемессажетипе** расширяется следующими сложными типами:</span><span class="sxs-lookup"><span data-stu-id="8e76f-171">The **ResponseMessageType** type is extended by the following complex types:</span></span> 
  
- <span data-ttu-id="8e76f-172">**аппликонверсатионактионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-172">**ApplyConversationActionResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-173">**аттачментинфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-173">**AttachmentInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-174">**делетеаттачментреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-174">**DeleteAttachmentResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-175">**делетеитемреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-175">**DeleteItemResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-176">**експанддлреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-176">**ExpandDLResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-177">**финдфолдерреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-177">**FindFolderResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-178">**финдитемреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-178">**FindItemResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-179">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-179">**FolderInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-180">**жетевентсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-180">**GetEventsResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-181">**итеминфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-181">**ItemInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-182">**ресолвенамесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-182">**ResolveNamesResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-183">**субскрибереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-183">**SubscribeResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-184">**сенднотификатионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-184">**SendNotificationResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-185">**синкфолдерхиерарчиреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-185">**SyncFolderHierarchyResponseMessageType**</span></span>
    
- <span data-ttu-id="8e76f-186">**синкфолдеритемсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="8e76f-186">**SyncFolderItemsResponseMessageType**</span></span>
    
<span data-ttu-id="8e76f-187">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8e76f-187">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="8e76f-188">Различия версий</span><span class="sxs-lookup"><span data-stu-id="8e76f-188">Version differences</span></span>

<span data-ttu-id="8e76f-189">Типы **аппликонверсатионактионреспонсемессаже** и **делетеитемреспонсемессажетипе** были представлены в Exchange Build 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="8e76f-189">The **ApplyConversationActionResponseMessage** and **DeleteItemResponseMessageType** types were introduced in Exchange build 15.00.0986.00.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8e76f-190">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8e76f-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e76f-191">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8e76f-191">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8e76f-192">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8e76f-192">Schema Name</span></span>  <br/> |<span data-ttu-id="8e76f-193">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8e76f-193">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8e76f-194">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8e76f-194">Validation File</span></span>  <br/> |<span data-ttu-id="8e76f-195">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8e76f-195">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8e76f-196">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8e76f-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e76f-197">False</span><span class="sxs-lookup"><span data-stu-id="8e76f-197">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e76f-198">См. также</span><span class="sxs-lookup"><span data-stu-id="8e76f-198">See also</span></span>

- [<span data-ttu-id="8e76f-199">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="8e76f-199">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="8e76f-200">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8e76f-200">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="8e76f-201">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8e76f-201">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="8e76f-202">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="8e76f-202">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

