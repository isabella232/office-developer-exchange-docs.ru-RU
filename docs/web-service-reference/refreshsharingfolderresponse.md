---
title: рефрешшарингфолдерреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolderResponse
api_type:
- schema
ms.assetid: 951ab681-f2d5-4f10-933e-ff199685ff8e
description: Элемент Рефрешшарингфолдерреспонсе определяет ответ на запрос операции RefreshSharingFolder.
ms.openlocfilehash: 4ef7a63b2153c6106dae988439f499046689c2b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835048"
---
# <a name="refreshsharingfolderresponse"></a><span data-ttu-id="702b9-103">рефрешшарингфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="702b9-103">RefreshSharingFolderResponse</span></span>

<span data-ttu-id="702b9-104">Элемент **рефрешшарингфолдерреспонсе** определяет ответ на запрос [операции RefreshSharingFolder](refreshsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="702b9-104">The **RefreshSharingFolderResponse** element defines a response to a [RefreshSharingFolder operation](refreshsharingfolder-operation.md) request.</span></span> 
  
```xml
<RefreshSharingFolderResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponse>
```

 <span data-ttu-id="702b9-105">**рефрешшарингфолдерреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="702b9-105">**RefreshSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="702b9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="702b9-106">Attributes and elements</span></span>

<span data-ttu-id="702b9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="702b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="702b9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="702b9-108">Attributes</span></span>

|<span data-ttu-id="702b9-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="702b9-109">**Attribute**</span></span>|<span data-ttu-id="702b9-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="702b9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="702b9-111">**респонсекласс**</span><span class="sxs-lookup"><span data-stu-id="702b9-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="702b9-112">Описывает состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="702b9-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="702b9-113">Для этого атрибута допустимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="702b9-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="702b9-114">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="702b9-114">-  Success</span></span>  <br/><span data-ttu-id="702b9-115">— Предупреждение</span><span class="sxs-lookup"><span data-stu-id="702b9-115">-  Warning</span></span>  <br/><span data-ttu-id="702b9-116">— Ошибка</span><span class="sxs-lookup"><span data-stu-id="702b9-116">-  Error</span></span>  <br/>- |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="702b9-117">Значения атрибутов Респонсекласс</span><span class="sxs-lookup"><span data-stu-id="702b9-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="702b9-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="702b9-118">**Value**</span></span>|<span data-ttu-id="702b9-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="702b9-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="702b9-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="702b9-120">**Success**</span></span> <br/> |<span data-ttu-id="702b9-121">Описывает выполненный запрос.</span><span class="sxs-lookup"><span data-stu-id="702b9-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="702b9-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="702b9-122">**Warning**</span></span> <br/> | <span data-ttu-id="702b9-123">Описывает запрос, который не был обработан.</span><span class="sxs-lookup"><span data-stu-id="702b9-123">Describes a request that was not processed.</span></span> <span data-ttu-id="702b9-124">Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.</span><span class="sxs-lookup"><span data-stu-id="702b9-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="702b9-125">Ниже приведены примеры источников предупреждений.</span><span class="sxs-lookup"><span data-stu-id="702b9-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="702b9-126">— Хранилище Exchange находится в автономном режиме во время выполнения пакета.</span><span class="sxs-lookup"><span data-stu-id="702b9-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="702b9-127">— Служба каталогов Active Directory находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="702b9-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="702b9-128">— Почтовые ящики были перемещены.</span><span class="sxs-lookup"><span data-stu-id="702b9-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="702b9-129">— База данных сообщений (MDB) находится в автономном режиме.</span><span class="sxs-lookup"><span data-stu-id="702b9-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="702b9-130">— Срок действия пароля истек.</span><span class="sxs-lookup"><span data-stu-id="702b9-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="702b9-131">— Превышена квота.</span><span class="sxs-lookup"><span data-stu-id="702b9-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="702b9-132">**Ошибка**</span><span class="sxs-lookup"><span data-stu-id="702b9-132">**Error**</span></span> <br/> | <span data-ttu-id="702b9-133">Описывает запрос, который не может быть выполнен.</span><span class="sxs-lookup"><span data-stu-id="702b9-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="702b9-134">Ниже приведены примеры источников ошибок.</span><span class="sxs-lookup"><span data-stu-id="702b9-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="702b9-135">— Недопустимые атрибуты или элементы</span><span class="sxs-lookup"><span data-stu-id="702b9-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="702b9-136">— Атрибуты или элементы выходят за пределы допустимого диапазона</span><span class="sxs-lookup"><span data-stu-id="702b9-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="702b9-137">— Неизвестный тег</span><span class="sxs-lookup"><span data-stu-id="702b9-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="702b9-138">— Атрибут или элемент не является допустимым в контексте</span><span class="sxs-lookup"><span data-stu-id="702b9-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="702b9-139">— Попытки несанкционированного доступа, выполняемые любым клиентом;</span><span class="sxs-lookup"><span data-stu-id="702b9-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="702b9-140">Ошибка на стороне сервера в ответ на действительный вызов на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="702b9-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="702b9-141">Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="702b9-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="702b9-142">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="702b9-142">Child elements</span></span>

|<span data-ttu-id="702b9-143">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="702b9-143">**Element**</span></span>|<span data-ttu-id="702b9-144">**Описание**</span><span class="sxs-lookup"><span data-stu-id="702b9-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="702b9-145">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="702b9-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="702b9-146">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="702b9-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="702b9-147">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="702b9-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="702b9-148">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="702b9-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="702b9-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="702b9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="702b9-150">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="702b9-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="702b9-151">Этот элемент содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="702b9-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="702b9-152">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="702b9-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="702b9-153">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="702b9-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="702b9-154">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="702b9-154">Parent elements</span></span>

<span data-ttu-id="702b9-155">Нет.</span><span class="sxs-lookup"><span data-stu-id="702b9-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="702b9-156">Примечания</span><span class="sxs-lookup"><span data-stu-id="702b9-156">Remarks</span></span>

<span data-ttu-id="702b9-157">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="702b9-157">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="702b9-158">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="702b9-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="702b9-159">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="702b9-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="702b9-160">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="702b9-160">Schema Name</span></span>  <br/> |<span data-ttu-id="702b9-161">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="702b9-161">Messages schema</span></span>  <br/> |
|<span data-ttu-id="702b9-162">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="702b9-162">Validation File</span></span>  <br/> |<span data-ttu-id="702b9-163">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="702b9-163">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="702b9-164">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="702b9-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="702b9-165">False</span><span class="sxs-lookup"><span data-stu-id="702b9-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="702b9-166">См. также</span><span class="sxs-lookup"><span data-stu-id="702b9-166">See also</span></span>

- [<span data-ttu-id="702b9-167">Операция RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="702b9-167">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md)
- [<span data-ttu-id="702b9-168">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="702b9-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

