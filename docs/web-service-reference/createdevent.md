---
title: CreatedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreatedEvent
api_type:
- schema
ms.assetid: f0e53a53-c352-42a5-8280-cd808b0e961b
description: CreatedEvent элемент представляет событие, в котором создается элемента или папки.
ms.openlocfilehash: f52516090d0789b4dd9fc1ced824786ce000e885
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761864"
---
# <a name="createdevent"></a><span data-ttu-id="54458-103">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="54458-103">CreatedEvent</span></span>

<span data-ttu-id="54458-104">**CreatedEvent** элемент представляет событие, в котором создается элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="54458-104">The **CreatedEvent** element represents an event in which an item or folder is created.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

 <span data-ttu-id="54458-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="54458-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54458-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="54458-106">Attributes and elements</span></span>

<span data-ttu-id="54458-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="54458-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54458-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="54458-108">Attributes</span></span>

<span data-ttu-id="54458-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="54458-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54458-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="54458-110">Child elements</span></span>

|<span data-ttu-id="54458-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54458-111">**Element**</span></span>|<span data-ttu-id="54458-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54458-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54458-113">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="54458-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="54458-114">Представляет закладку события в таблице событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="54458-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="54458-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="54458-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="54458-116">Представляет отметки времени событии создания элемента или папки почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="54458-116">Represents the timestamp of a created item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="54458-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="54458-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="54458-118">Представляет идентификатор созданного папки.</span><span class="sxs-lookup"><span data-stu-id="54458-118">Represents the identifier of the created folder.</span></span>  <br/> |
|[<span data-ttu-id="54458-119">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="54458-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="54458-120">Представляет идентификатор созданного элемента.</span><span class="sxs-lookup"><span data-stu-id="54458-120">Represents the identifier of the created item.</span></span>  <br/> |
|[<span data-ttu-id="54458-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="54458-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="54458-122">Представляет идентификатор родительской папки, созданной элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="54458-122">Represents the identifier of the parent folder of the created item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54458-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="54458-123">Parent elements</span></span>

|<span data-ttu-id="54458-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54458-124">**Element**</span></span>|<span data-ttu-id="54458-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54458-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54458-126">Уведомление</span><span class="sxs-lookup"><span data-stu-id="54458-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="54458-127">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="54458-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54458-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="54458-128">Remarks</span></span>

<span data-ttu-id="54458-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="54458-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54458-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="54458-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54458-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="54458-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54458-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="54458-132">Schema name</span></span>  <br/> |<span data-ttu-id="54458-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="54458-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="54458-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="54458-134">Validation file</span></span>  <br/> |<span data-ttu-id="54458-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="54458-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="54458-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="54458-136">Can be empty</span></span>  <br/> |<span data-ttu-id="54458-137">False</span><span class="sxs-lookup"><span data-stu-id="54458-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54458-138">См. также</span><span class="sxs-lookup"><span data-stu-id="54458-138">See also</span></span>



[<span data-ttu-id="54458-139">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="54458-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="54458-140">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="54458-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="54458-141">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="54458-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="54458-142">С помощью подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="54458-142">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="54458-143">Уведомления о событиях в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="54458-143">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

