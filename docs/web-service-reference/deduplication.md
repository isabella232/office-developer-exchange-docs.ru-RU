---
title: Дедупликацию
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: Элемент дедупликации указывает, должен ли результат поиска удалять повторяющиеся элементы.
ms.openlocfilehash: c39f980658aba7036cfabb3b51af5a41005f97b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463715"
---
# <a name="deduplication"></a><span data-ttu-id="9a417-103">Дедупликацию</span><span class="sxs-lookup"><span data-stu-id="9a417-103">Deduplication</span></span>

<span data-ttu-id="9a417-104">Элемент **дедупликации** указывает, должен ли результат поиска удалять повторяющиеся элементы.</span><span class="sxs-lookup"><span data-stu-id="9a417-104">The **Deduplication** element indicates whether the search result should remove duplicate items.</span></span> 
  
```XML
<Deduplication> true | false </Deduplication>
```

<span data-ttu-id="9a417-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9a417-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9a417-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9a417-106">Attributes and elements</span></span>

<span data-ttu-id="9a417-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9a417-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a417-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9a417-108">Attributes</span></span>

<span data-ttu-id="9a417-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9a417-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a417-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9a417-110">Child elements</span></span>

<span data-ttu-id="9a417-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9a417-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9a417-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9a417-112">Parent elements</span></span>

<span data-ttu-id="9a417-113">[SearchMailboxes](searchmailboxes.md)  |  [SetHoldOnMailboxes](setholdonmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="9a417-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9a417-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9a417-114">Text value</span></span>

<span data-ttu-id="9a417-115">Текстовое значение **true** для элемента дедупликации указывает на то, что результаты поиска не могут содержать дублирующиеся элементы.</span><span class="sxs-lookup"><span data-stu-id="9a417-115">A text value of **true** for the Deduplication element indicates that search results may not contain duplicate items.</span></span> <span data-ttu-id="9a417-116">Значение **false** указывает, что результаты поиска могут содержать дублирующиеся элементы.</span><span class="sxs-lookup"><span data-stu-id="9a417-116">A value of **false** indicates that search results may contain duplicate items.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9a417-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="9a417-117">Remarks</span></span>

<span data-ttu-id="9a417-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9a417-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9a417-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9a417-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a417-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9a417-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a417-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9a417-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9a417-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9a417-122">Schema name</span></span>  <br/> |<span data-ttu-id="9a417-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9a417-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="9a417-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9a417-124">Validation file</span></span>  <br/> |<span data-ttu-id="9a417-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9a417-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9a417-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9a417-126">Can be empty</span></span>  <br/> |<span data-ttu-id="9a417-127">false</span><span class="sxs-lookup"><span data-stu-id="9a417-127">false</span></span>  <br/> |
   

