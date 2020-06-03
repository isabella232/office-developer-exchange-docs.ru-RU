---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: Элемент GetNonIndexableItemDetails указывает запрос на получение сведений о неиндексируемых элементах.
ms.openlocfilehash: 1c04b4cd7a86183210be869973c9779188fa0adf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458602"
---
# <a name="getnonindexableitemdetails"></a><span data-ttu-id="9c58e-103">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="9c58e-103">GetNonIndexableItemDetails</span></span>

<span data-ttu-id="9c58e-104">Элемент **GetNonIndexableItemDetails** указывает запрос на получение сведений о неиндексируемых элементах.</span><span class="sxs-lookup"><span data-stu-id="9c58e-104">The **GetNonIndexableItemDetails** element specifies a request to retrieve nonindexable item details.</span></span> 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 <span data-ttu-id="9c58e-105">**жетнониндексаблеитемдетаилстипе**</span><span class="sxs-lookup"><span data-stu-id="9c58e-105">**GetNonIndexableItemDetailsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c58e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9c58e-106">Attributes and elements</span></span>

<span data-ttu-id="9c58e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9c58e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c58e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9c58e-108">Attributes</span></span>

<span data-ttu-id="9c58e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9c58e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c58e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9c58e-110">Child elements</span></span>

|<span data-ttu-id="9c58e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9c58e-111">**Element**</span></span>|<span data-ttu-id="9c58e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9c58e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c58e-113">Почтовые ящики (Нонемптяррайофлегациднстипе)</span><span class="sxs-lookup"><span data-stu-id="9c58e-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="9c58e-114">Указывает массив элементов **почтового ящика** .</span><span class="sxs-lookup"><span data-stu-id="9c58e-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
|[<span data-ttu-id="9c58e-115">PageSize</span><span class="sxs-lookup"><span data-stu-id="9c58e-115">PageSize</span></span>](pagesize.md) <br/> |<span data-ttu-id="9c58e-116">Содержит количество элементов, возвращаемых на одной странице для результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="9c58e-116">Contains the number of items to be returned in a single page for a search result.</span></span>  <br/> |
|[<span data-ttu-id="9c58e-117">пажеитемреференце</span><span class="sxs-lookup"><span data-stu-id="9c58e-117">PageItemReference</span></span>](pageitemreference.md) <br/> |<span data-ttu-id="9c58e-118">Указывает ссылку на элемент страницы.</span><span class="sxs-lookup"><span data-stu-id="9c58e-118">Specifies the reference for a page item.</span></span>  <br/> |
|[<span data-ttu-id="9c58e-119">пажедиректион</span><span class="sxs-lookup"><span data-stu-id="9c58e-119">PageDirection</span></span>](pagedirection.md) <br/> |<span data-ttu-id="9c58e-120">Содержит направление разбивки в результатах поиска.</span><span class="sxs-lookup"><span data-stu-id="9c58e-120">Contains the direction for pagination in the search result.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c58e-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9c58e-121">Parent elements</span></span>

<span data-ttu-id="9c58e-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="9c58e-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9c58e-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="9c58e-123">Remarks</span></span>

<span data-ttu-id="9c58e-124">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9c58e-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9c58e-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c58e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c58e-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9c58e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c58e-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9c58e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9c58e-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9c58e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9c58e-129">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="9c58e-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="9c58e-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9c58e-130">Validation File</span></span>  <br/> |<span data-ttu-id="9c58e-131">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9c58e-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9c58e-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9c58e-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9c58e-133">См. также</span><span class="sxs-lookup"><span data-stu-id="9c58e-133">See also</span></span>



- [<span data-ttu-id="9c58e-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9c58e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

