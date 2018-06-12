---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: Элемент ParentFolderId определяет папку, в которой будет создана новая папка или папки для поиска FindConversation операции.
ms.openlocfilehash: 61072e1dd3321beb5f3b76d9accf20530b443796
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834686"
---
# <a name="parentfolderid-targetfolderidtype"></a><span data-ttu-id="d67d3-103">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="d67d3-103">ParentFolderId (TargetFolderIdType)</span></span>

<span data-ttu-id="d67d3-104">Элемент **ParentFolderId** определяет папку, в которой будет создана новая папка или папки для поиска [FindConversation операции](findconversation-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d67d3-104">The **ParentFolderId** element identifies the folder in which a new folder is created or the folder to search for the [FindConversation operation](findconversation-operation.md).</span></span>
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

<span data-ttu-id="d67d3-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="d67d3-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d67d3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d67d3-106">Attributes and elements</span></span>

<span data-ttu-id="d67d3-107">Элемент **ParentFolderId** содержит два дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="d67d3-107">The **ParentFolderId** element contains two child elements.</span></span> <span data-ttu-id="d67d3-108">Дочерние элементы являются взаимоисключающими в схеме.</span><span class="sxs-lookup"><span data-stu-id="d67d3-108">The child elements are mutually exclusive in the schema.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="d67d3-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d67d3-109">Attributes</span></span>

<span data-ttu-id="d67d3-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="d67d3-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d67d3-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d67d3-111">Child elements</span></span>

|<span data-ttu-id="d67d3-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d67d3-112">**Element**</span></span>|<span data-ttu-id="d67d3-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d67d3-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d67d3-114">FolderId</span><span class="sxs-lookup"><span data-stu-id="d67d3-114">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d67d3-115">Содержит обязательного элемента identifier и ключ необязательно изменения папки, в которой будет создана новая папка или к папке, где выполняется поиск [FindConversation операции](findconversation-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d67d3-115">Contains the required identifier and the optional change key of a folder in which a new folder is created or the folder that is searched for the [FindConversation operation](findconversation-operation.md).</span></span> <span data-ttu-id="d67d3-116">С помощью этого элемента исключает использование элемента [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="d67d3-116">Using this element excludes the use of the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="d67d3-117">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="d67d3-117">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="d67d3-118">Идентифицирует папок Microsoft Exchange Server 2007 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d67d3-118">Identifies default Microsoft Exchange Server 2007 folders.</span></span> <span data-ttu-id="d67d3-119">С помощью этого элемента исключает использование элемента [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="d67d3-119">Using this element excludes the use of the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d67d3-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d67d3-120">Parent elements</span></span>

|<span data-ttu-id="d67d3-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d67d3-121">**Element**</span></span>|<span data-ttu-id="d67d3-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d67d3-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d67d3-123">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="d67d3-123">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="d67d3-124">Определяет запрос на создание папки в базе данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="d67d3-124">Defines a request to create a folder in the Exchange database.</span></span>  <br/> <span data-ttu-id="d67d3-125">Ниже приведен выражение XPath для этого элемента.`/CreateFolder`</span><span class="sxs-lookup"><span data-stu-id="d67d3-125">The following is the XPath expression to this element:  `/CreateFolder`</span></span> <br/> |
|[<span data-ttu-id="d67d3-126">FindConversation</span><span class="sxs-lookup"><span data-stu-id="d67d3-126">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="d67d3-127">Определяет запрос на поиск бесед в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="d67d3-127">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d67d3-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d67d3-128">Text value</span></span>

<span data-ttu-id="d67d3-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="d67d3-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d67d3-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="d67d3-130">Remarks</span></span>

<span data-ttu-id="d67d3-131">Два дочерние элементы используются для определения папки, которая будет содержать новую папку.</span><span class="sxs-lookup"><span data-stu-id="d67d3-131">The two child elements are used to define the folder that will contain the new folder.</span></span> <span data-ttu-id="d67d3-132">Необходимо выбрать [FolderId](folderid.md) или элемент [DistinguishedFolderId](distinguishedfolderid.md) для определения родительской папки новую папку.</span><span class="sxs-lookup"><span data-stu-id="d67d3-132">You must select either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element to identify the parent folder of the new folder.</span></span> <span data-ttu-id="d67d3-133">Нельзя использовать оба этих элемента в то же время.</span><span class="sxs-lookup"><span data-stu-id="d67d3-133">You cannot use both elements at the same time.</span></span> <span data-ttu-id="d67d3-134">Этот элемент необходим для создания папки.</span><span class="sxs-lookup"><span data-stu-id="d67d3-134">This element is required to create folders.</span></span> 
  
<span data-ttu-id="d67d3-135">Элемент [ParentFolderId](parentfolderid.md) описывает расположение существующих элементов и папок.</span><span class="sxs-lookup"><span data-stu-id="d67d3-135">The [ParentFolderId](parentfolderid.md) element describes the location of existing items and folders.</span></span> 
  
<span data-ttu-id="d67d3-136">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d67d3-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d67d3-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d67d3-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d67d3-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d67d3-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d67d3-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d67d3-139">Schema Name</span></span>  <br/> |<span data-ttu-id="d67d3-140">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="d67d3-140">Message schema</span></span>  <br/> |
|<span data-ttu-id="d67d3-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d67d3-141">Validation File</span></span>  <br/> |<span data-ttu-id="d67d3-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d67d3-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d67d3-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d67d3-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="d67d3-144">False</span><span class="sxs-lookup"><span data-stu-id="d67d3-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d67d3-145">См. также</span><span class="sxs-lookup"><span data-stu-id="d67d3-145">See also</span></span>

- [<span data-ttu-id="d67d3-146">CreateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="d67d3-146">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="d67d3-147">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="d67d3-147">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="d67d3-148">Создание папки (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="d67d3-148">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

