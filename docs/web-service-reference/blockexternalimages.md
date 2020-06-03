---
title: блоккекстерналимажес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: Элемент Блоккекстерналимажес указывает, блокируются ли внешние изображения в теле HTML-текста.
ms.openlocfilehash: 73342316024ebe476a0e35f14157befc80edcf83
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527406"
---
# <a name="blockexternalimages"></a><span data-ttu-id="4d966-103">блоккекстерналимажес</span><span class="sxs-lookup"><span data-stu-id="4d966-103">BlockExternalImages</span></span>

<span data-ttu-id="4d966-104">Элемент **блоккекстерналимажес** указывает, блокируются ли внешние изображения в теле HTML-текста.</span><span class="sxs-lookup"><span data-stu-id="4d966-104">The **BlockExternalImages** element specifies whether external images are blocked in HTML text bodies.</span></span> 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 <span data-ttu-id="4d966-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4d966-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d966-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4d966-106">Attributes and elements</span></span>

<span data-ttu-id="4d966-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4d966-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d966-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4d966-108">Attributes</span></span>

<span data-ttu-id="4d966-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4d966-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d966-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4d966-110">Child elements</span></span>

<span data-ttu-id="4d966-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4d966-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4d966-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4d966-112">Parent elements</span></span>

|<span data-ttu-id="4d966-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d966-113">**Element**</span></span>|<span data-ttu-id="4d966-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d966-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d966-115">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="4d966-115">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="4d966-116">Определяет свойства папки, которые необходимо включить в ответ "GetResponse Folder", "FindFolder" или "SyncFolderHierarchy".</span><span class="sxs-lookup"><span data-stu-id="4d966-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span>  <br/> |
|[<span data-ttu-id="4d966-117">итемшапе</span><span class="sxs-lookup"><span data-stu-id="4d966-117">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="4d966-118">Определяет свойства и контент элемента, включаемые в ответ GetItem, FindItem или SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="4d966-118">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4d966-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4d966-119">Text value</span></span>

<span data-ttu-id="4d966-120">Текстовое значение **true** для элемента **блоккекстерналимажес** указывает на то, что внешние изображения блокируются в HTML-тексте.</span><span class="sxs-lookup"><span data-stu-id="4d966-120">A text value of **true** for **BlockExternalImages** element indicates that external images are blocked in HTML bodies.</span></span> <span data-ttu-id="4d966-121">Значение **false** указывает, что внешние изображения разрешены.</span><span class="sxs-lookup"><span data-stu-id="4d966-121">A value of **false** indicates that external images are allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4d966-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="4d966-122">Remarks</span></span>

<span data-ttu-id="4d966-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4d966-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4d966-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d966-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d966-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4d966-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d966-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4d966-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d966-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4d966-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4d966-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="4d966-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="4d966-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4d966-129">Validation File</span></span>  <br/> |<span data-ttu-id="4d966-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4d966-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d966-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4d966-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4d966-132">См. также</span><span class="sxs-lookup"><span data-stu-id="4d966-132">See also</span></span>



- [<span data-ttu-id="4d966-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4d966-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

