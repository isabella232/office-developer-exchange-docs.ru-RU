---
title: моведевент
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
description: Элемент Моведевент представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.
ms.openlocfilehash: 07f9c02ea194187a9fdfb1e27b19eb311392f51f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353261"
---
# <a name="movedevent"></a><span data-ttu-id="8f85f-103">моведевент</span><span class="sxs-lookup"><span data-stu-id="8f85f-103">MovedEvent</span></span>

<span data-ttu-id="8f85f-104">Элемент **моведевент** представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="8f85f-104">The **MovedEvent** element represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span> 
  
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

```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</MovedEvent>
```


<span data-ttu-id="8f85f-105">**моведкопиедевенттипе**</span><span class="sxs-lookup"><span data-stu-id="8f85f-105">**MovedCopiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8f85f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8f85f-106">Attributes and elements</span></span>

<span data-ttu-id="8f85f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8f85f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f85f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8f85f-108">Attributes</span></span>

<span data-ttu-id="8f85f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8f85f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f85f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8f85f-110">Child elements</span></span>

|<span data-ttu-id="8f85f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8f85f-111">**Element**</span></span>|<span data-ttu-id="8f85f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8f85f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f85f-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="8f85f-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="8f85f-114">Представляет закладку Events в таблице событий почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="8f85f-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="8f85f-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="8f85f-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="8f85f-116">Представляет метку времени для события перемещения элемента/почтового ящика папки.</span><span class="sxs-lookup"><span data-stu-id="8f85f-116">Represents the timestamp of a move item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="8f85f-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="8f85f-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="8f85f-118">Представляет идентификатор перемещенной папки.</span><span class="sxs-lookup"><span data-stu-id="8f85f-118">Represents the identifier of the moved folder.</span></span>  <br/> |
|[<span data-ttu-id="8f85f-119">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="8f85f-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="8f85f-120">Представляет идентификатор перемещенного элемента.</span><span class="sxs-lookup"><span data-stu-id="8f85f-120">Represents the identifier of the moved item.</span></span>  <br/> |
|[<span data-ttu-id="8f85f-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="8f85f-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="8f85f-122">Представляет идентификатор папки, содержащей перемещенный элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="8f85f-122">Represents the identifier of the folder that contains the moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="8f85f-123">олдфолдерид</span><span class="sxs-lookup"><span data-stu-id="8f85f-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="8f85f-124">Содержит идентификатор исходной папки перед ее перемещением или копированием.</span><span class="sxs-lookup"><span data-stu-id="8f85f-124">Contains the folder identifier of the original folder before it was moved or copied.</span></span>  <br/> |
|[<span data-ttu-id="8f85f-125">олдитемид</span><span class="sxs-lookup"><span data-stu-id="8f85f-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="8f85f-126">Содержит уникальный идентификатор исходного элемента перед его перемещением.</span><span class="sxs-lookup"><span data-stu-id="8f85f-126">Contains the unique identifier of the original item before it was moved.</span></span>  <br/> |
|[<span data-ttu-id="8f85f-127">олдпарентфолдерид</span><span class="sxs-lookup"><span data-stu-id="8f85f-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="8f85f-128">Содержит идентификатор исходной родительской папки для перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="8f85f-128">Contains the identifier of the original parent folder of an item or folder that was moved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8f85f-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8f85f-129">Parent elements</span></span>

|<span data-ttu-id="8f85f-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8f85f-130">**Element**</span></span>|<span data-ttu-id="8f85f-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8f85f-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f85f-132">Уведомление</span><span class="sxs-lookup"><span data-stu-id="8f85f-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8f85f-133">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="8f85f-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8f85f-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="8f85f-134">Remarks</span></span>

<span data-ttu-id="8f85f-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8f85f-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f85f-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8f85f-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f85f-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8f85f-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8f85f-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8f85f-138">Schema name</span></span>  <br/> |<span data-ttu-id="8f85f-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8f85f-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="8f85f-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8f85f-140">Validation file</span></span>  <br/> |<span data-ttu-id="8f85f-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8f85f-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8f85f-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8f85f-142">Can be empty</span></span>  <br/> |<span data-ttu-id="8f85f-143">False</span><span class="sxs-lookup"><span data-stu-id="8f85f-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8f85f-144">См. также</span><span class="sxs-lookup"><span data-stu-id="8f85f-144">See also</span></span>

- [<span data-ttu-id="8f85f-145">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="8f85f-145">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="8f85f-146">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="8f85f-146">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="8f85f-147">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="8f85f-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)

