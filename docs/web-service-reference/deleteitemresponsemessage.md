---
title: делетеитемреспонсемессаже
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
description: Элемент Делетеитемреспонсемессаже содержит состояние и результат одного запроса операции DeleteItem.
ms.openlocfilehash: 78e3efc6a9e9e6629d7efe7f2dc294e0a731005a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526930"
---
# <a name="deleteitemresponsemessage"></a><span data-ttu-id="bb9dc-103">делетеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="bb9dc-103">DeleteItemResponseMessage</span></span>

<span data-ttu-id="bb9dc-104">Элемент **делетеитемреспонсемессаже** содержит состояние и результат одного запроса [операции DeleteItem](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bb9dc-104">The **DeleteItemResponseMessage** element contains the status and result of a single [DeleteItem operation](deleteitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="bb9dc-105">делетеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="bb9dc-105">DeleteItemResponse</span></span>](deleteitemresponse.md) 
- [<span data-ttu-id="bb9dc-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="bb9dc-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="bb9dc-107">делетеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="bb9dc-107">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 <span data-ttu-id="bb9dc-108">**делетеитемреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-108">**DeleteItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb9dc-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bb9dc-109">Attributes and elements</span></span>

<span data-ttu-id="bb9dc-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb9dc-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bb9dc-111">Attributes</span></span>

|<span data-ttu-id="bb9dc-112">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-112">**Attribute**</span></span>|<span data-ttu-id="bb9dc-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bb9dc-114">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bb9dc-115">Описывает состояние ответа [операции DeleteItem](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bb9dc-115">Describes the status of a [DeleteItem operation](deleteitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="bb9dc-116">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="bb9dc-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="bb9dc-117">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="bb9dc-117">- Success</span></span>  <br/><span data-ttu-id="bb9dc-118">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="bb9dc-118">-  Warning</span></span>  <br/><span data-ttu-id="bb9dc-119">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="bb9dc-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="bb9dc-120">Атрибут Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="bb9dc-120">ResponseClass attribute</span></span>

|<span data-ttu-id="bb9dc-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-121">**Value**</span></span>|<span data-ttu-id="bb9dc-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bb9dc-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-123">**Success**</span></span> <br/> |<span data-ttu-id="bb9dc-124">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bb9dc-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-125">**Warning**</span></span> <br/> | <span data-ttu-id="bb9dc-126">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-126">Describes a request that was not processed.</span></span> <span data-ttu-id="bb9dc-127">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="bb9dc-128">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="bb9dc-129">— Хранилище Exchange в пакетном режиме переключается в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="bb9dc-130">-Доменные службы Active Directory (AD DS) переключаются в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="bb9dc-131">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="bb9dc-132">— База данных сообщений (MDB) переводится в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="bb9dc-133">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="bb9dc-134">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="bb9dc-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-135">**Error**</span></span> <br/> | <span data-ttu-id="bb9dc-136">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="bb9dc-137">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="bb9dc-138">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="bb9dc-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="bb9dc-139">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="bb9dc-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="bb9dc-140">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="bb9dc-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="bb9dc-141">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="bb9dc-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="bb9dc-142">Клиент пытается установить уровень ведения журнала ошибок выше максимального уровня, разрешенного администратором</span><span class="sxs-lookup"><span data-stu-id="bb9dc-142">-  A client attempt to set the error logging level above the maximum level that is permitted by the administrator</span></span>  <br/><span data-ttu-id="bb9dc-143">— Попытка клиента задать уровень серьезности сбоя ниже уровня по умолчанию, указанного администратором.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-143">-  A client attempt to set the severity failure level below the default level that is specified by the administrator</span></span>  <br/><span data-ttu-id="bb9dc-144">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="bb9dc-144">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="bb9dc-145">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="bb9dc-145">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="bb9dc-146">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="bb9dc-146">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bb9dc-147">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bb9dc-147">Child elements</span></span>

|<span data-ttu-id="bb9dc-148">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-148">**Element**</span></span>|<span data-ttu-id="bb9dc-149">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-149">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb9dc-150">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="bb9dc-150">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bb9dc-151">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-151">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bb9dc-152">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bb9dc-152">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bb9dc-153">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-153">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bb9dc-154">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="bb9dc-154">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bb9dc-155">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-155">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="bb9dc-156">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-156">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bb9dc-157">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="bb9dc-157">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bb9dc-158">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-158">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bb9dc-159">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bb9dc-159">Parent elements</span></span>

|<span data-ttu-id="bb9dc-160">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-160">**Element**</span></span>|<span data-ttu-id="bb9dc-161">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bb9dc-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb9dc-162">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="bb9dc-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bb9dc-163">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bb9dc-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="bb9dc-164">Remarks</span></span>

<span data-ttu-id="bb9dc-165">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="bb9dc-166">Различия версий</span><span class="sxs-lookup"><span data-stu-id="bb9dc-166">Version differences</span></span>

<span data-ttu-id="bb9dc-167">В версиях Exchange, начиная с сборки 15.00.0986.00, элемент **делетеитемреспонсемессаже** имеет тип **делетеитемреспонсемессажетипе**.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-167">In versions of Exchange starting with build 15.00.0986.00, the **DeleteItemResponseMessage** element is of type **DeleteItemResponseMessageType**.</span></span> <span data-ttu-id="bb9dc-168">В предыдущих версиях элемент относится к типу **респонсемессажетипе**.</span><span class="sxs-lookup"><span data-stu-id="bb9dc-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb9dc-169">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bb9dc-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb9dc-170">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bb9dc-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bb9dc-171">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bb9dc-171">Schema Name</span></span>  <br/> |<span data-ttu-id="bb9dc-172">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bb9dc-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bb9dc-173">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bb9dc-173">Validation File</span></span>  <br/> |<span data-ttu-id="bb9dc-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bb9dc-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bb9dc-175">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bb9dc-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="bb9dc-176">False</span><span class="sxs-lookup"><span data-stu-id="bb9dc-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb9dc-177">См. также</span><span class="sxs-lookup"><span data-stu-id="bb9dc-177">See also</span></span>

- [<span data-ttu-id="bb9dc-178">Операция DeleteItem</span><span class="sxs-lookup"><span data-stu-id="bb9dc-178">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="bb9dc-179">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="bb9dc-179">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="bb9dc-180">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bb9dc-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="bb9dc-181">Удаление элементов (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="bb9dc-181">Deleting Items (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

