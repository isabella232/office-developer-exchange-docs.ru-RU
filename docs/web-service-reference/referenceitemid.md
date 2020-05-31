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
ms.openlocfilehash: d29f2dfec8f2c23fe0ac8c84d2bb9029fce613d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835032"
---
# <a name="referenceitemid"></a><span data-ttu-id="60ca7-103">референцеитемид</span><span class="sxs-lookup"><span data-stu-id="60ca7-103">ReferenceItemId</span></span>

<span data-ttu-id="60ca7-104">Элемент **референцеитемид** определяет элемент, на который ссылается объект Response.</span><span class="sxs-lookup"><span data-stu-id="60ca7-104">The **ReferenceItemId** element identifies the item to which the response object refers.</span></span> 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="60ca7-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="60ca7-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60ca7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="60ca7-106">Attributes and elements</span></span>

<span data-ttu-id="60ca7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="60ca7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60ca7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="60ca7-108">Attributes</span></span>

|<span data-ttu-id="60ca7-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="60ca7-109">**Attribute**</span></span>|<span data-ttu-id="60ca7-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="60ca7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="60ca7-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="60ca7-111">**Id**</span></span> <br/> |<span data-ttu-id="60ca7-112">Определяет определенный элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="60ca7-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="60ca7-113">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="60ca7-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="60ca7-114">Определяет определенную версию элемента.</span><span class="sxs-lookup"><span data-stu-id="60ca7-114">Identifies a specific version of an item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="60ca7-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="60ca7-115">Child elements</span></span>

<span data-ttu-id="60ca7-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="60ca7-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="60ca7-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="60ca7-117">Parent elements</span></span>

|<span data-ttu-id="60ca7-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="60ca7-118">**Element**</span></span>|<span data-ttu-id="60ca7-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="60ca7-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60ca7-120">акцептитем</span><span class="sxs-lookup"><span data-stu-id="60ca7-120">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="60ca7-121">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="60ca7-121">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="60ca7-122">акцептшарингинвитатион</span><span class="sxs-lookup"><span data-stu-id="60ca7-122">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="60ca7-123">Представляет ответ на приглашение для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="60ca7-123">Represents an Accept reply to a sharing invitation.</span></span>  <br/> |
|[<span data-ttu-id="60ca7-124">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="60ca7-124">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="60ca7-125">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="60ca7-125">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="60ca7-126">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="60ca7-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="60ca7-127">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="60ca7-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="60ca7-128">форвардитем</span><span class="sxs-lookup"><span data-stu-id="60ca7-128">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="60ca7-129">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="60ca7-129">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="60ca7-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="60ca7-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="60ca7-131">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="60ca7-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="60ca7-132">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="60ca7-132">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="60ca7-133">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="60ca7-133">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="60ca7-134">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="60ca7-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="60ca7-135">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="60ca7-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="60ca7-136">суппрессреадрецеипт</span><span class="sxs-lookup"><span data-stu-id="60ca7-136">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="60ca7-137">Используется для ответа на запросы уведомления о прочтении.</span><span class="sxs-lookup"><span data-stu-id="60ca7-137">Used to respond to read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="60ca7-138">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="60ca7-138">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="60ca7-139">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="60ca7-139">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="60ca7-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="60ca7-140">Remarks</span></span>

<span data-ttu-id="60ca7-141">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="60ca7-141">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60ca7-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="60ca7-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60ca7-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="60ca7-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="60ca7-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="60ca7-144">Schema Name</span></span>  <br/> |<span data-ttu-id="60ca7-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="60ca7-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="60ca7-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="60ca7-146">Validation File</span></span>  <br/> |<span data-ttu-id="60ca7-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="60ca7-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="60ca7-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="60ca7-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="60ca7-149">False</span><span class="sxs-lookup"><span data-stu-id="60ca7-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60ca7-150">См. также</span><span class="sxs-lookup"><span data-stu-id="60ca7-150">See also</span></span>



- [<span data-ttu-id="60ca7-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="60ca7-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

