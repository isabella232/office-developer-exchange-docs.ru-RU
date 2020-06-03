---
title: делетедевент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedEvent
api_type:
- schema
ms.assetid: c4565eb4-b537-466c-b1ff-11602533812b
description: Элемент Делетедевент представляет событие, в котором удаляется элемент или папка.
ms.openlocfilehash: 5eb0c947aacc592f81c595da2cc00bf4874f300b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526944"
---
# <a name="deletedevent"></a><span data-ttu-id="7c0f5-103">делетедевент</span><span class="sxs-lookup"><span data-stu-id="7c0f5-103">DeletedEvent</span></span>

<span data-ttu-id="7c0f5-104">Элемент **делетедевент** представляет событие, в котором удаляется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="7c0f5-104">The **DeletedEvent** element represents an event in which an item or folder is deleted.</span></span> 
  
```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</DeletedEvent>
```

```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
</DeletedEvent>
```

<span data-ttu-id="7c0f5-105">**басеобжектчанжедевенттипе**</span><span class="sxs-lookup"><span data-stu-id="7c0f5-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7c0f5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7c0f5-106">Attributes and elements</span></span>

<span data-ttu-id="7c0f5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7c0f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c0f5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7c0f5-108">Attributes</span></span>

<span data-ttu-id="7c0f5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7c0f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c0f5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7c0f5-110">Child elements</span></span>

|<span data-ttu-id="7c0f5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c0f5-111">**Element**</span></span>|<span data-ttu-id="7c0f5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c0f5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c0f5-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="7c0f5-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="7c0f5-114">Представляет закладку события в таблице событий почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="7c0f5-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="7c0f5-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="7c0f5-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="7c0f5-116">Представляет метку времени для удаленного события элемента или папки почтового ящика папки.</span><span class="sxs-lookup"><span data-stu-id="7c0f5-116">Represents the timestamp of a deleted item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="7c0f5-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="7c0f5-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="7c0f5-118">Представляет идентификатор удаленной папки.</span><span class="sxs-lookup"><span data-stu-id="7c0f5-118">Represents the identifier of the deleted folder.</span></span>  <br/> |
|[<span data-ttu-id="7c0f5-119">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="7c0f5-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7c0f5-120">Представляет идентификатор удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="7c0f5-120">Represents the identifier of the deleted item.</span></span>  <br/> |
|[<span data-ttu-id="7c0f5-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="7c0f5-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="7c0f5-122">Представляет идентификатор родительской папки удаленного элемента или папки перед удалением.</span><span class="sxs-lookup"><span data-stu-id="7c0f5-122">Represents the identifier of the parent folder of the deleted item or folder before deletion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c0f5-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7c0f5-123">Parent elements</span></span>

|<span data-ttu-id="7c0f5-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c0f5-124">**Element**</span></span>|<span data-ttu-id="7c0f5-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c0f5-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c0f5-126">Уведомление</span><span class="sxs-lookup"><span data-stu-id="7c0f5-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7c0f5-127">Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="7c0f5-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c0f5-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="7c0f5-128">Remarks</span></span>

<span data-ttu-id="7c0f5-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7c0f5-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c0f5-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7c0f5-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c0f5-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7c0f5-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c0f5-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7c0f5-132">Schema name</span></span>  <br/> |<span data-ttu-id="7c0f5-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7c0f5-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c0f5-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7c0f5-134">Validation file</span></span>  <br/> |<span data-ttu-id="7c0f5-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7c0f5-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c0f5-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7c0f5-136">Can be empty</span></span>  <br/> |<span data-ttu-id="7c0f5-137">False</span><span class="sxs-lookup"><span data-stu-id="7c0f5-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c0f5-138">См. также</span><span class="sxs-lookup"><span data-stu-id="7c0f5-138">See also</span></span>

- [<span data-ttu-id="7c0f5-139">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="7c0f5-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="7c0f5-140">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="7c0f5-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="7c0f5-141">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="7c0f5-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)

