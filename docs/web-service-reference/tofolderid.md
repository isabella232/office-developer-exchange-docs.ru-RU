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
ms.openlocfilehash: 9d2fd6c177711cfe3a5d3415320440259e2f5289
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353660"
---
# <a name="tofolderid"></a><span data-ttu-id="93841-103">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="93841-103">ToFolderId</span></span>

<span data-ttu-id="93841-104">Элемент **ToFolderId** представляет конечной папки для копируемые или перемещения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="93841-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

```xml
<ToFolderId>
   <DistinguishedFolderId/>
</ToFolderId>
```

<span data-ttu-id="93841-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="93841-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="93841-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93841-106">Attributes and elements</span></span>

<span data-ttu-id="93841-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="93841-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93841-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93841-108">Attributes</span></span>

<span data-ttu-id="93841-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="93841-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93841-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93841-110">Child elements</span></span>

|<span data-ttu-id="93841-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93841-111">**Element**</span></span>|<span data-ttu-id="93841-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93841-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93841-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="93841-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="93841-114">Содержит идентификатор конечной папки для копируемые или перемещения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="93841-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="93841-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="93841-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="93841-116">Определяет именованный конечной папки для копируемые или перемещения элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="93841-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93841-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93841-117">Parent elements</span></span>

|<span data-ttu-id="93841-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93841-118">**Element**</span></span>|<span data-ttu-id="93841-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93841-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93841-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="93841-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="93841-121">Определяет запрос на перемещение в папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="93841-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="93841-122">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="93841-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="93841-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="93841-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="93841-124">Определяет запрос для копирования в папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="93841-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="93841-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="93841-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="93841-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="93841-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="93841-127">Определяет запрос на перемещение элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="93841-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="93841-128">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="93841-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="93841-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="93841-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="93841-130">Определяет запрос для копирования элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="93841-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="93841-131">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="93841-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93841-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="93841-132">Remarks</span></span>

<span data-ttu-id="93841-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="93841-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93841-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93841-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93841-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93841-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93841-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93841-136">Schema Name</span></span>  <br/> |<span data-ttu-id="93841-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="93841-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93841-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93841-138">Validation File</span></span>  <br/> |<span data-ttu-id="93841-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="93841-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93841-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93841-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="93841-141">False</span><span class="sxs-lookup"><span data-stu-id="93841-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93841-142">См. также</span><span class="sxs-lookup"><span data-stu-id="93841-142">See also</span></span>

- [<span data-ttu-id="93841-143">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="93841-143">MoveFolder operation</span></span>](movefolder-operation.md)  
- [<span data-ttu-id="93841-144">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="93841-144">CopyFolder operation</span></span>](copyfolder-operation.md) 
- [<span data-ttu-id="93841-145">Операция MoveItem</span><span class="sxs-lookup"><span data-stu-id="93841-145">MoveItem operation</span></span>](moveitem-operation.md) 
- [<span data-ttu-id="93841-146">Операция CopyItem</span><span class="sxs-lookup"><span data-stu-id="93841-146">CopyItem operation</span></span>](copyitem-operation.md)

