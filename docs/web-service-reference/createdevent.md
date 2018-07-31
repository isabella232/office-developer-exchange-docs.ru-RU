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
ms.openlocfilehash: 791b8af87c0cc8ae7f07850e3a6fedd9975a251e
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353177"
---
# <a name="createdevent"></a><span data-ttu-id="37c55-103">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="37c55-103">CreatedEvent</span></span>

<span data-ttu-id="37c55-104">**CreatedEvent** элемент представляет событие, в котором создается элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="37c55-104">The **CreatedEvent** element represents an event in which an item or folder is created.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
</CreatedEvent>
```

<span data-ttu-id="37c55-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="37c55-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="37c55-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="37c55-106">Attributes and elements</span></span>

<span data-ttu-id="37c55-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="37c55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37c55-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="37c55-108">Attributes</span></span>

<span data-ttu-id="37c55-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="37c55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37c55-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="37c55-110">Child elements</span></span>

|<span data-ttu-id="37c55-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="37c55-111">**Element**</span></span>|<span data-ttu-id="37c55-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="37c55-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37c55-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="37c55-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="37c55-114">Представляет закладку события в таблице событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="37c55-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="37c55-115">TimeStamp</span><span class="sxs-lookup"><span data-stu-id="37c55-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="37c55-116">Представляет отметки времени событии создания элемента или папки почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="37c55-116">Represents the timestamp of a created item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="37c55-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="37c55-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="37c55-118">Представляет идентификатор созданного папки.</span><span class="sxs-lookup"><span data-stu-id="37c55-118">Represents the identifier of the created folder.</span></span>  <br/> |
|[<span data-ttu-id="37c55-119">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="37c55-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="37c55-120">Представляет идентификатор созданного элемента.</span><span class="sxs-lookup"><span data-stu-id="37c55-120">Represents the identifier of the created item.</span></span>  <br/> |
|[<span data-ttu-id="37c55-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="37c55-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="37c55-122">Представляет идентификатор родительской папки, созданной элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="37c55-122">Represents the identifier of the parent folder of the created item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="37c55-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="37c55-123">Parent elements</span></span>

|<span data-ttu-id="37c55-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="37c55-124">**Element**</span></span>|<span data-ttu-id="37c55-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="37c55-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37c55-126">Уведомление</span><span class="sxs-lookup"><span data-stu-id="37c55-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="37c55-127">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="37c55-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="37c55-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="37c55-128">Remarks</span></span>

<span data-ttu-id="37c55-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="37c55-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37c55-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="37c55-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37c55-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="37c55-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37c55-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="37c55-132">Schema name</span></span>  <br/> |<span data-ttu-id="37c55-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="37c55-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="37c55-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="37c55-134">Validation file</span></span>  <br/> |<span data-ttu-id="37c55-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="37c55-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37c55-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="37c55-136">Can be empty</span></span>  <br/> |<span data-ttu-id="37c55-137">False</span><span class="sxs-lookup"><span data-stu-id="37c55-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37c55-138">См. также</span><span class="sxs-lookup"><span data-stu-id="37c55-138">See also</span></span>

- [<span data-ttu-id="37c55-139">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="37c55-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="37c55-140">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="37c55-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="37c55-141">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="37c55-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="37c55-142">С помощью подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="37c55-142">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [<span data-ttu-id="37c55-143">Уведомления о событиях в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="37c55-143">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

