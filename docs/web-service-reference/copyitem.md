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
ms.openlocfilehash: b9af1670fd580107de08ad3b950191399436388d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458504"
---
# <a name="copyitem"></a><span data-ttu-id="0a47c-103">CopyItem</span><span class="sxs-lookup"><span data-stu-id="0a47c-103">CopyItem</span></span>

<span data-ttu-id="0a47c-104">Элемент **CopyItem** определяет запрос на копирование элемента в почтовом ящике в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a47c-104">The **CopyItem** element defines a request to copy an item in a mailbox in the Exchange store.</span></span> 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 <span data-ttu-id="0a47c-105">**копитемтипе**</span><span class="sxs-lookup"><span data-stu-id="0a47c-105">**CopyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a47c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0a47c-106">Attributes and elements</span></span>

<span data-ttu-id="0a47c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0a47c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a47c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0a47c-108">Attributes</span></span>

<span data-ttu-id="0a47c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0a47c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a47c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0a47c-110">Child elements</span></span>

|<span data-ttu-id="0a47c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0a47c-111">**Element**</span></span>|<span data-ttu-id="0a47c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0a47c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a47c-113">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="0a47c-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="0a47c-114">Представляет папку назначения для скопированного элемента.</span><span class="sxs-lookup"><span data-stu-id="0a47c-114">Represents the destination folder for a copied item.</span></span>  <br/> |
|[<span data-ttu-id="0a47c-115">итемидс</span><span class="sxs-lookup"><span data-stu-id="0a47c-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="0a47c-116">Содержит массив идентифицированных элементов, которые необходимо скопировать в папку, представленную элементом [тофолдерид](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="0a47c-116">Contains an array of identified items to copy to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="0a47c-117">ретурнневитемидс</span><span class="sxs-lookup"><span data-stu-id="0a47c-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="0a47c-118">Указывает, возвращаются ли в ответе идентификаторы элементов новых элементов.</span><span class="sxs-lookup"><span data-stu-id="0a47c-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a47c-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0a47c-119">Parent elements</span></span>

<span data-ttu-id="0a47c-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="0a47c-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0a47c-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="0a47c-121">Remarks</span></span>

<span data-ttu-id="0a47c-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a47c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a47c-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0a47c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a47c-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0a47c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0a47c-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0a47c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0a47c-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0a47c-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0a47c-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0a47c-127">Validation File</span></span>  <br/> |<span data-ttu-id="0a47c-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0a47c-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0a47c-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0a47c-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="0a47c-130">False</span><span class="sxs-lookup"><span data-stu-id="0a47c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a47c-131">См. также</span><span class="sxs-lookup"><span data-stu-id="0a47c-131">See also</span></span>



[<span data-ttu-id="0a47c-132">Операция CopyItem</span><span class="sxs-lookup"><span data-stu-id="0a47c-132">CopyItem operation</span></span>](copyitem-operation.md)


- [<span data-ttu-id="0a47c-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0a47c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

