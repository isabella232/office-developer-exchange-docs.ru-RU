---
title: CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: ffb4c13e-e7ea-4e6b-87a0-509ce5371100
description: Элемент CopyItem определяет запрос для копирования элемента в почтовом ящике в хранилище Exchange.
ms.openlocfilehash: 08cc1b67f7c7d369263acfc4b3d13e8aa70d2d5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761842"
---
# <a name="copyitem"></a><span data-ttu-id="d284b-103">CopyItem</span><span class="sxs-lookup"><span data-stu-id="d284b-103">CopyItem</span></span>

<span data-ttu-id="d284b-104">Элемент **CopyItem** определяет запрос для копирования элемента в почтовом ящике в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d284b-104">The **CopyItem** element defines a request to copy an item in a mailbox in the Exchange store.</span></span> 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 <span data-ttu-id="d284b-105">**CopyItemType**</span><span class="sxs-lookup"><span data-stu-id="d284b-105">**CopyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d284b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d284b-106">Attributes and elements</span></span>

<span data-ttu-id="d284b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d284b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d284b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d284b-108">Attributes</span></span>

<span data-ttu-id="d284b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d284b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d284b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d284b-110">Child elements</span></span>

|<span data-ttu-id="d284b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d284b-111">**Element**</span></span>|<span data-ttu-id="d284b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d284b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d284b-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="d284b-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="d284b-114">Представляет конечной папки для скопированного элемента.</span><span class="sxs-lookup"><span data-stu-id="d284b-114">Represents the destination folder for a copied item.</span></span>  <br/> |
|[<span data-ttu-id="d284b-115">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="d284b-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="d284b-116">Содержит массив определенных элементов для копирования в папку, представленного элементом [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="d284b-116">Contains an array of identified items to copy to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="d284b-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="d284b-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="d284b-118">Указывает, возвращаются ли идентификаторы элементов новых элементов в ответе.</span><span class="sxs-lookup"><span data-stu-id="d284b-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d284b-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d284b-119">Parent elements</span></span>

<span data-ttu-id="d284b-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="d284b-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d284b-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="d284b-121">Remarks</span></span>

<span data-ttu-id="d284b-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d284b-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d284b-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d284b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d284b-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d284b-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d284b-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d284b-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d284b-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d284b-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d284b-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d284b-127">Validation File</span></span>  <br/> |<span data-ttu-id="d284b-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d284b-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d284b-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d284b-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="d284b-130">False</span><span class="sxs-lookup"><span data-stu-id="d284b-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d284b-131">См. также</span><span class="sxs-lookup"><span data-stu-id="d284b-131">See also</span></span>



[<span data-ttu-id="d284b-132">CopyItem Operation</span><span class="sxs-lookup"><span data-stu-id="d284b-132">CopyItem operation</span></span>](copyitem-operation.md)


- [<span data-ttu-id="d284b-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d284b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

