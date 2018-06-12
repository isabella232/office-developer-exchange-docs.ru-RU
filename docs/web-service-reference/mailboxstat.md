---
title: MailboxStat
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: Элемент MailboxStat указывает статистика почтового ящика, просматриваемой поиск обнаружения.
ms.openlocfilehash: 692f15904467ce192074b14f7c2a742b3e76de8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834296"
---
# <a name="mailboxstat"></a><span data-ttu-id="f41a6-103">MailboxStat</span><span class="sxs-lookup"><span data-stu-id="f41a6-103">MailboxStat</span></span>

<span data-ttu-id="f41a6-104">Элемент **MailboxStat** указывает статистика почтового ящика, просматриваемой поиск обнаружения.</span><span class="sxs-lookup"><span data-stu-id="f41a6-104">The **MailboxStat** element specifies statistics for a mailbox searched by discovery search.</span></span> 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

<span data-ttu-id="f41a6-105">**MailboxStatisticsItemType**</span><span class="sxs-lookup"><span data-stu-id="f41a6-105">**MailboxStatisticsItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f41a6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f41a6-106">Attributes and elements</span></span>

<span data-ttu-id="f41a6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f41a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f41a6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f41a6-108">Attributes</span></span>

<span data-ttu-id="f41a6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f41a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f41a6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f41a6-110">Child elements</span></span>

<span data-ttu-id="f41a6-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [размер (long)](size-long.md)</span><span class="sxs-lookup"><span data-stu-id="f41a6-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f41a6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f41a6-112">Parent elements</span></span>

[<span data-ttu-id="f41a6-113">MailboxStats</span><span class="sxs-lookup"><span data-stu-id="f41a6-113">MailboxStats</span></span>](mailboxstats.md)
  
## <a name="remarks"></a><span data-ttu-id="f41a6-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="f41a6-114">Remarks</span></span>

<span data-ttu-id="f41a6-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f41a6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f41a6-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f41a6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f41a6-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f41a6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f41a6-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f41a6-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f41a6-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f41a6-119">Schema name</span></span>  <br/> |<span data-ttu-id="f41a6-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f41a6-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="f41a6-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f41a6-121">Validation file</span></span>  <br/> |<span data-ttu-id="f41a6-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f41a6-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f41a6-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f41a6-123">Can be empty</span></span>  <br/> |<span data-ttu-id="f41a6-124">Нет</span><span class="sxs-lookup"><span data-stu-id="f41a6-124">false</span></span>  <br/> |
   

