---
title: DestinationFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DestinationFolderId
api_type:
- schema
ms.assetid: 77d2d222-320b-4aab-88e4-934ef177f55c
description: Элемент DestinationFolderId определяет папку назначения для копирования и перемещения действия.
ms.openlocfilehash: 5fb6cae7db9cdb09e23b3627e26e695ecf6418f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762080"
---
# <a name="destinationfolderid"></a><span data-ttu-id="9aea3-103">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="9aea3-103">DestinationFolderId</span></span>

<span data-ttu-id="9aea3-104">Элемент **DestinationFolderId** определяет папку назначения для копирования и перемещения действия.</span><span class="sxs-lookup"><span data-stu-id="9aea3-104">The **DestinationFolderId** element indicates the destination folder for copy and move actions.</span></span> 
  
- [<span data-ttu-id="9aea3-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="9aea3-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="9aea3-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="9aea3-106">ConversationActions</span></span>](conversationactions.md) 
- [<span data-ttu-id="9aea3-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="9aea3-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="9aea3-108">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="9aea3-108">DestinationFolderId</span></span>](destinationfolderid.md)
  
```XML
<DestinationFolderId>
   <FolderId/>
</DestinationFolderId>
```

 <span data-ttu-id="9aea3-109">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="9aea3-109">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9aea3-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9aea3-110">Attributes and elements</span></span>

<span data-ttu-id="9aea3-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9aea3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9aea3-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9aea3-112">Attributes</span></span>

<span data-ttu-id="9aea3-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="9aea3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9aea3-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9aea3-114">Child elements</span></span>

|<span data-ttu-id="9aea3-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9aea3-115">**Element**</span></span>|<span data-ttu-id="9aea3-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9aea3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9aea3-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="9aea3-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="9aea3-118">Содержит идентификатор и ключ изменения папки назначения.</span><span class="sxs-lookup"><span data-stu-id="9aea3-118">Contains the identifier and change key of the destination folder.</span></span>  <br/> |
|[<span data-ttu-id="9aea3-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="9aea3-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="9aea3-120">Идентифицирует папки, которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="9aea3-120">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9aea3-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9aea3-121">Parent elements</span></span>

|<span data-ttu-id="9aea3-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9aea3-122">**Element**</span></span>|<span data-ttu-id="9aea3-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9aea3-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9aea3-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="9aea3-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="9aea3-125">Содержит одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="9aea3-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9aea3-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9aea3-126">Text value</span></span>

<span data-ttu-id="9aea3-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="9aea3-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9aea3-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="9aea3-128">Remarks</span></span>

<span data-ttu-id="9aea3-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9aea3-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9aea3-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9aea3-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9aea3-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9aea3-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9aea3-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9aea3-132">Schema Name</span></span>  <br/> |<span data-ttu-id="9aea3-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9aea3-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="9aea3-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9aea3-134">Validation File</span></span>  <br/> |<span data-ttu-id="9aea3-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9aea3-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9aea3-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9aea3-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="9aea3-137">False</span><span class="sxs-lookup"><span data-stu-id="9aea3-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9aea3-138">См. также</span><span class="sxs-lookup"><span data-stu-id="9aea3-138">See also</span></span>

- [<span data-ttu-id="9aea3-139">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="9aea3-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

