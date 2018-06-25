---
title: ReferenceItemId
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
description: Элемент ReferenceItemId определяет элемент, к которому относится объект ответа.
ms.openlocfilehash: d29f2dfec8f2c23fe0ac8c84d2bb9029fce613d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835032"
---
# <a name="referenceitemid"></a><span data-ttu-id="f7af8-103">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="f7af8-103">ReferenceItemId</span></span>

<span data-ttu-id="f7af8-104">Элемент **ReferenceItemId** определяет элемент, к которому относится объект ответа.</span><span class="sxs-lookup"><span data-stu-id="f7af8-104">The **ReferenceItemId** element identifies the item to which the response object refers.</span></span> 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="f7af8-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="f7af8-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7af8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f7af8-106">Attributes and elements</span></span>

<span data-ttu-id="f7af8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f7af8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7af8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f7af8-108">Attributes</span></span>

|<span data-ttu-id="f7af8-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f7af8-109">**Attribute**</span></span>|<span data-ttu-id="f7af8-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f7af8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f7af8-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="f7af8-111">**Id**</span></span> <br/> |<span data-ttu-id="f7af8-112">Идентифицирует определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7af8-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="f7af8-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="f7af8-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="f7af8-114">Идентифицирует определенной версии элемента.</span><span class="sxs-lookup"><span data-stu-id="f7af8-114">Identifies a specific version of an item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f7af8-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f7af8-115">Child elements</span></span>

<span data-ttu-id="f7af8-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="f7af8-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f7af8-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f7af8-117">Parent elements</span></span>

|<span data-ttu-id="f7af8-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f7af8-118">**Element**</span></span>|<span data-ttu-id="f7af8-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f7af8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7af8-120">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="f7af8-120">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="f7af8-121">Представляет ответ на принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="f7af8-121">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f7af8-122">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="f7af8-122">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="f7af8-123">Представляет ответ на Accept для приглашения на общий доступ.</span><span class="sxs-lookup"><span data-stu-id="f7af8-123">Represents an Accept reply to a sharing invitation.</span></span>  <br/> |
|[<span data-ttu-id="f7af8-124">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="f7af8-124">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="f7af8-125">Представляет объект ответа, которая используется для отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="f7af8-125">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="f7af8-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="f7af8-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="f7af8-127">Представляет отклонить ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="f7af8-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f7af8-128">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="f7af8-128">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="f7af8-129">Содержит элемент хранилища Exchange переадресация получателям.</span><span class="sxs-lookup"><span data-stu-id="f7af8-129">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="f7af8-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="f7af8-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="f7af8-131">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7af8-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7af8-132">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="f7af8-132">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="f7af8-133">Содержит ответить всем получателям определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7af8-133">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7af8-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="f7af8-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="f7af8-135">Содержит ответ создателем элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7af8-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7af8-136">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="f7af8-136">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="f7af8-137">Используется для ответа на чтение запросов уведомлений.</span><span class="sxs-lookup"><span data-stu-id="f7af8-137">Used to respond to read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="f7af8-138">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="f7af8-138">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="f7af8-139">Представляет под вопросом ответ на приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="f7af8-139">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f7af8-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="f7af8-140">Remarks</span></span>

<span data-ttu-id="f7af8-141">Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f7af8-141">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7af8-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f7af8-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7af8-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f7af8-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7af8-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f7af8-144">Schema Name</span></span>  <br/> |<span data-ttu-id="f7af8-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f7af8-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7af8-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f7af8-146">Validation File</span></span>  <br/> |<span data-ttu-id="f7af8-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f7af8-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7af8-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f7af8-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7af8-149">False</span><span class="sxs-lookup"><span data-stu-id="f7af8-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7af8-150">См. также</span><span class="sxs-lookup"><span data-stu-id="f7af8-150">See also</span></span>



- [<span data-ttu-id="f7af8-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f7af8-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

