---
title: фолдеридс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: Элемент Фолдеридс содержит массив идентификаторов папок, которые используются для идентификации папок для копирования, перемещения, получения, удаления или отслеживания уведомлений о событиях.
ms.openlocfilehash: 911a74ca778ee988c270c16c67620a40656d82d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762623"
---
# <a name="folderids"></a><span data-ttu-id="55a53-103">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="55a53-103">FolderIds</span></span>

<span data-ttu-id="55a53-104">Элемент **фолдеридс** содержит массив идентификаторов папок, которые используются для идентификации папок для копирования, перемещения, получения, удаления или отслеживания уведомлений о событиях.</span><span class="sxs-lookup"><span data-stu-id="55a53-104">The **FolderIds** element contains an array of folder identifiers that are used to identify folders to copy, move, get, delete, or monitor for event notifications.</span></span> 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 <span data-ttu-id="55a53-105">**нонемптяррайофбасефолдеридстипе**</span><span class="sxs-lookup"><span data-stu-id="55a53-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55a53-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="55a53-106">Attributes and elements</span></span>

<span data-ttu-id="55a53-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="55a53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55a53-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="55a53-108">Attributes</span></span>

<span data-ttu-id="55a53-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="55a53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55a53-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="55a53-110">Child elements</span></span>

|<span data-ttu-id="55a53-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55a53-111">**Element**</span></span>|<span data-ttu-id="55a53-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55a53-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55a53-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="55a53-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="55a53-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="55a53-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="55a53-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="55a53-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="55a53-116">Определяет папки Microsoft Exchange Server, на которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="55a53-116">Identifies Microsoft Exchange Server folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55a53-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="55a53-117">Parent elements</span></span>

|<span data-ttu-id="55a53-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55a53-118">**Element**</span></span>|<span data-ttu-id="55a53-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55a53-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55a53-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="55a53-120">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="55a53-121">Определяет запрос на получение папки из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="55a53-121">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="55a53-122">Ниже приведено выражение XPath для этого элемента:`/GetFolder`</span><span class="sxs-lookup"><span data-stu-id="55a53-122">The following is the XPath expression to this element:  `/GetFolder`</span></span> <br/> |
|[<span data-ttu-id="55a53-123">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="55a53-123">DeleteFolder</span></span>](deletefolder.md) <br/> |<span data-ttu-id="55a53-124">Определяет запрос на удаление папок из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="55a53-124">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="55a53-125">Ниже приведено выражение XPath для этого элемента:`/DeleteFolder`</span><span class="sxs-lookup"><span data-stu-id="55a53-125">The following is the XPath expression to this element:  `/DeleteFolder`</span></span> <br/> |
|[<span data-ttu-id="55a53-126">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="55a53-126">EmptyFolder</span></span>](emptyfolder.md) <br/> |<span data-ttu-id="55a53-127">Определяет запрос на удаление папок из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="55a53-127">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="55a53-128">Ниже приведено выражение XPath для этого элемента:`/EmptyFolder`</span><span class="sxs-lookup"><span data-stu-id="55a53-128">The following is the XPath expression to this element:  `/EmptyFolder`</span></span> <br/> |
|[<span data-ttu-id="55a53-129">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="55a53-129">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="55a53-130">Определяет запрос на перемещение папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="55a53-130">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="55a53-131">Ниже приведено выражение XPath для этого элемента:`/MoveFolder`</span><span class="sxs-lookup"><span data-stu-id="55a53-131">The following is the XPath expression to this element:  `/MoveFolder`</span></span> <br/> |
|[<span data-ttu-id="55a53-132">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="55a53-132">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="55a53-133">Определяет запрос на копирование папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="55a53-133">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="55a53-134">Ниже приведено выражение XPath для этого элемента:`/CopyFolder`</span><span class="sxs-lookup"><span data-stu-id="55a53-134">The following is the XPath expression to this element:  `/CopyFolder`</span></span> <br/> |
|[<span data-ttu-id="55a53-135">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="55a53-135">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="55a53-136">Представляет подписку на подписку на уведомления о событиях на основе push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="55a53-136">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="55a53-137">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="55a53-137">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="55a53-138">Представляет подписку на подписку на уведомления о событиях по запросу.</span><span class="sxs-lookup"><span data-stu-id="55a53-138">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55a53-139">Примечания</span><span class="sxs-lookup"><span data-stu-id="55a53-139">Remarks</span></span>

<span data-ttu-id="55a53-140">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="55a53-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55a53-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="55a53-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55a53-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="55a53-142">Namespace</span></span>  <br/> |<span data-ttu-id="55a53-143">http://schemas.microsoft.com/exchange/services/2006/messages и http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="55a53-143">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="55a53-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="55a53-144">Schema Name</span></span>  <br/> |<span data-ttu-id="55a53-145">Схема сообщений; Схема Types</span><span class="sxs-lookup"><span data-stu-id="55a53-145">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="55a53-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="55a53-146">Validation File</span></span>  <br/> |<span data-ttu-id="55a53-147">Messages. xsd; Types. xsd</span><span class="sxs-lookup"><span data-stu-id="55a53-147">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55a53-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="55a53-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="55a53-149">False</span><span class="sxs-lookup"><span data-stu-id="55a53-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55a53-150">См. также</span><span class="sxs-lookup"><span data-stu-id="55a53-150">See also</span></span>



[<span data-ttu-id="55a53-151">Операция GetFolder</span><span class="sxs-lookup"><span data-stu-id="55a53-151">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="55a53-152">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="55a53-152">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="55a53-153">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="55a53-153">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="55a53-154">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="55a53-154">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="55a53-155">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="55a53-155">Subscribe operation</span></span>](subscribe-operation.md)

