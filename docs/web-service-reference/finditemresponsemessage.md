---
title: финдитемреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItemResponseMessage
api_type:
- schema
ms.assetid: fb2cd399-8a04-4f26-9091-993134ed1d15
description: Элемент Финдитемреспонсемессаже содержит состояние и результат одного запроса операции FindItem.
ms.openlocfilehash: ca941e0c7e5b9b08f6f495ccae0d634d72b8f429
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462537"
---
# <a name="finditemresponsemessage"></a><span data-ttu-id="48b36-103">финдитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="48b36-103">FindItemResponseMessage</span></span>

<span data-ttu-id="48b36-104">Элемент **финдитемреспонсемессаже** содержит состояние и результат одного запроса [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="48b36-104">The **FindItemResponseMessage** element contains the status and result of a single [FindItem operation](finditem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="48b36-105">финдитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="48b36-105">FindItemResponse</span></span>](finditemresponse.md) 
- [<span data-ttu-id="48b36-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="48b36-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="48b36-107">финдитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="48b36-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
```xml
<FindItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindItemResponseMessage>
```

 <span data-ttu-id="48b36-108">**финдитемреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="48b36-108">**FindItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="48b36-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="48b36-109">Attributes and elements</span></span>

<span data-ttu-id="48b36-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="48b36-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48b36-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="48b36-111">Attributes</span></span>

|<span data-ttu-id="48b36-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="48b36-112">**Attribute**</span></span>|<span data-ttu-id="48b36-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="48b36-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="48b36-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="48b36-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="48b36-115">Описывает состояние ответа [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="48b36-115">Describes the status of a [FindItem operation](finditem-operation.md) response.</span></span><br/><br/> <span data-ttu-id="48b36-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="48b36-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="48b36-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="48b36-117">-  Success</span></span>  <br/><span data-ttu-id="48b36-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="48b36-118">-  Warning</span></span>  <br/><span data-ttu-id="48b36-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="48b36-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="48b36-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="48b36-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="48b36-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="48b36-121">**Value**</span></span>|<span data-ttu-id="48b36-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="48b36-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="48b36-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="48b36-123">**Success**</span></span> <br/> |<span data-ttu-id="48b36-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="48b36-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="48b36-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="48b36-125">**Warning**</span></span> <br/> | <span data-ttu-id="48b36-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="48b36-126">Describes a request that was not processed.</span></span> <span data-ttu-id="48b36-127">Если при обработке элемента в запросе возникла ошибка, и последующие элементы не удалось обработать, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="48b36-127">A warning may be returned if an error occurred while processing an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="48b36-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="48b36-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="48b36-129">— Хранилище Exchange в пакетном режиме переключается в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="48b36-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="48b36-130">-Доменные службы Active Directory (AD DS) переключаются в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="48b36-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="48b36-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="48b36-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="48b36-132">— База данных сообщений (MDB) переводится в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="48b36-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="48b36-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="48b36-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="48b36-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="48b36-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="48b36-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="48b36-135">**Error**</span></span> <br/> | <span data-ttu-id="48b36-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="48b36-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="48b36-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="48b36-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="48b36-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="48b36-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="48b36-139">— Атрибуты или элементы, которые выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="48b36-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="48b36-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="48b36-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="48b36-141">— Атрибут или элемент, который не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="48b36-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="48b36-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="48b36-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="48b36-143">— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="48b36-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="48b36-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="48b36-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="48b36-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="48b36-145">Child elements</span></span>

|<span data-ttu-id="48b36-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="48b36-146">**Element**</span></span>|<span data-ttu-id="48b36-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="48b36-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48b36-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="48b36-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="48b36-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="48b36-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="48b36-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="48b36-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="48b36-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="48b36-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="48b36-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="48b36-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="48b36-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="48b36-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="48b36-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="48b36-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="48b36-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="48b36-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="48b36-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="48b36-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="48b36-157">Рутфолдер (Финдитемреспонсемессаже)</span><span class="sxs-lookup"><span data-stu-id="48b36-157">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="48b36-158">Содержит результаты поиска в одной корневой папке во время [операции FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="48b36-158">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="48b36-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="48b36-159">Parent elements</span></span>

|<span data-ttu-id="48b36-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="48b36-160">**Element**</span></span>|<span data-ttu-id="48b36-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="48b36-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48b36-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="48b36-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="48b36-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="48b36-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="48b36-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="48b36-164">Remarks</span></span>

<span data-ttu-id="48b36-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="48b36-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48b36-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="48b36-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48b36-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="48b36-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="48b36-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="48b36-168">Schema name</span></span>  <br/> |<span data-ttu-id="48b36-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="48b36-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="48b36-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="48b36-170">Validation file</span></span>  <br/> |<span data-ttu-id="48b36-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="48b36-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="48b36-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="48b36-172">Can be empty</span></span>  <br/> |<span data-ttu-id="48b36-173">False</span><span class="sxs-lookup"><span data-stu-id="48b36-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48b36-174">См. также</span><span class="sxs-lookup"><span data-stu-id="48b36-174">See also</span></span>

- [<span data-ttu-id="48b36-175">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="48b36-175">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="48b36-176">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="48b36-176">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

