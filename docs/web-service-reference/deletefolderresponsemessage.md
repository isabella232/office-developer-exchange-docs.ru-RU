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
ms.openlocfilehash: 5601fe2e48ad002e0fab60d812e7d70c7398f3ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762038"
---
# <a name="deletefolderresponsemessage"></a><span data-ttu-id="01262-103">делетефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="01262-103">DeleteFolderResponseMessage</span></span>

<span data-ttu-id="01262-104">Элемент **делетефолдерреспонсемессаже** содержит состояние и результат одного запроса [операции DeleteFolder](deletefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="01262-104">The **DeleteFolderResponseMessage** element contains the status and result of a single [DeleteFolder operation](deletefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="01262-105">делетефолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="01262-105">DeleteFolderResponse</span></span>](deletefolderresponse.md)  
- [<span data-ttu-id="01262-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="01262-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="01262-107">делетефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="01262-107">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
  
```xml
<DeleteFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteFolderResponseMessage>
```

 <span data-ttu-id="01262-108">**респонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="01262-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01262-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="01262-109">Attributes and elements</span></span>

<span data-ttu-id="01262-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="01262-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01262-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="01262-111">Attributes</span></span>

|<span data-ttu-id="01262-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="01262-112">**Attribute**</span></span>|<span data-ttu-id="01262-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="01262-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="01262-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="01262-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="01262-115">Описывает состояние ответа [операции DeleteFolder](deletefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="01262-115">Describes the status of a [DeleteFolder operation](deletefolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="01262-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="01262-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="01262-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="01262-117">-  Success</span></span>  <br/><span data-ttu-id="01262-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="01262-118">-  Warning</span></span>  <br/><span data-ttu-id="01262-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="01262-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="01262-120">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="01262-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="01262-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="01262-121">**Value**</span></span>|<span data-ttu-id="01262-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="01262-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="01262-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="01262-123">**Success**</span></span> <br/> |<span data-ttu-id="01262-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="01262-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="01262-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="01262-125">**Warning**</span></span> <br/> | <span data-ttu-id="01262-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="01262-126">Describes a request that was not processed.</span></span> <span data-ttu-id="01262-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="01262-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="01262-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="01262-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="01262-129">— Хранилище Exchange в пакетном режиме переключается в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="01262-129">- The Exchange store goes offline during the batch.</span></span><br/><span data-ttu-id="01262-130">-Доменные службы Active Directory (AD DS) переключаются в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="01262-130">- Active Directory Domain Services (AD DS) goes offline.</span></span><br/><span data-ttu-id="01262-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="01262-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="01262-132">— База данных сообщений (MDB) переводится в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="01262-132">- The message database (MDB) goes offline.</span></span><br/><span data-ttu-id="01262-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="01262-133">- A password is expired.</span></span><br/><span data-ttu-id="01262-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="01262-134">- A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="01262-135">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="01262-135">**Error**</span></span> <br/> | <span data-ttu-id="01262-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="01262-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="01262-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="01262-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="01262-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="01262-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="01262-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="01262-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="01262-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="01262-140">- Unknown tag</span></span><br/><span data-ttu-id="01262-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="01262-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="01262-142">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="01262-142">- Unauthorized access attempt by any client</span></span><br/><span data-ttu-id="01262-143">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="01262-143">- Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="01262-144">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="01262-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="01262-145">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="01262-145">Child elements</span></span>

|<span data-ttu-id="01262-146">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="01262-146">**Element**</span></span>|<span data-ttu-id="01262-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="01262-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01262-148">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="01262-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="01262-149">Текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="01262-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="01262-150">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="01262-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="01262-151">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="01262-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="01262-152">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="01262-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="01262-153">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="01262-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="01262-154">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="01262-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="01262-155">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="01262-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="01262-156">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="01262-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01262-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="01262-157">Parent elements</span></span>

|<span data-ttu-id="01262-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="01262-158">**Element**</span></span>|<span data-ttu-id="01262-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="01262-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01262-160">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="01262-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="01262-161">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="01262-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="01262-162">Примечания</span><span class="sxs-lookup"><span data-stu-id="01262-162">Remarks</span></span>

<span data-ttu-id="01262-163">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="01262-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01262-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="01262-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01262-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="01262-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01262-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="01262-166">Schema Name</span></span>  <br/> |<span data-ttu-id="01262-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="01262-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="01262-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="01262-168">Validation File</span></span>  <br/> |<span data-ttu-id="01262-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="01262-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01262-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="01262-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="01262-171">False</span><span class="sxs-lookup"><span data-stu-id="01262-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01262-172">См. также</span><span class="sxs-lookup"><span data-stu-id="01262-172">See also</span></span>

- [<span data-ttu-id="01262-173">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="01262-173">DeleteFolder operation</span></span>](deletefolder-operation.md)
- [<span data-ttu-id="01262-174">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="01262-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="01262-175">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="01262-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="01262-176">Удаление папок</span><span class="sxs-lookup"><span data-stu-id="01262-176">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

