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
ms.openlocfilehash: 357958e393ba9331d23ee48661f21e2afe00cf01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835518"
---
# <a name="sortby"></a><span data-ttu-id="a9849-103">SortBy</span><span class="sxs-lookup"><span data-stu-id="a9849-103">SortBy</span></span>

<span data-ttu-id="a9849-104">Элемент **SortBy** содержит свойство Item, используемое для сортировки результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="a9849-104">The **SortBy** element contains an item property used for sorting the search result.</span></span> 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 <span data-ttu-id="a9849-105">**фиелдордертипе**</span><span class="sxs-lookup"><span data-stu-id="a9849-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a9849-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a9849-106">Attributes and elements</span></span>

<span data-ttu-id="a9849-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a9849-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9849-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a9849-108">Attributes</span></span>

|<span data-ttu-id="a9849-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a9849-109">**Attribute**</span></span>|<span data-ttu-id="a9849-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a9849-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a9849-111">Порядок</span><span class="sxs-lookup"><span data-stu-id="a9849-111">Order</span></span>  <br/> |<span data-ttu-id="a9849-112">Текстовое значение атрибута **Order** — это порядок сортировки.</span><span class="sxs-lookup"><span data-stu-id="a9849-112">The text value of the **Order** attribute is the sort order.</span></span> <span data-ttu-id="a9849-113">Текстовое значение по **возрастанию** указывает на то, что результаты представлены в возрастающем порядке.</span><span class="sxs-lookup"><span data-stu-id="a9849-113">A text value of **Ascending** indicates that the results are in ascending order.</span></span> <span data-ttu-id="a9849-114">Текстовое значение "по **убыванию** " указывает на то, что результаты представлены в убывающем порядке.</span><span class="sxs-lookup"><span data-stu-id="a9849-114">A text value of **Descending** indicates that the results are in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a9849-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a9849-115">Child elements</span></span>

<span data-ttu-id="a9849-116">[Фиелдури](fielduri.md) | [индекседфиелдури](indexedfielduri.md)</span><span class="sxs-lookup"><span data-stu-id="a9849-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a9849-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a9849-117">Parent elements</span></span>

[<span data-ttu-id="a9849-118">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="a9849-118">SearchMailboxes</span></span>](searchmailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="a9849-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="a9849-119">Remarks</span></span>

<span data-ttu-id="a9849-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a9849-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a9849-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9849-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9849-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a9849-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9849-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a9849-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a9849-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a9849-124">Schema name</span></span>  <br/> |<span data-ttu-id="a9849-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a9849-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a9849-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a9849-126">Validation file</span></span>  <br/> |<span data-ttu-id="a9849-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a9849-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a9849-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a9849-128">Can be empty</span></span>  <br/> ||
   

