---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: Элемент BlockExternalImages указывает, заблокирован ли внешние изображения в теле текста HTML.
ms.openlocfilehash: 41ab2ec7ec1c24ccbbef037ef1e27431c1fe6811
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761562"
---
# <a name="blockexternalimages"></a><span data-ttu-id="e96f7-103">BlockExternalImages</span><span class="sxs-lookup"><span data-stu-id="e96f7-103">BlockExternalImages</span></span>

<span data-ttu-id="e96f7-104">Элемент **BlockExternalImages** указывает, заблокирован ли внешние изображения в теле текста HTML.</span><span class="sxs-lookup"><span data-stu-id="e96f7-104">The **BlockExternalImages** element specifies whether external images are blocked in HTML text bodies.</span></span> 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 <span data-ttu-id="e96f7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e96f7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e96f7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e96f7-106">Attributes and elements</span></span>

<span data-ttu-id="e96f7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e96f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e96f7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e96f7-108">Attributes</span></span>

<span data-ttu-id="e96f7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e96f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e96f7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e96f7-110">Child elements</span></span>

<span data-ttu-id="e96f7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e96f7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e96f7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e96f7-112">Parent elements</span></span>

|<span data-ttu-id="e96f7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e96f7-113">**Element**</span></span>|<span data-ttu-id="e96f7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e96f7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e96f7-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="e96f7-115">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="e96f7-116">Задает свойства папки для включения в ответе GetFolder, FindFolder или SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="e96f7-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span>  <br/> |
|[<span data-ttu-id="e96f7-117">ItemShape</span><span class="sxs-lookup"><span data-stu-id="e96f7-117">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="e96f7-118">Определяет свойства элемента и содержимого для включения в GetItem, FindItem или SyncFolderItems ответа.</span><span class="sxs-lookup"><span data-stu-id="e96f7-118">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e96f7-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e96f7-119">Text value</span></span>

<span data-ttu-id="e96f7-120">Текстовое значение **true** для элемента **BlockExternalImages** указывает, что внешние изображения блокируются в теле HTML-код.</span><span class="sxs-lookup"><span data-stu-id="e96f7-120">A text value of **true** for **BlockExternalImages** element indicates that external images are blocked in HTML bodies.</span></span> <span data-ttu-id="e96f7-121">Значение **false** указывает, что разрешенных внешних изображений.</span><span class="sxs-lookup"><span data-stu-id="e96f7-121">A value of **false** indicates that external images are allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e96f7-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="e96f7-122">Remarks</span></span>

<span data-ttu-id="e96f7-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e96f7-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e96f7-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e96f7-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e96f7-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e96f7-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e96f7-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e96f7-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e96f7-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e96f7-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e96f7-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="e96f7-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="e96f7-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e96f7-129">Validation File</span></span>  <br/> |<span data-ttu-id="e96f7-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e96f7-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e96f7-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e96f7-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e96f7-132">См. также</span><span class="sxs-lookup"><span data-stu-id="e96f7-132">See also</span></span>



- [<span data-ttu-id="e96f7-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e96f7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

