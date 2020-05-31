---
title: Метка времени
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeStamp
api_type:
- schema
ms.assetid: 5eae859a-5a74-4bf6-b196-d1b2fd38501a
description: Элемент timestamp представляет метку времени события почтового ящика.
ms.openlocfilehash: d020d9a4cf3a128d26e0ff2b83be9f3deb024339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840231"
---
# <a name="timestamp"></a><span data-ttu-id="93984-103">Метка времени</span><span class="sxs-lookup"><span data-stu-id="93984-103">TimeStamp</span></span>

<span data-ttu-id="93984-104">Элемент **timestamp** представляет метку времени события почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="93984-104">The **Timestamp** element represents the timestamp of a mailbox event.</span></span> 
  
```xml
<TimeStamp/>
```

 <span data-ttu-id="93984-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="93984-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93984-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93984-106">Attributes and elements</span></span>

<span data-ttu-id="93984-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="93984-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93984-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93984-108">Attributes</span></span>

<span data-ttu-id="93984-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="93984-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93984-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93984-110">Child elements</span></span>

<span data-ttu-id="93984-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="93984-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93984-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93984-112">Parent elements</span></span>

|<span data-ttu-id="93984-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93984-113">**Element**</span></span>|<span data-ttu-id="93984-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93984-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93984-115">копиедевент</span><span class="sxs-lookup"><span data-stu-id="93984-115">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="93984-116">Представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="93984-116">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="93984-117">креатедевент</span><span class="sxs-lookup"><span data-stu-id="93984-117">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="93984-118">Представляет событие, в котором создается элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="93984-118">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="93984-119">делетедевент</span><span class="sxs-lookup"><span data-stu-id="93984-119">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="93984-120">Представляет событие, в котором удаляется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="93984-120">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="93984-121">модифиедевент</span><span class="sxs-lookup"><span data-stu-id="93984-121">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="93984-122">Представляет событие, в котором изменяется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="93984-122">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="93984-123">моведевент</span><span class="sxs-lookup"><span data-stu-id="93984-123">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="93984-124">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="93984-124">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="93984-125">невмаилевент</span><span class="sxs-lookup"><span data-stu-id="93984-125">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="93984-126">Представляет событие, инициированное новым почтовым элементом в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="93984-126">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93984-127">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="93984-127">Text value</span></span>

<span data-ttu-id="93984-128">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="93984-128">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93984-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="93984-129">Remarks</span></span>

<span data-ttu-id="93984-130">Этот элемент в основном доступен для использования в определении клиента частоты событий.</span><span class="sxs-lookup"><span data-stu-id="93984-130">This element is primarily available for use in client determination of event frequency.</span></span> <span data-ttu-id="93984-131">Отсутствует в [статусевент](statusevent.md).</span><span class="sxs-lookup"><span data-stu-id="93984-131">This is not present in [StatusEvent](statusevent.md).</span></span>
  
<span data-ttu-id="93984-132">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="93984-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93984-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93984-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93984-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93984-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93984-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93984-135">Schema name</span></span>  <br/> |<span data-ttu-id="93984-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="93984-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="93984-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93984-137">Validation file</span></span>  <br/> |<span data-ttu-id="93984-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="93984-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93984-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93984-139">Can be empty</span></span>  <br/> |<span data-ttu-id="93984-140">False</span><span class="sxs-lookup"><span data-stu-id="93984-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93984-141">См. также</span><span class="sxs-lookup"><span data-stu-id="93984-141">See also</span></span>



[<span data-ttu-id="93984-142">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="93984-142">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="93984-143">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="93984-143">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="93984-144">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="93984-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)

