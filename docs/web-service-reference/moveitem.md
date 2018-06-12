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
ms.openlocfilehash: cd7f35bdabe8a596f4c186df1c8cd54e0ea1c540
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834486"
---
# <a name="moveitem"></a><span data-ttu-id="0e04d-103">MoveItem</span><span class="sxs-lookup"><span data-stu-id="0e04d-103">MoveItem</span></span>

<span data-ttu-id="0e04d-104">Элемент **MoveItem** определяет запрос на перемещение элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0e04d-104">The **MoveItem** element defines a request to move an item in the Exchange store.</span></span> 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 <span data-ttu-id="0e04d-105">**MoveItemType**</span><span class="sxs-lookup"><span data-stu-id="0e04d-105">**MoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e04d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0e04d-106">Attributes and elements</span></span>

<span data-ttu-id="0e04d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0e04d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e04d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0e04d-108">Attributes</span></span>

<span data-ttu-id="0e04d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0e04d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e04d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0e04d-110">Child elements</span></span>

|<span data-ttu-id="0e04d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0e04d-111">**Element**</span></span>|<span data-ttu-id="0e04d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0e04d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e04d-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="0e04d-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="0e04d-114">Представляет конечную папку для перемещения элемента.</span><span class="sxs-lookup"><span data-stu-id="0e04d-114">Represents the destination folder for a moved item.</span></span>  <br/> |
|[<span data-ttu-id="0e04d-115">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="0e04d-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="0e04d-116">Содержит массив определенных элементов для перемещения в папку, представленного элементом [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="0e04d-116">Contains an array of identified items to move to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="0e04d-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="0e04d-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="0e04d-118">Указывает, возвращаются ли идентификаторы элементов новых элементов в ответе.</span><span class="sxs-lookup"><span data-stu-id="0e04d-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0e04d-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0e04d-119">Parent elements</span></span>

<span data-ttu-id="0e04d-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="0e04d-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0e04d-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0e04d-121">Text value</span></span>

<span data-ttu-id="0e04d-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="0e04d-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0e04d-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="0e04d-123">Remarks</span></span>

<span data-ttu-id="0e04d-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0e04d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e04d-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0e04d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e04d-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0e04d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0e04d-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0e04d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="0e04d-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0e04d-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0e04d-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0e04d-129">Validation File</span></span>  <br/> |<span data-ttu-id="0e04d-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0e04d-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0e04d-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0e04d-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e04d-132">False</span><span class="sxs-lookup"><span data-stu-id="0e04d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e04d-133">См. также</span><span class="sxs-lookup"><span data-stu-id="0e04d-133">See also</span></span>



[<span data-ttu-id="0e04d-134">MoveItem Operation</span><span class="sxs-lookup"><span data-stu-id="0e04d-134">MoveItem operation</span></span>](moveitem-operation.md)


- [<span data-ttu-id="0e04d-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0e04d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

