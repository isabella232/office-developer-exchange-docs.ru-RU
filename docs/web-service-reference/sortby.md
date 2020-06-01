---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: Элемент SortBy содержит свойство Item, используемое для сортировки результатов поиска.
ms.openlocfilehash: cf2b1e633bc66e526028078833afade363e4c5e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468399"
---
# <a name="sortby"></a><span data-ttu-id="078d5-103">SortBy</span><span class="sxs-lookup"><span data-stu-id="078d5-103">SortBy</span></span>

<span data-ttu-id="078d5-104">Элемент **SortBy** содержит свойство Item, используемое для сортировки результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="078d5-104">The **SortBy** element contains an item property used for sorting the search result.</span></span> 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 <span data-ttu-id="078d5-105">**фиелдордертипе**</span><span class="sxs-lookup"><span data-stu-id="078d5-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="078d5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="078d5-106">Attributes and elements</span></span>

<span data-ttu-id="078d5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="078d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="078d5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="078d5-108">Attributes</span></span>

|<span data-ttu-id="078d5-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="078d5-109">**Attribute**</span></span>|<span data-ttu-id="078d5-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="078d5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="078d5-111">Порядок</span><span class="sxs-lookup"><span data-stu-id="078d5-111">Order</span></span>  <br/> |<span data-ttu-id="078d5-112">Текстовое значение атрибута **Order** — это порядок сортировки.</span><span class="sxs-lookup"><span data-stu-id="078d5-112">The text value of the **Order** attribute is the sort order.</span></span> <span data-ttu-id="078d5-113">Текстовое значение по **возрастанию** указывает на то, что результаты представлены в возрастающем порядке.</span><span class="sxs-lookup"><span data-stu-id="078d5-113">A text value of **Ascending** indicates that the results are in ascending order.</span></span> <span data-ttu-id="078d5-114">Текстовое значение "по **убыванию** " указывает на то, что результаты представлены в убывающем порядке.</span><span class="sxs-lookup"><span data-stu-id="078d5-114">A text value of **Descending** indicates that the results are in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="078d5-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="078d5-115">Child elements</span></span>

<span data-ttu-id="078d5-116">[Фиелдури](fielduri.md)  |  [Индекседфиелдури](indexedfielduri.md)</span><span class="sxs-lookup"><span data-stu-id="078d5-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="078d5-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="078d5-117">Parent elements</span></span>

[<span data-ttu-id="078d5-118">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="078d5-118">SearchMailboxes</span></span>](searchmailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="078d5-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="078d5-119">Remarks</span></span>

<span data-ttu-id="078d5-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="078d5-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="078d5-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="078d5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="078d5-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="078d5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="078d5-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="078d5-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="078d5-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="078d5-124">Schema name</span></span>  <br/> |<span data-ttu-id="078d5-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="078d5-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="078d5-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="078d5-126">Validation file</span></span>  <br/> |<span data-ttu-id="078d5-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="078d5-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="078d5-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="078d5-128">Can be empty</span></span>  <br/> ||
   

