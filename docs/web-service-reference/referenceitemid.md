---
title: референцеитемид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReferenceItemId
api_type:
- schema
ms.assetid: 8fd4bb12-a94b-43f5-be3b-f435684e311d
description: Элемент Референцеитемид определяет элемент, на который ссылается объект Response.
ms.openlocfilehash: 3b77d75de91af8ec8fb7ae2d507377d1d976febf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457230"
---
# <a name="referenceitemid"></a><span data-ttu-id="ab3fd-103">референцеитемид</span><span class="sxs-lookup"><span data-stu-id="ab3fd-103">ReferenceItemId</span></span>

<span data-ttu-id="ab3fd-104">Элемент **референцеитемид** определяет элемент, на который ссылается объект Response.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-104">The **ReferenceItemId** element identifies the item to which the response object refers.</span></span> 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="ab3fd-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="ab3fd-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab3fd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ab3fd-106">Attributes and elements</span></span>

<span data-ttu-id="ab3fd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab3fd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ab3fd-108">Attributes</span></span>

|<span data-ttu-id="ab3fd-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ab3fd-109">**Attribute**</span></span>|<span data-ttu-id="ab3fd-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ab3fd-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ab3fd-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="ab3fd-111">**Id**</span></span> <br/> |<span data-ttu-id="ab3fd-112">Определяет определенный элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="ab3fd-113">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="ab3fd-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="ab3fd-114">Определяет определенную версию элемента.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-114">Identifies a specific version of an item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ab3fd-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ab3fd-115">Child elements</span></span>

<span data-ttu-id="ab3fd-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ab3fd-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ab3fd-117">Parent elements</span></span>

|<span data-ttu-id="ab3fd-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ab3fd-118">**Element**</span></span>|<span data-ttu-id="ab3fd-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ab3fd-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ab3fd-120">акцептитем</span><span class="sxs-lookup"><span data-stu-id="ab3fd-120">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="ab3fd-121">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-121">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ab3fd-122">акцептшарингинвитатион</span><span class="sxs-lookup"><span data-stu-id="ab3fd-122">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="ab3fd-123">Представляет ответ на приглашение для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-123">Represents an Accept reply to a sharing invitation.</span></span>  <br/> |
|[<span data-ttu-id="ab3fd-124">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="ab3fd-124">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="ab3fd-125">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-125">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="ab3fd-126">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="ab3fd-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="ab3fd-127">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ab3fd-128">форвардитем</span><span class="sxs-lookup"><span data-stu-id="ab3fd-128">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="ab3fd-129">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-129">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="ab3fd-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="ab3fd-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="ab3fd-131">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ab3fd-132">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="ab3fd-132">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="ab3fd-133">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-133">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ab3fd-134">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="ab3fd-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="ab3fd-135">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ab3fd-136">суппрессреадрецеипт</span><span class="sxs-lookup"><span data-stu-id="ab3fd-136">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="ab3fd-137">Используется для ответа на запросы уведомления о прочтении.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-137">Used to respond to read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="ab3fd-138">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="ab3fd-138">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="ab3fd-139">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-139">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ab3fd-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="ab3fd-140">Remarks</span></span>

<span data-ttu-id="ab3fd-141">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ab3fd-141">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab3fd-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ab3fd-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab3fd-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ab3fd-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ab3fd-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ab3fd-144">Schema Name</span></span>  <br/> |<span data-ttu-id="ab3fd-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ab3fd-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="ab3fd-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ab3fd-146">Validation File</span></span>  <br/> |<span data-ttu-id="ab3fd-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ab3fd-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ab3fd-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ab3fd-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="ab3fd-149">False</span><span class="sxs-lookup"><span data-stu-id="ab3fd-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ab3fd-150">См. также</span><span class="sxs-lookup"><span data-stu-id="ab3fd-150">See also</span></span>



- [<span data-ttu-id="ab3fd-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ab3fd-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

