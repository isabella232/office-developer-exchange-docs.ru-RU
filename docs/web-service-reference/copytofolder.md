---
title: CopyToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyToFolder
api_type:
- schema
ms.assetid: 6fd8a6b8-d813-43ff-991b-0e9e782fe00e
description: Элемент CopyToFolder указывает идентификатор папки сообщение электронной почты, можно скопировать элементы.
ms.openlocfilehash: b641c23b7aed11ae85157e2ed01cfa9d61d07e0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761844"
---
# <a name="copytofolder"></a><span data-ttu-id="06ee0-103">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="06ee0-103">CopyToFolder</span></span>

<span data-ttu-id="06ee0-104">Элемент **CopyToFolder** указывает идентификатор папки сообщение электронной почты, можно скопировать элементы.</span><span class="sxs-lookup"><span data-stu-id="06ee0-104">The **CopyToFolder** element specifies the identifier of the folder that email items can be copied to.</span></span> 
  
```XML
<CopyToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</CopyToFolder>
```

 <span data-ttu-id="06ee0-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="06ee0-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06ee0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="06ee0-106">Attributes and elements</span></span>

<span data-ttu-id="06ee0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="06ee0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06ee0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="06ee0-108">Attributes</span></span>

<span data-ttu-id="06ee0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="06ee0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06ee0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="06ee0-110">Child elements</span></span>

|<span data-ttu-id="06ee0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="06ee0-111">**Element**</span></span>|<span data-ttu-id="06ee0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="06ee0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06ee0-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="06ee0-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="06ee0-114">Содержит идентификатор конечной папки для копируемые или перемещения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="06ee0-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="06ee0-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="06ee0-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="06ee0-116">Определяет именованный конечной папки для копируемые или перемещения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="06ee0-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06ee0-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="06ee0-117">Parent elements</span></span>

|<span data-ttu-id="06ee0-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="06ee0-118">**Element**</span></span>|<span data-ttu-id="06ee0-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="06ee0-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06ee0-120">Действия</span><span class="sxs-lookup"><span data-stu-id="06ee0-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="06ee0-121">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="06ee0-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06ee0-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="06ee0-122">Text value</span></span>

<span data-ttu-id="06ee0-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="06ee0-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06ee0-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="06ee0-124">Remarks</span></span>

<span data-ttu-id="06ee0-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="06ee0-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06ee0-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="06ee0-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06ee0-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="06ee0-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="06ee0-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="06ee0-128">Schema Name</span></span>  <br/> |<span data-ttu-id="06ee0-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="06ee0-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="06ee0-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="06ee0-130">Validation File</span></span>  <br/> |<span data-ttu-id="06ee0-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="06ee0-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06ee0-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="06ee0-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="06ee0-133">True</span><span class="sxs-lookup"><span data-stu-id="06ee0-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06ee0-134">См. также</span><span class="sxs-lookup"><span data-stu-id="06ee0-134">See also</span></span>



[<span data-ttu-id="06ee0-135">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="06ee0-135">MoveToFolder</span></span>](movetofolder.md)


- [<span data-ttu-id="06ee0-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="06ee0-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

