---
title: MovedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MovedEvent
api_type:
- schema
ms.assetid: 572f8b40-dfa8-47bc-b0c1-e1a7138506fd
description: MovedEvent элемент представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.
ms.openlocfilehash: a375f421ca9159103e47b515729316b21149c68a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834479"
---
# <a name="movedevent"></a><span data-ttu-id="3479d-103">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="3479d-103">MovedEvent</span></span>

<span data-ttu-id="3479d-104">**MovedEvent** элемент представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="3479d-104">The **MovedEvent** element represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span> 
  
```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldItemId/>
   <OldParentFolderId/>
</MovedEvent>
```

 <span data-ttu-id="3479d-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="3479d-105">**MovedCopiedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3479d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3479d-106">Attributes and elements</span></span>

<span data-ttu-id="3479d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3479d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3479d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3479d-108">Attributes</span></span>

<span data-ttu-id="3479d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3479d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3479d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3479d-110">Child elements</span></span>

|<span data-ttu-id="3479d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3479d-111">**Element**</span></span>|<span data-ttu-id="3479d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3479d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3479d-113">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="3479d-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="3479d-114">Представляет закладку события в таблице событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3479d-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="3479d-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="3479d-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="3479d-116">Представляет метка времени события перемещения элемента или временная папка почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3479d-116">Represents the timestamp of a move item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="3479d-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="3479d-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="3479d-118">Представляет идентификатор перемещенной папки.</span><span class="sxs-lookup"><span data-stu-id="3479d-118">Represents the identifier of the moved folder.</span></span>  <br/> |
|[<span data-ttu-id="3479d-119">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="3479d-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3479d-120">Представляет идентификатор перемещаемый элемент.</span><span class="sxs-lookup"><span data-stu-id="3479d-120">Represents the identifier of the moved item.</span></span>  <br/> |
|[<span data-ttu-id="3479d-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="3479d-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="3479d-122">Представляет идентификатор папка, содержащая перемещенный элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="3479d-122">Represents the identifier of the folder that contains the moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="3479d-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="3479d-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="3479d-124">Содержит идентификатор папки исходной папки, прежде чем он был перемещен или скопирован.</span><span class="sxs-lookup"><span data-stu-id="3479d-124">Contains the folder identifier of the original folder before it was moved or copied.</span></span>  <br/> |
|[<span data-ttu-id="3479d-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="3479d-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="3479d-126">Содержит уникальный идентификатор исходного элемента, прежде чем был перемещен.</span><span class="sxs-lookup"><span data-stu-id="3479d-126">Contains the unique identifier of the original item before it was moved.</span></span>  <br/> |
|[<span data-ttu-id="3479d-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="3479d-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="3479d-128">Содержит идентификатор исходной родительской папки, элемента или папки, который был перемещен.</span><span class="sxs-lookup"><span data-stu-id="3479d-128">Contains the identifier of the original parent folder of an item or folder that was moved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3479d-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3479d-129">Parent elements</span></span>

|<span data-ttu-id="3479d-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3479d-130">**Element**</span></span>|<span data-ttu-id="3479d-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3479d-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3479d-132">Уведомление</span><span class="sxs-lookup"><span data-stu-id="3479d-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3479d-133">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="3479d-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3479d-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="3479d-134">Remarks</span></span>

<span data-ttu-id="3479d-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3479d-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3479d-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3479d-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3479d-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3479d-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3479d-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3479d-138">Schema name</span></span>  <br/> |<span data-ttu-id="3479d-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3479d-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="3479d-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3479d-140">Validation file</span></span>  <br/> |<span data-ttu-id="3479d-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3479d-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3479d-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3479d-142">Can be empty</span></span>  <br/> |<span data-ttu-id="3479d-143">False</span><span class="sxs-lookup"><span data-stu-id="3479d-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3479d-144">См. также</span><span class="sxs-lookup"><span data-stu-id="3479d-144">See also</span></span>



[<span data-ttu-id="3479d-145">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="3479d-145">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="3479d-146">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="3479d-146">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="3479d-147">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="3479d-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)

