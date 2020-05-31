---
title: SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fd5b9f0e-23e8-428c-8168-2d6b4ecd6beb
description: Элемент SetHoldOnMailboxes содержит запрос SetHoldOnMailboxes.
ms.openlocfilehash: 7d226de908c4d5a474129e3e1f2344ec1318f538
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835413"
---
# <a name="setholdonmailboxes"></a><span data-ttu-id="07e6d-103">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="07e6d-103">SetHoldOnMailboxes</span></span>

<span data-ttu-id="07e6d-104">Элемент **SetHoldOnMailboxes** содержит запрос **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="07e6d-104">The **SetHoldOnMailboxes** element contains a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxes>
   <ActionType/>
   <HoldId/>
   <Query/>
   <Mailboxes/>
   <Language/>
   <IncludeNonIndexableItems/>
   <Deduplication/>
   <InPlaceHoldIdentity/>
</SetHoldOnMailboxes>
```

 <span data-ttu-id="07e6d-105">**сесолдонмаилбоксестипе**</span><span class="sxs-lookup"><span data-stu-id="07e6d-105">**SetHoldOnMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07e6d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="07e6d-106">Attributes and elements</span></span>

<span data-ttu-id="07e6d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="07e6d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07e6d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="07e6d-108">Attributes</span></span>

<span data-ttu-id="07e6d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="07e6d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07e6d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="07e6d-110">Child elements</span></span>

<span data-ttu-id="07e6d-111">[Холдактионтипе (](actiontype-holdactiontype.md) | [холдид](holdid.md) | ) | [почтовые ящики запросов (аррайофстрингстипе)](mailboxes-arrayofstringstype.md) | [Language](language.md) | [инклуденониндексаблеитемс](includenonindexableitems.md) | [дедупликации](deduplication.md) | [InPlaceHoldIdentity](inplaceholdidentity.md) [Query](query.md)</span><span class="sxs-lookup"><span data-stu-id="07e6d-111">[ActionType (HoldActionType)](actiontype-holdactiontype.md) | [HoldId](holdid.md) | [Query](query.md) | [Mailboxes (ArrayOfStringsType)](mailboxes-arrayofstringstype.md) | [Language](language.md) | [IncludeNonIndexableItems](includenonindexableitems.md) | [Deduplication](deduplication.md) | [InPlaceHoldIdentity](inplaceholdidentity.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="07e6d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="07e6d-112">Parent elements</span></span>

<span data-ttu-id="07e6d-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="07e6d-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="07e6d-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="07e6d-114">Remarks</span></span>

<span data-ttu-id="07e6d-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="07e6d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="07e6d-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="07e6d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07e6d-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="07e6d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07e6d-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="07e6d-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="07e6d-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="07e6d-119">Schema name</span></span>  <br/> |<span data-ttu-id="07e6d-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="07e6d-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="07e6d-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="07e6d-121">Validation file</span></span>  <br/> |<span data-ttu-id="07e6d-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="07e6d-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="07e6d-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="07e6d-123">Can be empty</span></span>  <br/> ||
   

