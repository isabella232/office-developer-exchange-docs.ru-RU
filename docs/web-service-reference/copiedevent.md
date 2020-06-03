---
title: копиедевент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: Элемент Копиедевент представляет событие, в котором копируется элемент или папка.
ms.openlocfilehash: 928910ddbe0bf1e48549d1665ab373f7382366d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529247"
---
# <a name="copiedevent"></a><span data-ttu-id="60052-103">копиедевент</span><span class="sxs-lookup"><span data-stu-id="60052-103">CopiedEvent</span></span>

<span data-ttu-id="60052-104">Элемент **копиедевент** представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="60052-104">The **CopiedEvent** element represents an event in which an item or folder is copied.</span></span> 
  
```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

<span data-ttu-id="60052-105">**моведкопиедевенттипе**</span><span class="sxs-lookup"><span data-stu-id="60052-105">**MovedCopiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="60052-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="60052-106">Attributes and elements</span></span>

<span data-ttu-id="60052-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="60052-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60052-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="60052-108">Attributes</span></span>

<span data-ttu-id="60052-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="60052-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60052-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="60052-110">Child elements</span></span>

|<span data-ttu-id="60052-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="60052-111">**Element**</span></span>|<span data-ttu-id="60052-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="60052-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60052-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="60052-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="60052-114">Представляет закладку Events в таблице событий почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="60052-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="60052-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="60052-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="60052-116">Представляет метку времени события копирования элемента или папки почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="60052-116">Represents the timestamp of a copy item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="60052-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="60052-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="60052-118">Представляет идентификатор папки.</span><span class="sxs-lookup"><span data-stu-id="60052-118">Represents the identifier of the folder.</span></span>  <br/> |
|[<span data-ttu-id="60052-119">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="60052-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="60052-120">Представляет идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="60052-120">Represents the identifier of the item.</span></span>  <br/> |
|[<span data-ttu-id="60052-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="60052-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="60052-122">Представляет идентификатор папки, содержащей копию.</span><span class="sxs-lookup"><span data-stu-id="60052-122">Represents the identifier of the folder that contains the copy.</span></span>  <br/> |
|[<span data-ttu-id="60052-123">олдфолдерид</span><span class="sxs-lookup"><span data-stu-id="60052-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="60052-124">Представляет идентификатор исходной папки перед ее копированием.</span><span class="sxs-lookup"><span data-stu-id="60052-124">Represents the folder identifier of the original folder before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="60052-125">олдитемид</span><span class="sxs-lookup"><span data-stu-id="60052-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="60052-126">Содержит уникальный идентификатор исходного элемента перед его копированием.</span><span class="sxs-lookup"><span data-stu-id="60052-126">Contains the unique identifier of the original item before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="60052-127">олдпарентфолдерид</span><span class="sxs-lookup"><span data-stu-id="60052-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="60052-128">Содержит идентификатор исходной родительской папки для скопированного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="60052-128">Contains the identifier of the original parent folder of an item or folder that was copied.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60052-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="60052-129">Parent elements</span></span>

|<span data-ttu-id="60052-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="60052-130">**Element**</span></span>|<span data-ttu-id="60052-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="60052-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60052-132">Уведомление</span><span class="sxs-lookup"><span data-stu-id="60052-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="60052-133">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="60052-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="60052-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="60052-134">Remarks</span></span>

<span data-ttu-id="60052-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="60052-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60052-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="60052-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60052-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="60052-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="60052-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="60052-138">Schema name</span></span>  <br/> |<span data-ttu-id="60052-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="60052-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="60052-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="60052-140">Validation file</span></span>  <br/> |<span data-ttu-id="60052-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="60052-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="60052-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="60052-142">Can be empty</span></span>  <br/> |<span data-ttu-id="60052-143">False</span><span class="sxs-lookup"><span data-stu-id="60052-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60052-144">См. также</span><span class="sxs-lookup"><span data-stu-id="60052-144">See also</span></span>

- [<span data-ttu-id="60052-145">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="60052-145">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="60052-146">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="60052-146">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="60052-147">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="60052-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="60052-148">Использование подписок по запросу</span><span class="sxs-lookup"><span data-stu-id="60052-148">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [<span data-ttu-id="60052-149">Пример приложения для push-уведомлений</span><span class="sxs-lookup"><span data-stu-id="60052-149">Push Notification Sample Application</span></span>](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

