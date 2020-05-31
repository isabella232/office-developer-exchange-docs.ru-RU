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
description: Элемент CopyItem определяет запрос на копирование элемента в почтовом ящике в хранилище Exchange.
ms.openlocfilehash: 08cc1b67f7c7d369263acfc4b3d13e8aa70d2d5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761842"
---
# <a name="copyitem"></a><span data-ttu-id="399bc-103">CopyItem</span><span class="sxs-lookup"><span data-stu-id="399bc-103">CopyItem</span></span>

<span data-ttu-id="399bc-104">Элемент **CopyItem** определяет запрос на копирование элемента в почтовом ящике в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="399bc-104">The **CopyItem** element defines a request to copy an item in a mailbox in the Exchange store.</span></span> 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 <span data-ttu-id="399bc-105">**копитемтипе**</span><span class="sxs-lookup"><span data-stu-id="399bc-105">**CopyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="399bc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="399bc-106">Attributes and elements</span></span>

<span data-ttu-id="399bc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="399bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="399bc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="399bc-108">Attributes</span></span>

<span data-ttu-id="399bc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="399bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="399bc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="399bc-110">Child elements</span></span>

|<span data-ttu-id="399bc-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="399bc-111">**Element**</span></span>|<span data-ttu-id="399bc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="399bc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="399bc-113">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="399bc-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="399bc-114">Представляет папку назначения для скопированного элемента.</span><span class="sxs-lookup"><span data-stu-id="399bc-114">Represents the destination folder for a copied item.</span></span>  <br/> |
|[<span data-ttu-id="399bc-115">итемидс</span><span class="sxs-lookup"><span data-stu-id="399bc-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="399bc-116">Содержит массив идентифицированных элементов, которые необходимо скопировать в папку, представленную элементом [тофолдерид](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="399bc-116">Contains an array of identified items to copy to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="399bc-117">ретурнневитемидс</span><span class="sxs-lookup"><span data-stu-id="399bc-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="399bc-118">Указывает, возвращаются ли в ответе идентификаторы элементов новых элементов.</span><span class="sxs-lookup"><span data-stu-id="399bc-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="399bc-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="399bc-119">Parent elements</span></span>

<span data-ttu-id="399bc-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="399bc-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="399bc-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="399bc-121">Remarks</span></span>

<span data-ttu-id="399bc-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="399bc-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="399bc-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="399bc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="399bc-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="399bc-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="399bc-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="399bc-125">Schema Name</span></span>  <br/> |<span data-ttu-id="399bc-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="399bc-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="399bc-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="399bc-127">Validation File</span></span>  <br/> |<span data-ttu-id="399bc-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="399bc-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="399bc-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="399bc-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="399bc-130">False</span><span class="sxs-lookup"><span data-stu-id="399bc-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="399bc-131">См. также</span><span class="sxs-lookup"><span data-stu-id="399bc-131">See also</span></span>



[<span data-ttu-id="399bc-132">Операция CopyItem</span><span class="sxs-lookup"><span data-stu-id="399bc-132">CopyItem operation</span></span>](copyitem-operation.md)


- [<span data-ttu-id="399bc-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="399bc-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

