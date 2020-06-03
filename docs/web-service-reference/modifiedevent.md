---
title: модифиедевент
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
description: Элемент Модифиедевент представляет событие, в котором изменяется элемент или папка.
ms.openlocfilehash: 1a798773601a0857b9064c7fa6a532a7a36517ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468553"
---
# <a name="modifiedevent"></a><span data-ttu-id="8a60a-103">модифиедевент</span><span class="sxs-lookup"><span data-stu-id="8a60a-103">ModifiedEvent</span></span>

<span data-ttu-id="8a60a-104">Элемент **модифиедевент** представляет событие, в котором изменяется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="8a60a-104">The **ModifiedEvent** element represents an event in which an item or folder is modified.</span></span> 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/> 
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

<span data-ttu-id="8a60a-105">**модифиедевенттипе**</span><span class="sxs-lookup"><span data-stu-id="8a60a-105">**ModifiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8a60a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8a60a-106">Attributes and elements</span></span>

<span data-ttu-id="8a60a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8a60a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a60a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8a60a-108">Attributes</span></span>

<span data-ttu-id="8a60a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8a60a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a60a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8a60a-110">Child elements</span></span>

|<span data-ttu-id="8a60a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a60a-111">**Element**</span></span>|<span data-ttu-id="8a60a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a60a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a60a-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="8a60a-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="8a60a-114">Представляет закладку события в таблице событий почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="8a60a-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="8a60a-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="8a60a-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="8a60a-116">Представляет метку времени для измененного события элемента или почтового ящика папки.</span><span class="sxs-lookup"><span data-stu-id="8a60a-116">Represents the timestamp of a modified item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="8a60a-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="8a60a-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="8a60a-118">Представляет идентификатор измененной папки.</span><span class="sxs-lookup"><span data-stu-id="8a60a-118">Represents the identifier of the modified folder.</span></span>  <br/> |
|[<span data-ttu-id="8a60a-119">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="8a60a-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="8a60a-120">Представляет идентификатор измененного элемента.</span><span class="sxs-lookup"><span data-stu-id="8a60a-120">Represents the identifier of the modified item.</span></span>  <br/> |
|[<span data-ttu-id="8a60a-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="8a60a-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="8a60a-122">Представляет идентификатор родительской папки измененного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="8a60a-122">Represents the identifier of the parent folder of the modified item or folder.</span></span>  <br/> |
|[<span data-ttu-id="8a60a-123">унреадкаунт</span><span class="sxs-lookup"><span data-stu-id="8a60a-123">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="8a60a-124">Представляет количество непрочитанных элементов в заданной папке.</span><span class="sxs-lookup"><span data-stu-id="8a60a-124">Represents the count of unread items within a given folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a60a-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8a60a-125">Parent elements</span></span>

|<span data-ttu-id="8a60a-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a60a-126">**Element**</span></span>|<span data-ttu-id="8a60a-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a60a-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a60a-128">Уведомление</span><span class="sxs-lookup"><span data-stu-id="8a60a-128">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8a60a-129">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="8a60a-129">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8a60a-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="8a60a-130">Remarks</span></span>

<span data-ttu-id="8a60a-131">Для каждого изменения элемента в папке создается два измененных события.</span><span class="sxs-lookup"><span data-stu-id="8a60a-131">Two modified events are generated for each modification of an item in a folder.</span></span> <span data-ttu-id="8a60a-132">Одно событие относится к измененному элементу.</span><span class="sxs-lookup"><span data-stu-id="8a60a-132">One event is relevant to the item that changed.</span></span> <span data-ttu-id="8a60a-133">Другое событие относится к родительской папке элемента.</span><span class="sxs-lookup"><span data-stu-id="8a60a-133">The other event is relevant to the parent folder of the item.</span></span> <span data-ttu-id="8a60a-134">Это та же папка, в которой была создана подписка.</span><span class="sxs-lookup"><span data-stu-id="8a60a-134">This is the same folder that the subscription was created against.</span></span> <span data-ttu-id="8a60a-135">Событие, связанное с папкой, используется для передачи потенциального изменения свойству [унреадкаунт](unreadcount.md) в папке.</span><span class="sxs-lookup"><span data-stu-id="8a60a-135">The event that is associated with the folder is used to communicate a potential change to the [UnreadCount](unreadcount.md) property on the folder.</span></span> 
  
<span data-ttu-id="8a60a-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8a60a-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a60a-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8a60a-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a60a-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8a60a-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a60a-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8a60a-139">Schema name</span></span>  <br/> |<span data-ttu-id="8a60a-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8a60a-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="8a60a-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8a60a-141">Validation file</span></span>  <br/> |<span data-ttu-id="8a60a-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8a60a-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a60a-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8a60a-143">Can be empty</span></span>  <br/> |<span data-ttu-id="8a60a-144">False</span><span class="sxs-lookup"><span data-stu-id="8a60a-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a60a-145">См. также</span><span class="sxs-lookup"><span data-stu-id="8a60a-145">See also</span></span>

- [<span data-ttu-id="8a60a-146">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="8a60a-146">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="8a60a-147">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="8a60a-147">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="8a60a-148">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="8a60a-148">Unsubscribe operation</span></span>](unsubscribe-operation.md)

