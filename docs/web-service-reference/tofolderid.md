---
title: тофолдерид
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
description: Элемент Тофолдерид представляет папку назначения для скопированного или перемещенного элемента или папки.
ms.openlocfilehash: 9d2fd6c177711cfe3a5d3415320440259e2f5289
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353660"
---
# <a name="tofolderid"></a><span data-ttu-id="15ea0-103">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="15ea0-103">ToFolderId</span></span>

<span data-ttu-id="15ea0-104">Элемент **тофолдерид** представляет папку назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="15ea0-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
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

<span data-ttu-id="15ea0-105">**таржетфолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="15ea0-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="15ea0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="15ea0-106">Attributes and elements</span></span>

<span data-ttu-id="15ea0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="15ea0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15ea0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="15ea0-108">Attributes</span></span>

<span data-ttu-id="15ea0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="15ea0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15ea0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="15ea0-110">Child elements</span></span>

|<span data-ttu-id="15ea0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="15ea0-111">**Element**</span></span>|<span data-ttu-id="15ea0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15ea0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15ea0-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="15ea0-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="15ea0-114">Содержит идентификатор папки назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="15ea0-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="15ea0-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="15ea0-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="15ea0-116">Определяет именованную папку назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="15ea0-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="15ea0-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="15ea0-117">Parent elements</span></span>

|<span data-ttu-id="15ea0-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="15ea0-118">**Element**</span></span>|<span data-ttu-id="15ea0-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15ea0-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15ea0-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="15ea0-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="15ea0-121">Определяет запрос на перемещение папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="15ea0-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="15ea0-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="15ea0-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="15ea0-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="15ea0-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="15ea0-124">Определяет запрос на копирование папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="15ea0-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="15ea0-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="15ea0-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="15ea0-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="15ea0-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="15ea0-127">Определяет запрос на перемещение элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="15ea0-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="15ea0-128">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="15ea0-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="15ea0-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="15ea0-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="15ea0-130">Определяет запрос на копирование элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="15ea0-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="15ea0-131">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="15ea0-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="15ea0-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="15ea0-132">Remarks</span></span>

<span data-ttu-id="15ea0-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="15ea0-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15ea0-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="15ea0-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15ea0-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="15ea0-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="15ea0-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="15ea0-136">Schema Name</span></span>  <br/> |<span data-ttu-id="15ea0-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="15ea0-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="15ea0-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="15ea0-138">Validation File</span></span>  <br/> |<span data-ttu-id="15ea0-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="15ea0-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="15ea0-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="15ea0-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="15ea0-141">False</span><span class="sxs-lookup"><span data-stu-id="15ea0-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15ea0-142">См. также</span><span class="sxs-lookup"><span data-stu-id="15ea0-142">See also</span></span>

- [<span data-ttu-id="15ea0-143">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="15ea0-143">MoveFolder operation</span></span>](movefolder-operation.md)  
- [<span data-ttu-id="15ea0-144">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="15ea0-144">CopyFolder operation</span></span>](copyfolder-operation.md) 
- [<span data-ttu-id="15ea0-145">Операция MoveItem</span><span class="sxs-lookup"><span data-stu-id="15ea0-145">MoveItem operation</span></span>](moveitem-operation.md) 
- [<span data-ttu-id="15ea0-146">Операция CopyItem</span><span class="sxs-lookup"><span data-stu-id="15ea0-146">CopyItem operation</span></span>](copyitem-operation.md)

