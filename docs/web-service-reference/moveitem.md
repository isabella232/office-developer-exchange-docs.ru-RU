---
title: MoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItem
api_type:
- schema
ms.assetid: a4593377-22dd-415f-b01d-387389ef650f
description: Элемент MoveItem определяет запрос на перемещение элемента в хранилище Exchange.
ms.openlocfilehash: 61dbb91cc20a71f50999241b3daa21bf8ebfbcc8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530403"
---
# <a name="moveitem"></a><span data-ttu-id="f3214-103">MoveItem</span><span class="sxs-lookup"><span data-stu-id="f3214-103">MoveItem</span></span>

<span data-ttu-id="f3214-104">Элемент **MoveItem** определяет запрос на перемещение элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3214-104">The **MoveItem** element defines a request to move an item in the Exchange store.</span></span> 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 <span data-ttu-id="f3214-105">**мовеитемтипе**</span><span class="sxs-lookup"><span data-stu-id="f3214-105">**MoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3214-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f3214-106">Attributes and elements</span></span>

<span data-ttu-id="f3214-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f3214-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3214-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f3214-108">Attributes</span></span>

<span data-ttu-id="f3214-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3214-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3214-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f3214-110">Child elements</span></span>

|<span data-ttu-id="f3214-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f3214-111">**Element**</span></span>|<span data-ttu-id="f3214-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f3214-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3214-113">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="f3214-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="f3214-114">Представляет папку назначения для перемещенного элемента.</span><span class="sxs-lookup"><span data-stu-id="f3214-114">Represents the destination folder for a moved item.</span></span>  <br/> |
|[<span data-ttu-id="f3214-115">итемидс</span><span class="sxs-lookup"><span data-stu-id="f3214-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="f3214-116">Содержит массив идентифицированных элементов для перемещения в папку, представленную элементом [тофолдерид](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="f3214-116">Contains an array of identified items to move to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="f3214-117">ретурнневитемидс</span><span class="sxs-lookup"><span data-stu-id="f3214-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="f3214-118">Указывает, возвращаются ли в ответе идентификаторы элементов новых элементов.</span><span class="sxs-lookup"><span data-stu-id="f3214-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3214-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f3214-119">Parent elements</span></span>

<span data-ttu-id="f3214-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3214-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f3214-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f3214-121">Text value</span></span>

<span data-ttu-id="f3214-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="f3214-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3214-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="f3214-123">Remarks</span></span>

<span data-ttu-id="f3214-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3214-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3214-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f3214-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3214-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f3214-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f3214-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f3214-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f3214-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f3214-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f3214-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f3214-129">Validation File</span></span>  <br/> |<span data-ttu-id="f3214-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f3214-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3214-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f3214-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3214-132">False</span><span class="sxs-lookup"><span data-stu-id="f3214-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3214-133">См. также</span><span class="sxs-lookup"><span data-stu-id="f3214-133">See also</span></span>



[<span data-ttu-id="f3214-134">Операция MoveItem</span><span class="sxs-lookup"><span data-stu-id="f3214-134">MoveItem operation</span></span>](moveitem-operation.md)


- [<span data-ttu-id="f3214-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f3214-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

