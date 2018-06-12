---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: Элемент GetNonIndexableItemDetails определяет запрос для получения сведений об элементе nonindexable.
ms.openlocfilehash: 0aeda85973aa78eff240a017db58ffb57fc0de06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762850"
---
# <a name="getnonindexableitemdetails"></a><span data-ttu-id="7a8a4-103">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="7a8a4-103">GetNonIndexableItemDetails</span></span>

<span data-ttu-id="7a8a4-104">Элемент **GetNonIndexableItemDetails** определяет запрос для получения сведений об элементе nonindexable.</span><span class="sxs-lookup"><span data-stu-id="7a8a4-104">The **GetNonIndexableItemDetails** element specifies a request to retrieve nonindexable item details.</span></span> 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 <span data-ttu-id="7a8a4-105">**GetNonIndexableItemDetailsType**</span><span class="sxs-lookup"><span data-stu-id="7a8a4-105">**GetNonIndexableItemDetailsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a8a4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7a8a4-106">Attributes and elements</span></span>

<span data-ttu-id="7a8a4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7a8a4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a8a4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7a8a4-108">Attributes</span></span>

<span data-ttu-id="7a8a4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7a8a4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a8a4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7a8a4-110">Child elements</span></span>

|<span data-ttu-id="7a8a4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7a8a4-111">**Element**</span></span>|<span data-ttu-id="7a8a4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7a8a4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a8a4-113">Почтовые ящики (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="7a8a4-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="7a8a4-114">Указывает массив элементов **почтового ящика** .</span><span class="sxs-lookup"><span data-stu-id="7a8a4-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
|[<span data-ttu-id="7a8a4-115">PageSize</span><span class="sxs-lookup"><span data-stu-id="7a8a4-115">PageSize</span></span>](pagesize.md) <br/> |<span data-ttu-id="7a8a4-116">Содержит число элементов, возвращаемых на одной странице для результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="7a8a4-116">Contains the number of items to be returned in a single page for a search result.</span></span>  <br/> |
|[<span data-ttu-id="7a8a4-117">PageItemReference</span><span class="sxs-lookup"><span data-stu-id="7a8a4-117">PageItemReference</span></span>](pageitemreference.md) <br/> |<span data-ttu-id="7a8a4-118">— Ссылка для элемента страницы.</span><span class="sxs-lookup"><span data-stu-id="7a8a4-118">Specifies the reference for a page item.</span></span>  <br/> |
|[<span data-ttu-id="7a8a4-119">PageDirection</span><span class="sxs-lookup"><span data-stu-id="7a8a4-119">PageDirection</span></span>](pagedirection.md) <br/> |<span data-ttu-id="7a8a4-120">Содержит направление для разбивки на страницы в результатах поиска.</span><span class="sxs-lookup"><span data-stu-id="7a8a4-120">Contains the direction for pagination in the search result.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a8a4-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7a8a4-121">Parent elements</span></span>

<span data-ttu-id="7a8a4-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="7a8a4-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7a8a4-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="7a8a4-123">Remarks</span></span>

<span data-ttu-id="7a8a4-124">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7a8a4-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7a8a4-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a8a4-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a8a4-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7a8a4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a8a4-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7a8a4-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7a8a4-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7a8a4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7a8a4-129">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="7a8a4-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="7a8a4-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7a8a4-130">Validation File</span></span>  <br/> |<span data-ttu-id="7a8a4-131">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7a8a4-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7a8a4-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7a8a4-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7a8a4-133">См. также</span><span class="sxs-lookup"><span data-stu-id="7a8a4-133">See also</span></span>



- [<span data-ttu-id="7a8a4-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7a8a4-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

