---
title: ресолвенамесреспонсемессаже
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
description: Элемент Ресолвенамесреспонсемессаже содержит состояние и результат запроса операции ResolveNames.
ms.openlocfilehash: 12f32008dbbc603fca7adf26057f1f1904d3cfb2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455599"
---
# <a name="resolvenamesresponsemessage"></a><span data-ttu-id="93d64-103">ресолвенамесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="93d64-103">ResolveNamesResponseMessage</span></span>

<span data-ttu-id="93d64-104">Элемент **ресолвенамесреспонсемессаже** содержит состояние и результат запроса [операции ResolveNames](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="93d64-104">The **ResolveNamesResponseMessage** element contains the status and result of a [ResolveNames operation](resolvenames-operation.md) request.</span></span> 
  
- [<span data-ttu-id="93d64-105">ресолвенамесреспонсе</span><span class="sxs-lookup"><span data-stu-id="93d64-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md) 
- [<span data-ttu-id="93d64-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="93d64-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="93d64-107">ресолвенамесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="93d64-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 <span data-ttu-id="93d64-108">**ресолвенамесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="93d64-108">**ResolveNamesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93d64-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93d64-109">Attributes and elements</span></span>

<span data-ttu-id="93d64-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="93d64-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93d64-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93d64-111">Attributes</span></span>

|<span data-ttu-id="93d64-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="93d64-112">**Attribute**</span></span>|<span data-ttu-id="93d64-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93d64-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93d64-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="93d64-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="93d64-115">Описывает состояние ответа [операции ResolveNames](resolvenames-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="93d64-115">Describes the status of a [ResolveNames operation](resolvenames-operation.md) response.</span></span> <br/><br/><span data-ttu-id="93d64-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="93d64-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="93d64-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="93d64-117">-  Success</span></span>  <br/><span data-ttu-id="93d64-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="93d64-118">-  Warning</span></span>  <br/><span data-ttu-id="93d64-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="93d64-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="93d64-120">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="93d64-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="93d64-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="93d64-121">**Value**</span></span>|<span data-ttu-id="93d64-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93d64-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93d64-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="93d64-123">**Success**</span></span> <br/> |<span data-ttu-id="93d64-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="93d64-124">Describes a request that is fulfilled.</span></span> <span data-ttu-id="93d64-125">Это происходит, когда запрошенное имя является неоднозначным и ответ содержит одного получателя.</span><span class="sxs-lookup"><span data-stu-id="93d64-125">This occurs when the requested name is unambiguous and the response contains a single recipient.</span></span>  <br/> |
|<span data-ttu-id="93d64-126">**Warning**</span><span class="sxs-lookup"><span data-stu-id="93d64-126">**Warning**</span></span> <br/> | <span data-ttu-id="93d64-127">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="93d64-127">Describes a request that was not processed.</span></span> <span data-ttu-id="93d64-128">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="93d64-128">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="93d64-129">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="93d64-129">The following are example of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="93d64-130">— Хранилище Exchange в пакетном режиме переключается в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="93d64-130">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="93d64-131">-Доменные службы Active Directory (AD DS) переключаются в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="93d64-131">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="93d64-132">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="93d64-132">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="93d64-133">-База данных почтовых ящиков находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="93d64-133">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="93d64-134">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="93d64-134">-  A password is expired.</span></span>  <br/><span data-ttu-id="93d64-135">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="93d64-135">-  A quota is exceeded.</span></span>  <br/><span data-ttu-id="93d64-136">-Запрошенное имя неоднозначно, а ответ содержит несколько получателей.</span><span class="sxs-lookup"><span data-stu-id="93d64-136">-  The requested name is ambiguous and the response contains multiple recipients.</span></span>  <br/> |
|<span data-ttu-id="93d64-137">**Error**</span><span class="sxs-lookup"><span data-stu-id="93d64-137">**Error**</span></span> <br/> | <span data-ttu-id="93d64-138">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="93d64-138">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="93d64-139">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="93d64-139">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="93d64-140">— Не удалось разрешить запрошенное имя.</span><span class="sxs-lookup"><span data-stu-id="93d64-140">-  The requested name could not be resolved.</span></span>  <br/><span data-ttu-id="93d64-141">Атрибуты или элементы являются недопустимыми.</span><span class="sxs-lookup"><span data-stu-id="93d64-141">-  Attributes or elements are invalid.</span></span>  <br/><span data-ttu-id="93d64-142">— Атрибуты или элементы выходят за пределы допустимого диапазона.</span><span class="sxs-lookup"><span data-stu-id="93d64-142">-  Attributes or elements are out of range.</span></span>  <br/><span data-ttu-id="93d64-143">— Неизвестный тег.</span><span class="sxs-lookup"><span data-stu-id="93d64-143">-  A tag is unknown.</span></span>  <br/><span data-ttu-id="93d64-144">— Недопустимый атрибут или элемент в контексте.</span><span class="sxs-lookup"><span data-stu-id="93d64-144">-  An attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="93d64-145">— Попытки несанкционированного доступа, выполняемые любым клиентом.</span><span class="sxs-lookup"><span data-stu-id="93d64-145">-  An unauthorized access attempt by any client occurred.</span></span>  <br/><span data-ttu-id="93d64-146">— Произошел сбой на стороне сервера в ответ на действительный вызов на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="93d64-146">-  A server-side failure occurred in response to a valid client-side call.</span></span>  <br/>  <br/><span data-ttu-id="93d64-147">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="93d64-147">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="93d64-148">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93d64-148">Child elements</span></span>

|<span data-ttu-id="93d64-149">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93d64-149">**Element**</span></span>|<span data-ttu-id="93d64-150">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93d64-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93d64-151">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="93d64-151">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="93d64-152">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="93d64-152">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="93d64-153">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="93d64-153">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="93d64-154">Предоставляет сведения об ошибке запроса.</span><span class="sxs-lookup"><span data-stu-id="93d64-154">Provides error information about the request.</span></span>  <br/> |
|[<span data-ttu-id="93d64-155">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="93d64-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="93d64-156">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="93d64-156">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="93d64-157">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="93d64-157">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="93d64-158">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="93d64-158">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="93d64-159">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="93d64-159">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="93d64-160">Авторешение</span><span class="sxs-lookup"><span data-stu-id="93d64-160">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="93d64-161">Содержит массив разрешений для неоднозначного имени.</span><span class="sxs-lookup"><span data-stu-id="93d64-161">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93d64-162">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93d64-162">Parent elements</span></span>

|<span data-ttu-id="93d64-163">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93d64-163">**Element**</span></span>|<span data-ttu-id="93d64-164">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93d64-164">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93d64-165">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="93d64-165">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="93d64-166">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="93d64-166">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93d64-167">Примечания</span><span class="sxs-lookup"><span data-stu-id="93d64-167">Remarks</span></span>

<span data-ttu-id="93d64-168">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="93d64-168">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93d64-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93d64-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93d64-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93d64-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93d64-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93d64-171">Schema name</span></span>  <br/> |<span data-ttu-id="93d64-172">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="93d64-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93d64-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93d64-173">Validation file</span></span>  <br/> |<span data-ttu-id="93d64-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="93d64-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93d64-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93d64-175">Can be empty</span></span>  <br/> |<span data-ttu-id="93d64-176">False</span><span class="sxs-lookup"><span data-stu-id="93d64-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93d64-177">См. также</span><span class="sxs-lookup"><span data-stu-id="93d64-177">See also</span></span>

- [<span data-ttu-id="93d64-178">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="93d64-178">ResolveNames</span></span>](resolvenames.md)
- [<span data-ttu-id="93d64-179">ресолвенамесреспонсе</span><span class="sxs-lookup"><span data-stu-id="93d64-179">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
- [<span data-ttu-id="93d64-180">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="93d64-180">ResolveNames operation</span></span>](resolvenames-operation.md)

