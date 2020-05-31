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
ms.openlocfilehash: 7ebfbb744a80e3a2d14ee9e0e1b952d2269dbf94
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353170"
---
# <a name="copiedevent"></a><span data-ttu-id="db381-103">копиедевент</span><span class="sxs-lookup"><span data-stu-id="db381-103">CopiedEvent</span></span>

<span data-ttu-id="db381-104">Элемент **копиедевент** представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="db381-104">The **CopiedEvent** element represents an event in which an item or folder is copied.</span></span> 
  
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

<span data-ttu-id="db381-105">**моведкопиедевенттипе**</span><span class="sxs-lookup"><span data-stu-id="db381-105">**MovedCopiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="db381-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="db381-106">Attributes and elements</span></span>

<span data-ttu-id="db381-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="db381-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db381-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="db381-108">Attributes</span></span>

<span data-ttu-id="db381-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="db381-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db381-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="db381-110">Child elements</span></span>

|<span data-ttu-id="db381-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db381-111">**Element**</span></span>|<span data-ttu-id="db381-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db381-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db381-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="db381-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="db381-114">Представляет закладку Events в таблице событий почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="db381-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="db381-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="db381-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="db381-116">Представляет метку времени события копирования элемента или папки почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="db381-116">Represents the timestamp of a copy item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="db381-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="db381-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="db381-118">Представляет идентификатор папки.</span><span class="sxs-lookup"><span data-stu-id="db381-118">Represents the identifier of the folder.</span></span>  <br/> |
|[<span data-ttu-id="db381-119">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="db381-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="db381-120">Представляет идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="db381-120">Represents the identifier of the item.</span></span>  <br/> |
|[<span data-ttu-id="db381-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="db381-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="db381-122">Представляет идентификатор папки, содержащей копию.</span><span class="sxs-lookup"><span data-stu-id="db381-122">Represents the identifier of the folder that contains the copy.</span></span>  <br/> |
|[<span data-ttu-id="db381-123">олдфолдерид</span><span class="sxs-lookup"><span data-stu-id="db381-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="db381-124">Представляет идентификатор исходной папки перед ее копированием.</span><span class="sxs-lookup"><span data-stu-id="db381-124">Represents the folder identifier of the original folder before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="db381-125">олдитемид</span><span class="sxs-lookup"><span data-stu-id="db381-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="db381-126">Содержит уникальный идентификатор исходного элемента перед его копированием.</span><span class="sxs-lookup"><span data-stu-id="db381-126">Contains the unique identifier of the original item before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="db381-127">олдпарентфолдерид</span><span class="sxs-lookup"><span data-stu-id="db381-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="db381-128">Содержит идентификатор исходной родительской папки для скопированного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="db381-128">Contains the identifier of the original parent folder of an item or folder that was copied.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db381-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="db381-129">Parent elements</span></span>

|<span data-ttu-id="db381-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db381-130">**Element**</span></span>|<span data-ttu-id="db381-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db381-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db381-132">Уведомление</span><span class="sxs-lookup"><span data-stu-id="db381-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="db381-133">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="db381-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="db381-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="db381-134">Remarks</span></span>

<span data-ttu-id="db381-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="db381-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db381-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="db381-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db381-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="db381-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="db381-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="db381-138">Schema name</span></span>  <br/> |<span data-ttu-id="db381-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="db381-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="db381-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="db381-140">Validation file</span></span>  <br/> |<span data-ttu-id="db381-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="db381-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="db381-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="db381-142">Can be empty</span></span>  <br/> |<span data-ttu-id="db381-143">False</span><span class="sxs-lookup"><span data-stu-id="db381-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db381-144">См. также</span><span class="sxs-lookup"><span data-stu-id="db381-144">See also</span></span>

- [<span data-ttu-id="db381-145">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="db381-145">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="db381-146">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="db381-146">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="db381-147">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="db381-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="db381-148">Использование подписок по запросу</span><span class="sxs-lookup"><span data-stu-id="db381-148">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [<span data-ttu-id="db381-149">Пример приложения для push-уведомлений</span><span class="sxs-lookup"><span data-stu-id="db381-149">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

