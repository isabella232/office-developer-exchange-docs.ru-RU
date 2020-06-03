---
title: копифолдерреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponseMessage
api_type:
- schema
ms.assetid: c82092a9-50ff-4ae1-b819-ebabbf89262b
description: Элемент Копифолдерреспонсемессаже содержит состояние и результат одного запроса операции CopyFolder.
ms.openlocfilehash: 796ec57116e4b4943ca370e45cf0abefe7782c08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458511"
---
# <a name="copyfolderresponsemessage"></a><span data-ttu-id="ea88f-103">копифолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ea88f-103">CopyFolderResponseMessage</span></span>

<span data-ttu-id="ea88f-104">Элемент **копифолдерреспонсемессаже** содержит состояние и результат одного запроса [операции CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ea88f-104">The **CopyFolderResponseMessage** element contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="ea88f-105">копифолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="ea88f-105">CopyFolderResponse</span></span>](copyfolderresponse.md) 
- [<span data-ttu-id="ea88f-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="ea88f-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="ea88f-107">копифолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ea88f-107">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
  
```xml
<CopyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CopyFolderResponseMessage>
```

 <span data-ttu-id="ea88f-108">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="ea88f-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea88f-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ea88f-109">Attributes and elements</span></span>

<span data-ttu-id="ea88f-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ea88f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea88f-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ea88f-111">Attributes</span></span>

|<span data-ttu-id="ea88f-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ea88f-112">**Attribute**</span></span>|<span data-ttu-id="ea88f-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea88f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea88f-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="ea88f-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ea88f-115">Описывает состояние ответа [операции CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ea88f-115">Describes the status of a [CopyFolder operation](copyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="ea88f-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="ea88f-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="ea88f-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="ea88f-117">- Success</span></span>  <br/><span data-ttu-id="ea88f-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="ea88f-118">-  Warning</span></span>  <br/><span data-ttu-id="ea88f-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="ea88f-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="ea88f-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="ea88f-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="ea88f-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="ea88f-121">**Value**</span></span>|<span data-ttu-id="ea88f-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea88f-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea88f-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="ea88f-123">**Success**</span></span> <br/> |<span data-ttu-id="ea88f-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="ea88f-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ea88f-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="ea88f-125">**Warning**</span></span> <br/> | <span data-ttu-id="ea88f-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="ea88f-126">Describes a request that was not processed.</span></span> <span data-ttu-id="ea88f-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="ea88f-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="ea88f-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="ea88f-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="ea88f-129">— Хранилище Exchange в пакетном режиме переключается в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="ea88f-129">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="ea88f-130">-Доменные службы Active Directory (AD DS) переключаются в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="ea88f-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="ea88f-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="ea88f-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="ea88f-132">— База данных сообщений (MDB) переводится в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="ea88f-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="ea88f-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="ea88f-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="ea88f-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="ea88f-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="ea88f-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="ea88f-135">**Error**</span></span> <br/> | <span data-ttu-id="ea88f-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="ea88f-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="ea88f-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="ea88f-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="ea88f-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="ea88f-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ea88f-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="ea88f-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="ea88f-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="ea88f-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="ea88f-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="ea88f-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="ea88f-142">— Несанкционированный доступ попытался любому клиенту</span><span class="sxs-lookup"><span data-stu-id="ea88f-142">-  Unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="ea88f-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="ea88f-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="ea88f-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="ea88f-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ea88f-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ea88f-145">Child elements</span></span>

|<span data-ttu-id="ea88f-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea88f-146">**Element**</span></span>|<span data-ttu-id="ea88f-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea88f-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea88f-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="ea88f-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ea88f-149">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="ea88f-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ea88f-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="ea88f-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ea88f-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="ea88f-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ea88f-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="ea88f-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ea88f-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="ea88f-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="ea88f-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="ea88f-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ea88f-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="ea88f-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ea88f-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="ea88f-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ea88f-157">Folders</span><span class="sxs-lookup"><span data-stu-id="ea88f-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ea88f-158">Содержит массив скопированных папок.</span><span class="sxs-lookup"><span data-stu-id="ea88f-158">Contains an array of copied folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea88f-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ea88f-159">Parent elements</span></span>

|<span data-ttu-id="ea88f-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea88f-160">**Element**</span></span>|<span data-ttu-id="ea88f-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea88f-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea88f-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="ea88f-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ea88f-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea88f-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ea88f-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="ea88f-164">Remarks</span></span>

<span data-ttu-id="ea88f-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ea88f-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea88f-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ea88f-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea88f-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ea88f-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ea88f-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ea88f-168">Schema name</span></span>  <br/> |<span data-ttu-id="ea88f-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ea88f-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ea88f-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ea88f-170">Validation file</span></span>  <br/> |<span data-ttu-id="ea88f-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ea88f-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ea88f-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ea88f-172">Can be empty</span></span>  <br/> |<span data-ttu-id="ea88f-173">False</span><span class="sxs-lookup"><span data-stu-id="ea88f-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea88f-174">См. также</span><span class="sxs-lookup"><span data-stu-id="ea88f-174">See also</span></span>

- [<span data-ttu-id="ea88f-175">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="ea88f-175">CopyFolder operation</span></span>](copyfolder-operation.md)
- [<span data-ttu-id="ea88f-176">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="ea88f-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="ea88f-177">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ea88f-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

