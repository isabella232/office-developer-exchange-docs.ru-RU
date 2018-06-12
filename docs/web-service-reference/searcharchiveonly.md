---
title: SearchArchiveOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: Элемент SearchArchiveOnly указывает только архивного почтового ящика в поисках Неиндексируемых элементов.
ms.openlocfilehash: ac9d3262784d8052486c631ef3e99e650d4757c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835293"
---
# <a name="searcharchiveonly"></a><span data-ttu-id="e2f5f-103">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="e2f5f-103">SearchArchiveOnly</span></span>

<span data-ttu-id="e2f5f-104">Элемент **SearchArchiveOnly** указывает только архивного почтового ящика в поисках Неиндексируемых элементов.</span><span class="sxs-lookup"><span data-stu-id="e2f5f-104">The **SearchArchiveOnly** element indicates whether only the archive mailbox is searched for non-indexable items.</span></span> 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 <span data-ttu-id="e2f5f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e2f5f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2f5f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e2f5f-106">Attributes and elements</span></span>

<span data-ttu-id="e2f5f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e2f5f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2f5f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e2f5f-108">Attributes</span></span>

<span data-ttu-id="e2f5f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e2f5f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2f5f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e2f5f-110">Child elements</span></span>

<span data-ttu-id="e2f5f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e2f5f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e2f5f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e2f5f-112">Parent elements</span></span>

<span data-ttu-id="e2f5f-113">│ [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span><span class="sxs-lookup"><span data-stu-id="e2f5f-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="e2f5f-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e2f5f-114">Text value</span></span>

<span data-ttu-id="e2f5f-115">Текстовое значение **true** для элемента **SearchArchiveOnly** указывает, что, что поиск неиндексируемых элемента выполняется только на архивного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e2f5f-115">A text value of **true** for the **SearchArchiveOnly** element indicates that non-indexable item search is only performed on the archive mailbox.</span></span> <span data-ttu-id="e2f5f-116">Текстовое значение **false** указывает, что поиск выполняется от основного почтового ящика и архивного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e2f5f-116">A text value of **false** indicates that the search is performed against the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e2f5f-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="e2f5f-117">Remarks</span></span>

<span data-ttu-id="e2f5f-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e2f5f-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e2f5f-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2f5f-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2f5f-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e2f5f-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2f5f-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e2f5f-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e2f5f-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e2f5f-122">Schema name</span></span>  <br/> |<span data-ttu-id="e2f5f-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e2f5f-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e2f5f-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e2f5f-124">Validation file</span></span>  <br/> |<span data-ttu-id="e2f5f-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e2f5f-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e2f5f-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e2f5f-126">Can be empty</span></span>  <br/> ||
   

