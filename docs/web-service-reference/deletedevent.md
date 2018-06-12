---
title: DeletedEvent
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
description: DeletedEvent элемент представляет событие, в котором удаляется элемент или папку.
ms.openlocfilehash: f06ca0727916f415c648e876f88bf7eacef5a5ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762027"
---
# <a name="deletedevent"></a><span data-ttu-id="a3f46-103">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="a3f46-103">DeletedEvent</span></span>

<span data-ttu-id="a3f46-104">**DeletedEvent** элемент представляет событие, в котором удаляется элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="a3f46-104">The **DeletedEvent** element represents an event in which an item or folder is deleted.</span></span> 
  
```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</DeletedEvent>
```

<span data-ttu-id="a3f46-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="a3f46-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a3f46-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a3f46-106">Attributes and elements</span></span>

<span data-ttu-id="a3f46-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a3f46-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3f46-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a3f46-108">Attributes</span></span>

<span data-ttu-id="a3f46-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a3f46-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3f46-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a3f46-110">Child elements</span></span>

|<span data-ttu-id="a3f46-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a3f46-111">**Element**</span></span>|<span data-ttu-id="a3f46-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a3f46-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3f46-113">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="a3f46-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="a3f46-114">Представляет закладку события в таблице событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a3f46-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="a3f46-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="a3f46-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="a3f46-116">Представляет отметки времени удаленного почтового ящика события элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="a3f46-116">Represents the timestamp of a deleted item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="a3f46-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="a3f46-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="a3f46-118">Представляет идентификатор папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="a3f46-118">Represents the identifier of the deleted folder.</span></span>  <br/> |
|[<span data-ttu-id="a3f46-119">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="a3f46-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="a3f46-120">Представляет идентификатор удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="a3f46-120">Represents the identifier of the deleted item.</span></span>  <br/> |
|[<span data-ttu-id="a3f46-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="a3f46-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="a3f46-122">Представляет идентификатор родительской папки удаленного элемента или папки до удаления.</span><span class="sxs-lookup"><span data-stu-id="a3f46-122">Represents the identifier of the parent folder of the deleted item or folder before deletion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3f46-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a3f46-123">Parent elements</span></span>

|<span data-ttu-id="a3f46-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a3f46-124">**Element**</span></span>|<span data-ttu-id="a3f46-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a3f46-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3f46-126">Уведомление</span><span class="sxs-lookup"><span data-stu-id="a3f46-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a3f46-127">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="a3f46-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a3f46-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="a3f46-128">Remarks</span></span>

<span data-ttu-id="a3f46-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a3f46-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3f46-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a3f46-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3f46-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a3f46-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a3f46-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a3f46-132">Schema name</span></span>  <br/> |<span data-ttu-id="a3f46-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a3f46-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="a3f46-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a3f46-134">Validation file</span></span>  <br/> |<span data-ttu-id="a3f46-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a3f46-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a3f46-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a3f46-136">Can be empty</span></span>  <br/> |<span data-ttu-id="a3f46-137">False</span><span class="sxs-lookup"><span data-stu-id="a3f46-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3f46-138">См. также</span><span class="sxs-lookup"><span data-stu-id="a3f46-138">See also</span></span>

- [<span data-ttu-id="a3f46-139">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="a3f46-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="a3f46-140">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="a3f46-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="a3f46-141">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="a3f46-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)

