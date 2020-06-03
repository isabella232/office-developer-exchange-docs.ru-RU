---
title: маилбоксстат
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: Элемент Маилбоксстат указывает статистику для почтового ящика, в котором выполняется поиск обнаружения.
ms.openlocfilehash: 417f63f5e1aa34c2157b1d5ad868461113afec7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44451434"
---
# <a name="mailboxstat"></a><span data-ttu-id="23652-103">маилбоксстат</span><span class="sxs-lookup"><span data-stu-id="23652-103">MailboxStat</span></span>

<span data-ttu-id="23652-104">Элемент **маилбоксстат** указывает статистику для почтового ящика, в котором выполняется поиск обнаружения.</span><span class="sxs-lookup"><span data-stu-id="23652-104">The **MailboxStat** element specifies statistics for a mailbox searched by discovery search.</span></span> 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

<span data-ttu-id="23652-105">**маилбоксстатистикситемтипе**</span><span class="sxs-lookup"><span data-stu-id="23652-105">**MailboxStatisticsItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="23652-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="23652-106">Attributes and elements</span></span>

<span data-ttu-id="23652-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="23652-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23652-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="23652-108">Attributes</span></span>

<span data-ttu-id="23652-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23652-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23652-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="23652-110">Child elements</span></span>

<span data-ttu-id="23652-111">[MailboxId](mailboxid.md)  |  [DisplayName (строка)](displayname-string.md)  |  [ItemCount](itemcount.md)  |  [Размер (длинный)](size-long.md)</span><span class="sxs-lookup"><span data-stu-id="23652-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23652-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="23652-112">Parent elements</span></span>

[<span data-ttu-id="23652-113">маилбоксстатс</span><span class="sxs-lookup"><span data-stu-id="23652-113">MailboxStats</span></span>](mailboxstats.md)
  
## <a name="remarks"></a><span data-ttu-id="23652-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="23652-114">Remarks</span></span>

<span data-ttu-id="23652-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="23652-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="23652-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="23652-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23652-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="23652-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23652-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="23652-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23652-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="23652-119">Schema name</span></span>  <br/> |<span data-ttu-id="23652-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="23652-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="23652-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="23652-121">Validation file</span></span>  <br/> |<span data-ttu-id="23652-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="23652-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="23652-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="23652-123">Can be empty</span></span>  <br/> |<span data-ttu-id="23652-124">false</span><span class="sxs-lookup"><span data-stu-id="23652-124">false</span></span>  <br/> |
   

