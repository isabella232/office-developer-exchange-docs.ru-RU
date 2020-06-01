---
title: ParentFolderId (Таржетфолдеридтипе)
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
description: Элемент ParentFolderId определяет папку, в которой создается новая папка, или папку для поиска операции FindConversation.
ms.openlocfilehash: 36e63266d10603c4d453a37e2b0d22e02599e516
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467804"
---
# <a name="parentfolderid-targetfolderidtype"></a><span data-ttu-id="6db11-103">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="6db11-103">ParentFolderId (TargetFolderIdType)</span></span>

<span data-ttu-id="6db11-104">Элемент **ParentFolderId** определяет папку, в которой создается новая папка, или папку для поиска [операции FindConversation](findconversation-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6db11-104">The **ParentFolderId** element identifies the folder in which a new folder is created or the folder to search for the [FindConversation operation](findconversation-operation.md).</span></span>
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

```xml
<ParentFolderId>
   <FolderId/> 
</ParentFolderId>
```

<span data-ttu-id="6db11-105">**таржетфолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="6db11-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6db11-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6db11-106">Attributes and elements</span></span>

<span data-ttu-id="6db11-107">Элемент **ParentFolderId** содержит два дочерних элемента.</span><span class="sxs-lookup"><span data-stu-id="6db11-107">The **ParentFolderId** element contains two child elements.</span></span> <span data-ttu-id="6db11-108">Дочерние элементы в схеме являются взаимоисключающими.</span><span class="sxs-lookup"><span data-stu-id="6db11-108">The child elements are mutually exclusive in the schema.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="6db11-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6db11-109">Attributes</span></span>

<span data-ttu-id="6db11-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6db11-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6db11-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6db11-111">Child elements</span></span>

|<span data-ttu-id="6db11-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6db11-112">**Element**</span></span>|<span data-ttu-id="6db11-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6db11-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6db11-114">FolderId</span><span class="sxs-lookup"><span data-stu-id="6db11-114">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="6db11-115">Содержит обязательный идентификатор и необязательный ключ изменения папки, в которой создается новая папка, или папки, в которой выполняется поиск [операции FindConversation](findconversation-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6db11-115">Contains the required identifier and the optional change key of a folder in which a new folder is created or the folder that is searched for the [FindConversation operation](findconversation-operation.md).</span></span> <span data-ttu-id="6db11-116">Использование этого элемента исключает использование элемента [дистингуишедфолдерид](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="6db11-116">Using this element excludes the use of the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="6db11-117">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="6db11-117">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="6db11-118">Определяет стандартные папки Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="6db11-118">Identifies default Microsoft Exchange Server 2007 folders.</span></span> <span data-ttu-id="6db11-119">Использование этого элемента исключает использование элемента [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="6db11-119">Using this element excludes the use of the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6db11-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6db11-120">Parent elements</span></span>

|<span data-ttu-id="6db11-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6db11-121">**Element**</span></span>|<span data-ttu-id="6db11-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6db11-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6db11-123">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="6db11-123">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="6db11-124">Определяет запрос на создание папки в базе данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="6db11-124">Defines a request to create a folder in the Exchange database.</span></span>  <br/> <span data-ttu-id="6db11-125">Ниже приведено выражение XPath для этого элемента:`/CreateFolder`</span><span class="sxs-lookup"><span data-stu-id="6db11-125">The following is the XPath expression to this element:  `/CreateFolder`</span></span> <br/> |
|[<span data-ttu-id="6db11-126">FindConversation</span><span class="sxs-lookup"><span data-stu-id="6db11-126">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="6db11-127">Определяет запрос на поиск бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6db11-127">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6db11-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6db11-128">Text value</span></span>

<span data-ttu-id="6db11-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="6db11-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6db11-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="6db11-130">Remarks</span></span>

<span data-ttu-id="6db11-131">Два дочерних элемента используются для определения папки, которая будет содержать новую папку.</span><span class="sxs-lookup"><span data-stu-id="6db11-131">The two child elements are used to define the folder that will contain the new folder.</span></span> <span data-ttu-id="6db11-132">Чтобы определить родительскую папку для новой папки, необходимо выбрать элемент [FolderId](folderid.md) или [дистингуишедфолдерид](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="6db11-132">You must select either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element to identify the parent folder of the new folder.</span></span> <span data-ttu-id="6db11-133">Одновременное использование обоих элементов невозможно.</span><span class="sxs-lookup"><span data-stu-id="6db11-133">You cannot use both elements at the same time.</span></span> <span data-ttu-id="6db11-134">Этот элемент необходим для создания папок.</span><span class="sxs-lookup"><span data-stu-id="6db11-134">This element is required to create folders.</span></span> 
  
<span data-ttu-id="6db11-135">Элемент [ParentFolderId](parentfolderid.md) описывает расположение существующих элементов и папок.</span><span class="sxs-lookup"><span data-stu-id="6db11-135">The [ParentFolderId](parentfolderid.md) element describes the location of existing items and folders.</span></span> 
  
<span data-ttu-id="6db11-136">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6db11-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6db11-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6db11-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6db11-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6db11-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6db11-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6db11-139">Schema Name</span></span>  <br/> |<span data-ttu-id="6db11-140">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="6db11-140">Message schema</span></span>  <br/> |
|<span data-ttu-id="6db11-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6db11-141">Validation File</span></span>  <br/> |<span data-ttu-id="6db11-142">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6db11-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6db11-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6db11-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="6db11-144">False</span><span class="sxs-lookup"><span data-stu-id="6db11-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6db11-145">См. также</span><span class="sxs-lookup"><span data-stu-id="6db11-145">See also</span></span>

- [<span data-ttu-id="6db11-146">Операция CreateFolder</span><span class="sxs-lookup"><span data-stu-id="6db11-146">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="6db11-147">Операция FindConversation</span><span class="sxs-lookup"><span data-stu-id="6db11-147">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="6db11-148">Создание папок (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="6db11-148">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

