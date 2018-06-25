---
title: FolderIds
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
description: Элемент FolderIds содержит массив идентификаторов папок, которые используются для определения папок для копирования, перемещение, получение, удаление или отслеживание уведомлений о событиях.
ms.openlocfilehash: 911a74ca778ee988c270c16c67620a40656d82d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762623"
---
# <a name="folderids"></a><span data-ttu-id="28e7a-103">FolderIds</span><span class="sxs-lookup"><span data-stu-id="28e7a-103">FolderIds</span></span>

<span data-ttu-id="28e7a-104">Элемент **FolderIds** содержит массив идентификаторов папок, которые используются для определения папок для копирования, перемещение, получение, удаление или отслеживание уведомлений о событиях.</span><span class="sxs-lookup"><span data-stu-id="28e7a-104">The **FolderIds** element contains an array of folder identifiers that are used to identify folders to copy, move, get, delete, or monitor for event notifications.</span></span> 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 <span data-ttu-id="28e7a-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="28e7a-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28e7a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="28e7a-106">Attributes and elements</span></span>

<span data-ttu-id="28e7a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="28e7a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28e7a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="28e7a-108">Attributes</span></span>

<span data-ttu-id="28e7a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="28e7a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28e7a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="28e7a-110">Child elements</span></span>

|<span data-ttu-id="28e7a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28e7a-111">**Element**</span></span>|<span data-ttu-id="28e7a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28e7a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28e7a-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="28e7a-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="28e7a-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="28e7a-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="28e7a-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="28e7a-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="28e7a-116">Идентифицирует папок Microsoft Exchange Server, которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="28e7a-116">Identifies Microsoft Exchange Server folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28e7a-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="28e7a-117">Parent elements</span></span>

|<span data-ttu-id="28e7a-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28e7a-118">**Element**</span></span>|<span data-ttu-id="28e7a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28e7a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28e7a-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="28e7a-120">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="28e7a-121">Определяет запрос на получение папки из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="28e7a-121">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="28e7a-122">Ниже приведен выражение XPath для этого элемента.`/GetFolder`</span><span class="sxs-lookup"><span data-stu-id="28e7a-122">The following is the XPath expression to this element:  `/GetFolder`</span></span> <br/> |
|[<span data-ttu-id="28e7a-123">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="28e7a-123">DeleteFolder</span></span>](deletefolder.md) <br/> |<span data-ttu-id="28e7a-124">Определяет запрос на удаление папок из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="28e7a-124">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="28e7a-125">Ниже приведен выражение XPath для этого элемента.`/DeleteFolder`</span><span class="sxs-lookup"><span data-stu-id="28e7a-125">The following is the XPath expression to this element:  `/DeleteFolder`</span></span> <br/> |
|[<span data-ttu-id="28e7a-126">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="28e7a-126">EmptyFolder</span></span>](emptyfolder.md) <br/> |<span data-ttu-id="28e7a-127">Определяет запрос на удаление папок из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="28e7a-127">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="28e7a-128">Ниже приведен выражение XPath для этого элемента.`/EmptyFolder`</span><span class="sxs-lookup"><span data-stu-id="28e7a-128">The following is the XPath expression to this element:  `/EmptyFolder`</span></span> <br/> |
|[<span data-ttu-id="28e7a-129">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="28e7a-129">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="28e7a-130">Определяет запрос на перемещение в папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="28e7a-130">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="28e7a-131">Ниже приведен выражение XPath для этого элемента.`/MoveFolder`</span><span class="sxs-lookup"><span data-stu-id="28e7a-131">The following is the XPath expression to this element:  `/MoveFolder`</span></span> <br/> |
|[<span data-ttu-id="28e7a-132">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="28e7a-132">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="28e7a-133">Определяет запрос для копирования в папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="28e7a-133">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="28e7a-134">Ниже приведен выражение XPath для этого элемента.`/CopyFolder`</span><span class="sxs-lookup"><span data-stu-id="28e7a-134">The following is the XPath expression to this element:  `/CopyFolder`</span></span> <br/> |
|[<span data-ttu-id="28e7a-135">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="28e7a-135">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="28e7a-136">Представляет подписка на подписку на уведомления о принудительной события.</span><span class="sxs-lookup"><span data-stu-id="28e7a-136">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="28e7a-137">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="28e7a-137">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="28e7a-138">Представляет подписка на подписку на уведомления о событий на основе репликации по запросу.</span><span class="sxs-lookup"><span data-stu-id="28e7a-138">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="28e7a-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="28e7a-139">Remarks</span></span>

<span data-ttu-id="28e7a-140">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="28e7a-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28e7a-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="28e7a-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28e7a-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="28e7a-142">Namespace</span></span>  <br/> |<span data-ttu-id="28e7a-143">http://schemas.microsoft.com/exchange/services/2006/messages и http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="28e7a-143">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="28e7a-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="28e7a-144">Schema Name</span></span>  <br/> |<span data-ttu-id="28e7a-145">Схема сообщения; Типы схемы</span><span class="sxs-lookup"><span data-stu-id="28e7a-145">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="28e7a-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="28e7a-146">Validation File</span></span>  <br/> |<span data-ttu-id="28e7a-147">Messages.xsd; Types.xsd</span><span class="sxs-lookup"><span data-stu-id="28e7a-147">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="28e7a-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="28e7a-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="28e7a-149">False</span><span class="sxs-lookup"><span data-stu-id="28e7a-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28e7a-150">См. также</span><span class="sxs-lookup"><span data-stu-id="28e7a-150">See also</span></span>



[<span data-ttu-id="28e7a-151">GetFolder Operation</span><span class="sxs-lookup"><span data-stu-id="28e7a-151">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="28e7a-152">Операция DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="28e7a-152">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="28e7a-153">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="28e7a-153">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="28e7a-154">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="28e7a-154">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="28e7a-155">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="28e7a-155">Subscribe operation</span></span>](subscribe-operation.md)

