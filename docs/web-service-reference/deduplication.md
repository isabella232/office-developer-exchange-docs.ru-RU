---
title: Дедупликации
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: Элемент дедупликации указывает, следует ли результат поиска удалять повторяющихся элементов.
ms.openlocfilehash: 3f06bb1dccd0677b7fd43c4ad82eda54a0c3f812
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762007"
---
# <a name="deduplication"></a><span data-ttu-id="42e36-103">Дедупликации</span><span class="sxs-lookup"><span data-stu-id="42e36-103">Deduplication</span></span>

<span data-ttu-id="42e36-104">Элемент **дедупликации** указывает, следует ли результат поиска удалять повторяющихся элементов.</span><span class="sxs-lookup"><span data-stu-id="42e36-104">The **Deduplication** element indicates whether the search result should remove duplicate items.</span></span> 
  
```XML
<Deduplication> true | false </Deduplication>
```

<span data-ttu-id="42e36-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="42e36-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="42e36-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="42e36-106">Attributes and elements</span></span>

<span data-ttu-id="42e36-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="42e36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42e36-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="42e36-108">Attributes</span></span>

<span data-ttu-id="42e36-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="42e36-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="42e36-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="42e36-110">Child elements</span></span>

<span data-ttu-id="42e36-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="42e36-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="42e36-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="42e36-112">Parent elements</span></span>

<span data-ttu-id="42e36-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="42e36-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="42e36-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="42e36-114">Text value</span></span>

<span data-ttu-id="42e36-115">Текстовое значение **true** для элемента дедупликации указывает, что результаты поиска не может содержать дублирующиеся элементы.</span><span class="sxs-lookup"><span data-stu-id="42e36-115">A text value of **true** for the Deduplication element indicates that search results may not contain duplicate items.</span></span> <span data-ttu-id="42e36-116">Значение **false** указывает, что результаты поиска может содержать дублирующиеся элементы.</span><span class="sxs-lookup"><span data-stu-id="42e36-116">A value of **false** indicates that search results may contain duplicate items.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="42e36-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="42e36-117">Remarks</span></span>

<span data-ttu-id="42e36-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="42e36-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="42e36-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="42e36-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42e36-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="42e36-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42e36-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="42e36-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="42e36-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="42e36-122">Schema name</span></span>  <br/> |<span data-ttu-id="42e36-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="42e36-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="42e36-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="42e36-124">Validation file</span></span>  <br/> |<span data-ttu-id="42e36-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="42e36-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="42e36-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="42e36-126">Can be empty</span></span>  <br/> |<span data-ttu-id="42e36-127">Нет</span><span class="sxs-lookup"><span data-stu-id="42e36-127">false</span></span>  <br/> |
   

