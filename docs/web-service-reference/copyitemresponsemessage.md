---
title: копитемреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItemResponseMessage
api_type:
- schema
ms.assetid: a43fe442-12c8-44ab-912c-8a226c9bb3e7
description: Элемент Копитемреспонсемессаже содержит состояние и результат одного запроса операции CopyItem.
ms.openlocfilehash: 99449a4c05d0b2ea13dfca4235aa5f40d54d1214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466446"
---
# <a name="copyitemresponsemessage"></a><span data-ttu-id="bd391-103">копитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="bd391-103">CopyItemResponseMessage</span></span>

<span data-ttu-id="bd391-104">Элемент **копитемреспонсемессаже** содержит состояние и результат одного запроса [операции CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bd391-104">The **CopyItemResponseMessage** element contains the status and result of a single [CopyItem operation](copyitem-operation.md) request.</span></span> 
  
```xml
<CopyItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CopyItemResponseMessage>
```

 <span data-ttu-id="bd391-105">**итеминфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="bd391-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd391-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bd391-106">Attributes and elements</span></span>

<span data-ttu-id="bd391-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bd391-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd391-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bd391-108">Attributes</span></span>

|<span data-ttu-id="bd391-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bd391-109">**Attribute**</span></span>|<span data-ttu-id="bd391-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd391-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bd391-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="bd391-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bd391-112">Описывает состояние ответа [операции CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bd391-112">Describes the status of a [CopyItem operation](copyitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="bd391-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="bd391-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="bd391-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="bd391-114">- Success</span></span>  <br/><span data-ttu-id="bd391-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="bd391-115">-  Warning</span></span>  <br/><span data-ttu-id="bd391-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="bd391-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="bd391-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="bd391-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="bd391-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="bd391-118">**Value**</span></span>|<span data-ttu-id="bd391-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd391-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bd391-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="bd391-120">**Success**</span></span> <br/> |<span data-ttu-id="bd391-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="bd391-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bd391-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="bd391-122">**Warning**</span></span> <br/> | <span data-ttu-id="bd391-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="bd391-123">Describes a request that was not processed.</span></span> <span data-ttu-id="bd391-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="bd391-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="bd391-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="bd391-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="bd391-126">— Хранилище Exchange в пакетном режиме переключается в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="bd391-126">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="bd391-127">-Доменные службы Active Directory (AD DS) переключаются в автономный режим.</span><span class="sxs-lookup"><span data-stu-id="bd391-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="bd391-128">— Почтовые ящики перемещаются.</span><span class="sxs-lookup"><span data-stu-id="bd391-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="bd391-129">-База данных почтовых ящиков находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="bd391-129">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="bd391-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="bd391-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="bd391-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="bd391-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="bd391-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="bd391-132">**Error**</span></span> <br/> | <span data-ttu-id="bd391-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="bd391-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="bd391-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="bd391-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="bd391-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="bd391-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="bd391-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="bd391-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="bd391-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="bd391-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="bd391-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="bd391-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="bd391-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="bd391-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="bd391-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="bd391-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="bd391-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="bd391-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bd391-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bd391-142">Child elements</span></span>

|<span data-ttu-id="bd391-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd391-143">**Element**</span></span>|<span data-ttu-id="bd391-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd391-144">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bd391-145">- [XML-элементы EWS в Exchange](ews-xml-elements-in-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="bd391-145">- [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md)</span></span> <br/> [<span data-ttu-id="bd391-146">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="bd391-146">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bd391-147">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="bd391-147">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bd391-148">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bd391-148">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bd391-149">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="bd391-149">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bd391-150">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="bd391-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bd391-151">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="bd391-151">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="bd391-152">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="bd391-152">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bd391-153">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="bd391-153">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bd391-154">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="bd391-154">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="bd391-155">Items</span><span class="sxs-lookup"><span data-stu-id="bd391-155">Items</span></span>](items.md) <br/> |<span data-ttu-id="bd391-156">Содержит массив скопированных элементов</span><span class="sxs-lookup"><span data-stu-id="bd391-156">Contains an array of copied items</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd391-157">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bd391-157">Parent elements</span></span>

|<span data-ttu-id="bd391-158">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd391-158">**Element**</span></span>|<span data-ttu-id="bd391-159">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd391-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd391-160">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="bd391-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bd391-161">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd391-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bd391-162">Примечания</span><span class="sxs-lookup"><span data-stu-id="bd391-162">Remarks</span></span>

<span data-ttu-id="bd391-163">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bd391-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd391-164">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bd391-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd391-165">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bd391-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bd391-166">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bd391-166">Schema name</span></span>  <br/> |<span data-ttu-id="bd391-167">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bd391-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bd391-168">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bd391-168">Validation file</span></span>  <br/> |<span data-ttu-id="bd391-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bd391-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bd391-170">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bd391-170">Can be empty</span></span>  <br/> |<span data-ttu-id="bd391-171">False</span><span class="sxs-lookup"><span data-stu-id="bd391-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd391-172">См. также</span><span class="sxs-lookup"><span data-stu-id="bd391-172">See also</span></span>

- [<span data-ttu-id="bd391-173">Операция CopyItem</span><span class="sxs-lookup"><span data-stu-id="bd391-173">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="bd391-174">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="bd391-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

