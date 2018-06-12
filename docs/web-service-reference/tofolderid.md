---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: Элемент ToFolderId представляет конечной папки для копируемые или перемещения элемента или папки.
ms.openlocfilehash: a48309f0b7f5c9bf667fc2eb653a0502832bc996
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840198"
---
# <a name="tofolderid"></a><span data-ttu-id="0c103-103">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="0c103-103">ToFolderId</span></span>

<span data-ttu-id="0c103-104">Элемент **ToFolderId** представляет конечной папки для копируемые или перемещения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="0c103-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

 <span data-ttu-id="0c103-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="0c103-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c103-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0c103-106">Attributes and elements</span></span>

<span data-ttu-id="0c103-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0c103-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c103-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0c103-108">Attributes</span></span>

<span data-ttu-id="0c103-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0c103-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c103-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0c103-110">Child elements</span></span>

|<span data-ttu-id="0c103-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c103-111">**Element**</span></span>|<span data-ttu-id="0c103-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c103-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c103-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="0c103-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="0c103-114">Содержит идентификатор конечной папки для копируемые или перемещения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="0c103-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="0c103-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="0c103-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="0c103-116">Определяет именованный конечной папки для копируемые или перемещения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="0c103-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c103-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0c103-117">Parent elements</span></span>

|<span data-ttu-id="0c103-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c103-118">**Element**</span></span>|<span data-ttu-id="0c103-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c103-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c103-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="0c103-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="0c103-121">Определяет запрос на перемещение в папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c103-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="0c103-122">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0c103-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="0c103-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="0c103-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="0c103-124">Определяет запрос для копирования в папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c103-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="0c103-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0c103-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="0c103-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="0c103-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="0c103-127">Определяет запрос на перемещение элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c103-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="0c103-128">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0c103-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="0c103-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="0c103-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="0c103-130">Определяет запрос для копирования элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c103-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="0c103-131">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0c103-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0c103-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="0c103-132">Remarks</span></span>

<span data-ttu-id="0c103-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0c103-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c103-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0c103-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c103-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0c103-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0c103-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0c103-136">Schema Name</span></span>  <br/> |<span data-ttu-id="0c103-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0c103-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0c103-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0c103-138">Validation File</span></span>  <br/> |<span data-ttu-id="0c103-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0c103-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0c103-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0c103-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c103-141">False</span><span class="sxs-lookup"><span data-stu-id="0c103-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c103-142">См. также</span><span class="sxs-lookup"><span data-stu-id="0c103-142">See also</span></span>



[<span data-ttu-id="0c103-143">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="0c103-143">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="0c103-144">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="0c103-144">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="0c103-145">MoveItem Operation</span><span class="sxs-lookup"><span data-stu-id="0c103-145">MoveItem operation</span></span>](moveitem-operation.md)
  
[<span data-ttu-id="0c103-146">CopyItem Operation</span><span class="sxs-lookup"><span data-stu-id="0c103-146">CopyItem operation</span></span>](copyitem-operation.md)

