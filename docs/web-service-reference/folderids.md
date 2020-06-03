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
ms.openlocfilehash: ff0476f72c7da088bd2b39f58ab560dcc82197e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530995"
---
# <a name="folderids"></a><span data-ttu-id="35ac5-103">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="35ac5-103">FolderIds</span></span>

<span data-ttu-id="35ac5-104">Элемент **фолдеридс** содержит массив идентификаторов папок, которые используются для идентификации папок для копирования, перемещения, получения, удаления или отслеживания уведомлений о событиях.</span><span class="sxs-lookup"><span data-stu-id="35ac5-104">The **FolderIds** element contains an array of folder identifiers that are used to identify folders to copy, move, get, delete, or monitor for event notifications.</span></span> 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 <span data-ttu-id="35ac5-105">**нонемптяррайофбасефолдеридстипе**</span><span class="sxs-lookup"><span data-stu-id="35ac5-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35ac5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="35ac5-106">Attributes and elements</span></span>

<span data-ttu-id="35ac5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="35ac5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35ac5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="35ac5-108">Attributes</span></span>

<span data-ttu-id="35ac5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="35ac5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35ac5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="35ac5-110">Child elements</span></span>

|<span data-ttu-id="35ac5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="35ac5-111">**Element**</span></span>|<span data-ttu-id="35ac5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="35ac5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35ac5-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="35ac5-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="35ac5-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="35ac5-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="35ac5-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="35ac5-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="35ac5-116">Определяет папки Microsoft Exchange Server, на которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="35ac5-116">Identifies Microsoft Exchange Server folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="35ac5-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="35ac5-117">Parent elements</span></span>

|<span data-ttu-id="35ac5-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="35ac5-118">**Element**</span></span>|<span data-ttu-id="35ac5-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="35ac5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35ac5-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="35ac5-120">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="35ac5-121">Определяет запрос на получение папки из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="35ac5-121">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="35ac5-122">Ниже приведено выражение XPath для этого элемента:`/GetFolder`</span><span class="sxs-lookup"><span data-stu-id="35ac5-122">The following is the XPath expression to this element:  `/GetFolder`</span></span> <br/> |
|[<span data-ttu-id="35ac5-123">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="35ac5-123">DeleteFolder</span></span>](deletefolder.md) <br/> |<span data-ttu-id="35ac5-124">Определяет запрос на удаление папок из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="35ac5-124">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="35ac5-125">Ниже приведено выражение XPath для этого элемента:`/DeleteFolder`</span><span class="sxs-lookup"><span data-stu-id="35ac5-125">The following is the XPath expression to this element:  `/DeleteFolder`</span></span> <br/> |
|[<span data-ttu-id="35ac5-126">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="35ac5-126">EmptyFolder</span></span>](emptyfolder.md) <br/> |<span data-ttu-id="35ac5-127">Определяет запрос на удаление папок из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="35ac5-127">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="35ac5-128">Ниже приведено выражение XPath для этого элемента:`/EmptyFolder`</span><span class="sxs-lookup"><span data-stu-id="35ac5-128">The following is the XPath expression to this element:  `/EmptyFolder`</span></span> <br/> |
|[<span data-ttu-id="35ac5-129">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="35ac5-129">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="35ac5-130">Определяет запрос на перемещение папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="35ac5-130">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="35ac5-131">Ниже приведено выражение XPath для этого элемента:`/MoveFolder`</span><span class="sxs-lookup"><span data-stu-id="35ac5-131">The following is the XPath expression to this element:  `/MoveFolder`</span></span> <br/> |
|[<span data-ttu-id="35ac5-132">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="35ac5-132">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="35ac5-133">Определяет запрос на копирование папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="35ac5-133">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="35ac5-134">Ниже приведено выражение XPath для этого элемента:`/CopyFolder`</span><span class="sxs-lookup"><span data-stu-id="35ac5-134">The following is the XPath expression to this element:  `/CopyFolder`</span></span> <br/> |
|[<span data-ttu-id="35ac5-135">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="35ac5-135">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="35ac5-136">Представляет подписку на подписку на уведомления о событиях на основе push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="35ac5-136">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="35ac5-137">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="35ac5-137">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="35ac5-138">Представляет подписку на подписку на уведомления о событиях по запросу.</span><span class="sxs-lookup"><span data-stu-id="35ac5-138">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="35ac5-139">Примечания</span><span class="sxs-lookup"><span data-stu-id="35ac5-139">Remarks</span></span>

<span data-ttu-id="35ac5-140">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="35ac5-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35ac5-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="35ac5-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35ac5-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="35ac5-142">Namespace</span></span>  <br/> |<span data-ttu-id="35ac5-143">https://schemas.microsoft.com/exchange/services/2006/messages и https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="35ac5-143">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="35ac5-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="35ac5-144">Schema Name</span></span>  <br/> |<span data-ttu-id="35ac5-145">Схема сообщений; Схема Types</span><span class="sxs-lookup"><span data-stu-id="35ac5-145">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="35ac5-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="35ac5-146">Validation File</span></span>  <br/> |<span data-ttu-id="35ac5-147">Messages. xsd; Types. xsd</span><span class="sxs-lookup"><span data-stu-id="35ac5-147">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="35ac5-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="35ac5-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="35ac5-149">False</span><span class="sxs-lookup"><span data-stu-id="35ac5-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="35ac5-150">См. также</span><span class="sxs-lookup"><span data-stu-id="35ac5-150">See also</span></span>



[<span data-ttu-id="35ac5-151">Операция GetFolder</span><span class="sxs-lookup"><span data-stu-id="35ac5-151">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="35ac5-152">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="35ac5-152">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="35ac5-153">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="35ac5-153">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="35ac5-154">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="35ac5-154">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="35ac5-155">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="35ac5-155">Subscribe operation</span></span>](subscribe-operation.md)

