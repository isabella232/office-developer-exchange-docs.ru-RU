---
title: ModifiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: ModifiedEvent элемент представляет событие, в котором изменения элемента или папки.
ms.openlocfilehash: fb464fb0a270d8ca7d33d40e5425e260970b2f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834482"
---
# <a name="modifiedevent"></a><span data-ttu-id="ba978-103">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="ba978-103">ModifiedEvent</span></span>

<span data-ttu-id="ba978-104">**ModifiedEvent** элемент представляет событие, в котором изменения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="ba978-104">The **ModifiedEvent** element represents an event in which an item or folder is modified.</span></span> 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

 <span data-ttu-id="ba978-105">**ModifiedEventType**</span><span class="sxs-lookup"><span data-stu-id="ba978-105">**ModifiedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba978-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ba978-106">Attributes and elements</span></span>

<span data-ttu-id="ba978-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ba978-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba978-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ba978-108">Attributes</span></span>

<span data-ttu-id="ba978-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ba978-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba978-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ba978-110">Child elements</span></span>

|<span data-ttu-id="ba978-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ba978-111">**Element**</span></span>|<span data-ttu-id="ba978-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ba978-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba978-113">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="ba978-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="ba978-114">Представляет закладку события в таблице событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="ba978-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="ba978-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="ba978-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="ba978-116">Представляет отметки времени событии изменения элемента или папки почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="ba978-116">Represents the timestamp of a modified item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="ba978-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="ba978-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="ba978-118">Представляет идентификатор измененного папки.</span><span class="sxs-lookup"><span data-stu-id="ba978-118">Represents the identifier of the modified folder.</span></span>  <br/> |
|[<span data-ttu-id="ba978-119">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="ba978-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ba978-120">Представляет идентификатор измененного элемента.</span><span class="sxs-lookup"><span data-stu-id="ba978-120">Represents the identifier of the modified item.</span></span>  <br/> |
|[<span data-ttu-id="ba978-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ba978-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ba978-122">Представляет идентификатор родительской папки изменения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="ba978-122">Represents the identifier of the parent folder of the modified item or folder.</span></span>  <br/> |
|[<span data-ttu-id="ba978-123">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="ba978-123">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="ba978-124">Представляет количество непрочитанных элементов в указанной папке.</span><span class="sxs-lookup"><span data-stu-id="ba978-124">Represents the count of unread items within a given folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ba978-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ba978-125">Parent elements</span></span>

|<span data-ttu-id="ba978-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ba978-126">**Element**</span></span>|<span data-ttu-id="ba978-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ba978-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba978-128">Уведомление</span><span class="sxs-lookup"><span data-stu-id="ba978-128">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ba978-129">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="ba978-129">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ba978-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="ba978-130">Remarks</span></span>

<span data-ttu-id="ba978-131">При каждом изменении элемента в папке создаются два события изменения.</span><span class="sxs-lookup"><span data-stu-id="ba978-131">Two modified events are generated for each modification of an item in a folder.</span></span> <span data-ttu-id="ba978-132">Одно событие предназначенных для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="ba978-132">One event is relevant to the item that changed.</span></span> <span data-ttu-id="ba978-133">Другие события относится к папке родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="ba978-133">The other event is relevant to the parent folder of the item.</span></span> <span data-ttu-id="ba978-134">Это ту же папку, которая была создана подписка.</span><span class="sxs-lookup"><span data-stu-id="ba978-134">This is the same folder that the subscription was created against.</span></span> <span data-ttu-id="ba978-135">Событие, связанное с папкой используется для взаимодействия потенциальных изменение свойства [UnreadCount](unreadcount.md) в общей папке.</span><span class="sxs-lookup"><span data-stu-id="ba978-135">The event that is associated with the folder is used to communicate a potential change to the [UnreadCount](unreadcount.md) property on the folder.</span></span> 
  
<span data-ttu-id="ba978-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ba978-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba978-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ba978-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba978-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ba978-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba978-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ba978-139">Schema name</span></span>  <br/> |<span data-ttu-id="ba978-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ba978-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba978-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ba978-141">Validation file</span></span>  <br/> |<span data-ttu-id="ba978-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ba978-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba978-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ba978-143">Can be empty</span></span>  <br/> |<span data-ttu-id="ba978-144">False</span><span class="sxs-lookup"><span data-stu-id="ba978-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba978-145">См. также</span><span class="sxs-lookup"><span data-stu-id="ba978-145">See also</span></span>



[<span data-ttu-id="ba978-146">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="ba978-146">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="ba978-147">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="ba978-147">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="ba978-148">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="ba978-148">Unsubscribe operation</span></span>](unsubscribe-operation.md)

