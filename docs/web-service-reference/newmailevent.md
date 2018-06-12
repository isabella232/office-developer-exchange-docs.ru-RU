---
title: NewMailEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewMailEvent
api_type:
- schema
ms.assetid: 45057945-a3ec-4dac-92db-f0dc5fcfc34d
description: NewMailEvent элемент представляет событие, которое инициируется нового элемента почты в почтовом ящике.
ms.openlocfilehash: 8df3e4a218a8eaa9d129854e4816a3a43beddafa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834527"
---
# <a name="newmailevent"></a><span data-ttu-id="7760c-103">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="7760c-103">NewMailEvent</span></span>

<span data-ttu-id="7760c-104">**NewMailEvent** элемент представляет событие, которое инициируется нового элемента почты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="7760c-104">The **NewMailEvent** element represents an event that is triggered by a new mail item in a mailbox.</span></span> 
  
```xml
<NewMailEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</NewMailEvent>
```

 <span data-ttu-id="7760c-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="7760c-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7760c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7760c-106">Attributes and elements</span></span>

<span data-ttu-id="7760c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7760c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7760c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7760c-108">Attributes</span></span>

<span data-ttu-id="7760c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7760c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7760c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7760c-110">Child elements</span></span>

|<span data-ttu-id="7760c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7760c-111">**Element**</span></span>|<span data-ttu-id="7760c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7760c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7760c-113">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="7760c-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="7760c-114">Представляет закладку события в таблице событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7760c-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="7760c-115">Метка времени</span><span class="sxs-lookup"><span data-stu-id="7760c-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="7760c-116">Представляет отметки времени поступления нового элемента почты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="7760c-116">Represents the timestamp of the arrival of a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7760c-117">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="7760c-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7760c-118">Представляет идентификатор нового почтового элемента.</span><span class="sxs-lookup"><span data-stu-id="7760c-118">Represents the identifier of a new mail item.</span></span>  <br/> |
|[<span data-ttu-id="7760c-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="7760c-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="7760c-120">Представляет идентификатор родительской папки нового почтового элемента.</span><span class="sxs-lookup"><span data-stu-id="7760c-120">Represents the identifier of the parent folder of the new mail item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7760c-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7760c-121">Parent elements</span></span>

|<span data-ttu-id="7760c-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7760c-122">**Element**</span></span>|<span data-ttu-id="7760c-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7760c-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7760c-124">Уведомление</span><span class="sxs-lookup"><span data-stu-id="7760c-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7760c-125">Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="7760c-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7760c-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="7760c-126">Remarks</span></span>

<span data-ttu-id="7760c-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7760c-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7760c-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7760c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7760c-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7760c-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7760c-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7760c-130">Schema name</span></span>  <br/> |<span data-ttu-id="7760c-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7760c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="7760c-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7760c-132">Validation file</span></span>  <br/> |<span data-ttu-id="7760c-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7760c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7760c-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7760c-134">Can be empty</span></span>  <br/> |<span data-ttu-id="7760c-135">False</span><span class="sxs-lookup"><span data-stu-id="7760c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7760c-136">См. также</span><span class="sxs-lookup"><span data-stu-id="7760c-136">See also</span></span>



[<span data-ttu-id="7760c-137">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="7760c-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="7760c-138">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="7760c-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="7760c-139">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="7760c-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

