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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761842"
---
# <a name="copyitem"></a><span data-ttu-id="7c163-103">CopyItem</span><span class="sxs-lookup"><span data-stu-id="7c163-103">CopyItem</span></span>

<span data-ttu-id="7c163-104">Элемент **CopyItem** определяет запрос для копирования элемента в почтовом ящике в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c163-104">The **CopyItem** element defines a request to copy an item in a mailbox in the Exchange store.</span></span> 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 <span data-ttu-id="7c163-105">**CopyItemType**</span><span class="sxs-lookup"><span data-stu-id="7c163-105">**CopyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c163-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7c163-106">Attributes and elements</span></span>

<span data-ttu-id="7c163-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7c163-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c163-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7c163-108">Attributes</span></span>

<span data-ttu-id="7c163-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7c163-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c163-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7c163-110">Child elements</span></span>

|<span data-ttu-id="7c163-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c163-111">**Element**</span></span>|<span data-ttu-id="7c163-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c163-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c163-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="7c163-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="7c163-114">Представляет конечной папки для скопированного элемента.</span><span class="sxs-lookup"><span data-stu-id="7c163-114">Represents the destination folder for a copied item.</span></span>  <br/> |
|[<span data-ttu-id="7c163-115">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="7c163-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="7c163-116">Содержит массив определенных элементов для копирования в папку, представленного элементом [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="7c163-116">Contains an array of identified items to copy to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="7c163-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="7c163-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="7c163-118">Указывает, возвращаются ли идентификаторы элементов новых элементов в ответе.</span><span class="sxs-lookup"><span data-stu-id="7c163-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c163-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7c163-119">Parent elements</span></span>

<span data-ttu-id="7c163-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="7c163-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7c163-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="7c163-121">Remarks</span></span>

<span data-ttu-id="7c163-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c163-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c163-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7c163-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c163-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7c163-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7c163-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7c163-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7c163-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7c163-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7c163-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7c163-127">Validation File</span></span>  <br/> |<span data-ttu-id="7c163-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7c163-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7c163-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7c163-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c163-130">False</span><span class="sxs-lookup"><span data-stu-id="7c163-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c163-131">См. также</span><span class="sxs-lookup"><span data-stu-id="7c163-131">See also</span></span>



[<span data-ttu-id="7c163-132">CopyItem Operation</span><span class="sxs-lookup"><span data-stu-id="7c163-132">CopyItem operation</span></span>](copyitem-operation.md)


- [<span data-ttu-id="7c163-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7c163-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

