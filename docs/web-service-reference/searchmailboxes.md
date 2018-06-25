---
title: SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d8c367a-67e9-43b3-8be0-6362d2152431
description: Элемент SearchMailboxes указывает начало запроса SearchMailboxes.
ms.openlocfilehash: cf8007be3201e2248f27371c2a80c960735a3ced
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835306"
---
# <a name="searchmailboxes"></a><span data-ttu-id="d4d8e-103">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="d4d8e-103">SearchMailboxes</span></span>

<span data-ttu-id="d4d8e-104">Элемент **SearchMailboxes** указывает начало запроса **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="d4d8e-104">The **SearchMailboxes** element indicates the beginning of the **SearchMailboxes** request.</span></span> 
  
```XML
<SearchMailboxes>
   <SearchQueries/>
   <ResultType/>
   <PreviewItemResponseShape/>
   <SortBy/>
   <Language/>
   <Deduplication/>
   <PageSize/>
   <PageItemReference/>
   <PageDirection/>
</SearchMailboxes>
```

 <span data-ttu-id="d4d8e-105">**SearchMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="d4d8e-105">**SearchMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4d8e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d4d8e-106">Attributes and elements</span></span>

<span data-ttu-id="d4d8e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d4d8e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4d8e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d4d8e-108">Attributes</span></span>

<span data-ttu-id="d4d8e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d4d8e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4d8e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d4d8e-110">Child elements</span></span>

<span data-ttu-id="d4d8e-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [PreviewItemResponseShape](previewitemresponseshape.md) | [SortBy](sortby.md) | [язык](language.md) | [дедупликации](deduplication.md) | [PageSize](pagesize.md)  |  [ PageItemReference](pageitemreference.md) | [PageDirection](pagedirection.md)</span><span class="sxs-lookup"><span data-stu-id="d4d8e-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [PreviewItemResponseShape](previewitemresponseshape.md) | [SortBy](sortby.md) | [Language](language.md) | [Deduplication](deduplication.md) | [PageSize](pagesize.md) | [PageItemReference](pageitemreference.md) | [PageDirection](pagedirection.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4d8e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d4d8e-112">Parent elements</span></span>

<span data-ttu-id="d4d8e-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="d4d8e-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4d8e-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="d4d8e-114">Remarks</span></span>

<span data-ttu-id="d4d8e-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d4d8e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d4d8e-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4d8e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4d8e-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d4d8e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4d8e-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d4d8e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d4d8e-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d4d8e-119">Schema name</span></span>  <br/> |<span data-ttu-id="d4d8e-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d4d8e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d4d8e-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d4d8e-121">Validation file</span></span>  <br/> |<span data-ttu-id="d4d8e-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d4d8e-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4d8e-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d4d8e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="d4d8e-124">Нет</span><span class="sxs-lookup"><span data-stu-id="d4d8e-124">false</span></span>  <br/> |
   

