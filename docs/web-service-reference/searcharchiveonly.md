---
title: сеарчарчивеонли
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: Элемент Сеарчарчивеонли указывает, выполняется ли поиск только в архивном почтовом ящике для элементов, которые не индексируются.
ms.openlocfilehash: 9014044ed06c697cc43dd62103d7a1a907bda5a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460500"
---
# <a name="searcharchiveonly"></a><span data-ttu-id="cac59-103">сеарчарчивеонли</span><span class="sxs-lookup"><span data-stu-id="cac59-103">SearchArchiveOnly</span></span>

<span data-ttu-id="cac59-104">Элемент **сеарчарчивеонли** указывает, выполняется ли поиск только в архивном почтовом ящике для элементов, которые не индексируются.</span><span class="sxs-lookup"><span data-stu-id="cac59-104">The **SearchArchiveOnly** element indicates whether only the archive mailbox is searched for non-indexable items.</span></span> 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 <span data-ttu-id="cac59-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="cac59-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cac59-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cac59-106">Attributes and elements</span></span>

<span data-ttu-id="cac59-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cac59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cac59-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cac59-108">Attributes</span></span>

<span data-ttu-id="cac59-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cac59-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cac59-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cac59-110">Child elements</span></span>

<span data-ttu-id="cac59-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cac59-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cac59-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cac59-112">Parent elements</span></span>

<span data-ttu-id="cac59-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span><span class="sxs-lookup"><span data-stu-id="cac59-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="cac59-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cac59-114">Text value</span></span>

<span data-ttu-id="cac59-115">Текстовое значение **true** для элемента **сеарчарчивеонли** указывает на то, что поиск неиндексируемого элемента выполняется только в архивном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="cac59-115">A text value of **true** for the **SearchArchiveOnly** element indicates that non-indexable item search is only performed on the archive mailbox.</span></span> <span data-ttu-id="cac59-116">Текстовое значение **false** указывает на то, что выполняется поиск по основному почтовому ящику и архивному почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="cac59-116">A text value of **false** indicates that the search is performed against the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cac59-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="cac59-117">Remarks</span></span>

<span data-ttu-id="cac59-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cac59-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cac59-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cac59-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cac59-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cac59-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cac59-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cac59-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cac59-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cac59-122">Schema name</span></span>  <br/> |<span data-ttu-id="cac59-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cac59-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cac59-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cac59-124">Validation file</span></span>  <br/> |<span data-ttu-id="cac59-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cac59-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cac59-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cac59-126">Can be empty</span></span>  <br/> ||
   

