---
title: делетефолдерреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderResponseMessage
api_type:
- schema
ms.assetid: de4c63ff-80b2-40c2-bc06-ef0c23beacd4
description: Элемент Делетефолдерреспонсемессаже содержит состояние и результат одного запроса операции DeleteFolder.
ms.openlocfilehash: 6c593e0d6e8820452bb27a6baa569980e329ef10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455739"
---
# <a name="deletefolderresponsemessage"></a><span data-ttu-id="463df-103">делетефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="463df-103">DeleteFolderResponseMessage</span></span>

<span data-ttu-id="463df-104">Элемент **делетефолдерреспонсемессаже** содержит состояние и результат одного запроса [операции DeleteFolder](deletefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="463df-104">The **DeleteFolderResponseMessage** element contains the status and result of a single [DeleteFolder operation](deletefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="463df-105">делетефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="463df-105">DeleteFolderResponse</span></span>](deletefolderresponse.md)  
- [<span data-ttu-id="463df-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="463df-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="463df-107">делетефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="463df-107">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
  
```xml
<DeleteFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteFolderResponseMessage>
```

 <span data-ttu-id="463df-108">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="463df-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="463df-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="463df-109">Attributes and elements</span></span>

<span data-ttu-id="463df-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="463df-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="463df-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="463df-111">Attributes</span></span>

|<span data-ttu-id="463df-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="463df-112">**Attribute**</span></span>|<span data-ttu-id="463df-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="463df-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="463df-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="463df-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="463df-115">Описывает состояние ответа [операции DeleteFolder](deletefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="463df-115">Describes the status of a [DeleteFolder operation](deletefolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="463df-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="463df-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="463df-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="463df-117">-  Success</span></span>  <br/><span data-ttu-id="463df-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="463df-118">-  Warning</span></span>  <br/><span data-ttu-id="463df-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="463df-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="463df-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="463df-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="463df-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="463df-121">**Value**</span></span>|<span data-ttu-id="463df-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="463df-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="463df-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="463df-123">**Success**</span></span> <br/> |<span data-ttu-id="463df-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="463df-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="463df-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="463df-125">**Warning**</span></span> <br/> | <span data-ttu-id="463df-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="463df-126">Describes a request that was not processed.</span></span> <span data-ttu-id="463df-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="463df-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="463df-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="463df-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="463df-129">— Хранилище Exchange в пакетном режиме переключается в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="463df-129">- The Exchange store goes offline during the batch.</span></span><br/><span data-ttu-id="463df-130">-Доменные службы Active Directory (AD DS) переключаются в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="463df-130">- Active Directory Domain Services (AD DS) goes offline.</span></span><br/><span data-ttu-id="463df-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="463df-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="463df-132">— База данных сообщений (MDB) переводится в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="463df-132">- The message database (MDB) goes offline.</span></span><br/><span data-ttu-id="463df-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="463df-133">- A password is expired.</span></span><br/><span data-ttu-id="463df-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="463df-134">- A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="463df-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="463df-135">**Error**</span></span> <br/> | <span data-ttu-id="463df-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="463df-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="463df-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="463df-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="463df-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="463df-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="463df-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="463df-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="463df-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="463df-140">- Unknown tag</span></span><br/><span data-ttu-id="463df-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="463df-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="463df-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="463df-142">- Unauthorized access attempt by any client</span></span><br/><span data-ttu-id="463df-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="463df-143">- Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="463df-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="463df-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="463df-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="463df-145">Child elements</span></span>

|<span data-ttu-id="463df-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="463df-146">**Element**</span></span>|<span data-ttu-id="463df-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="463df-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="463df-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="463df-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="463df-149">Текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="463df-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="463df-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="463df-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="463df-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="463df-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="463df-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="463df-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="463df-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="463df-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="463df-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="463df-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="463df-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="463df-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="463df-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="463df-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="463df-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="463df-157">Parent elements</span></span>

|<span data-ttu-id="463df-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="463df-158">**Element**</span></span>|<span data-ttu-id="463df-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="463df-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="463df-160">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="463df-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="463df-161">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="463df-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="463df-162">Примечания</span><span class="sxs-lookup"><span data-stu-id="463df-162">Remarks</span></span>

<span data-ttu-id="463df-163">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="463df-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="463df-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="463df-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="463df-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="463df-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="463df-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="463df-166">Schema Name</span></span>  <br/> |<span data-ttu-id="463df-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="463df-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="463df-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="463df-168">Validation File</span></span>  <br/> |<span data-ttu-id="463df-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="463df-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="463df-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="463df-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="463df-171">False</span><span class="sxs-lookup"><span data-stu-id="463df-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="463df-172">См. также</span><span class="sxs-lookup"><span data-stu-id="463df-172">See also</span></span>

- [<span data-ttu-id="463df-173">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="463df-173">DeleteFolder operation</span></span>](deletefolder-operation.md)
- [<span data-ttu-id="463df-174">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="463df-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="463df-175">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="463df-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="463df-176">Удаление папок</span><span class="sxs-lookup"><span data-stu-id="463df-176">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

