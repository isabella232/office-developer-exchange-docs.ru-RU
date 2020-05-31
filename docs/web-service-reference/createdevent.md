---
title: креатедевент
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
description: Элемент Креатедевент представляет событие, в котором создается элемент или папка.
ms.openlocfilehash: 791b8af87c0cc8ae7f07850e3a6fedd9975a251e
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353177"
---
# <a name="createdevent"></a><span data-ttu-id="3c8ce-103">креатедевент</span><span class="sxs-lookup"><span data-stu-id="3c8ce-103">CreatedEvent</span></span>

<span data-ttu-id="3c8ce-104">Элемент **креатедевент** представляет событие, в котором создается элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="3c8ce-104">The **CreatedEvent** element represents an event in which an item or folder is created.</span></span> 
  
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

<span data-ttu-id="3c8ce-105">**басеобжектчанжедевенттипе**</span><span class="sxs-lookup"><span data-stu-id="3c8ce-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3c8ce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3c8ce-106">Attributes and elements</span></span>

<span data-ttu-id="3c8ce-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3c8ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c8ce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3c8ce-108">Attributes</span></span>

<span data-ttu-id="3c8ce-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3c8ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c8ce-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3c8ce-110">Child elements</span></span>

|<span data-ttu-id="3c8ce-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3c8ce-111">**Element**</span></span>|<span data-ttu-id="3c8ce-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3c8ce-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c8ce-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="3c8ce-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="3c8ce-114">Представляет закладку события в таблице событий почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="3c8ce-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="3c8ce-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="3c8ce-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="3c8ce-116">Представляет метку времени для созданного события почтового ящика элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="3c8ce-116">Represents the timestamp of a created item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="3c8ce-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="3c8ce-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="3c8ce-118">Представляет идентификатор созданной папки.</span><span class="sxs-lookup"><span data-stu-id="3c8ce-118">Represents the identifier of the created folder.</span></span>  <br/> |
|[<span data-ttu-id="3c8ce-119">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3c8ce-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3c8ce-120">Представляет идентификатор созданного элемента.</span><span class="sxs-lookup"><span data-stu-id="3c8ce-120">Represents the identifier of the created item.</span></span>  <br/> |
|[<span data-ttu-id="3c8ce-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="3c8ce-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="3c8ce-122">Представляет идентификатор родительской папки созданного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="3c8ce-122">Represents the identifier of the parent folder of the created item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c8ce-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3c8ce-123">Parent elements</span></span>

|<span data-ttu-id="3c8ce-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3c8ce-124">**Element**</span></span>|<span data-ttu-id="3c8ce-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3c8ce-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c8ce-126">Уведомление</span><span class="sxs-lookup"><span data-stu-id="3c8ce-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3c8ce-127">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="3c8ce-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3c8ce-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="3c8ce-128">Remarks</span></span>

<span data-ttu-id="3c8ce-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3c8ce-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c8ce-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3c8ce-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c8ce-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3c8ce-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c8ce-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3c8ce-132">Schema name</span></span>  <br/> |<span data-ttu-id="3c8ce-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3c8ce-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c8ce-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3c8ce-134">Validation file</span></span>  <br/> |<span data-ttu-id="3c8ce-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3c8ce-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c8ce-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3c8ce-136">Can be empty</span></span>  <br/> |<span data-ttu-id="3c8ce-137">False</span><span class="sxs-lookup"><span data-stu-id="3c8ce-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c8ce-138">См. также</span><span class="sxs-lookup"><span data-stu-id="3c8ce-138">See also</span></span>

- [<span data-ttu-id="3c8ce-139">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="3c8ce-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="3c8ce-140">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="3c8ce-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="3c8ce-141">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="3c8ce-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="3c8ce-142">Использование подписок по запросу</span><span class="sxs-lookup"><span data-stu-id="3c8ce-142">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [<span data-ttu-id="3c8ce-143">Уведомления о событиях в EWS</span><span class="sxs-lookup"><span data-stu-id="3c8ce-143">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

