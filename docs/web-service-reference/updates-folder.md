---
title: Обновления (папка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: b047e3a4-a5ab-4098-b7a0-273bc809e702
description: Элемент Updates содержит набор элементов, которые определяют добавьте, Установка и удаление изменения свойств папки.
ms.openlocfilehash: 31f25b1e88fb8756f189a6d75259dd4fc198582f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840379"
---
# <a name="updates-folder"></a><span data-ttu-id="5c4d6-103">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="5c4d6-103">Updates (Folder)</span></span>

<span data-ttu-id="5c4d6-104">Элемент **Updates** содержит набор элементов, которые определяют добавьте, Установка и удаление изменения свойств папки.</span><span class="sxs-lookup"><span data-stu-id="5c4d6-104">The **Updates** element contains a set of elements that define append, set, and delete changes to folder properties.</span></span> 
  
- [<span data-ttu-id="5c4d6-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="5c4d6-105">UpdateFolder</span></span>](updatefolder.md)
  
- [<span data-ttu-id="5c4d6-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="5c4d6-106">FolderChanges</span></span>](folderchanges.md)
  
- [<span data-ttu-id="5c4d6-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="5c4d6-107">FolderChange</span></span>](folderchange.md)
  
- [<span data-ttu-id="5c4d6-108">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="5c4d6-108">Updates (Folder)</span></span>](updates-folder.md)
  
```xml
<Updates>
   <AppendToFolderField/>
   <SetFolderField/>
   <DeleteFolderField/>
</Updates>
```

<span data-ttu-id="5c4d6-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="5c4d6-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5c4d6-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5c4d6-110">Attributes and elements</span></span>

<span data-ttu-id="5c4d6-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5c4d6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c4d6-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5c4d6-112">Attributes</span></span>

<span data-ttu-id="5c4d6-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="5c4d6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c4d6-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5c4d6-114">Child elements</span></span>

|<span data-ttu-id="5c4d6-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5c4d6-115">**Element**</span></span>|<span data-ttu-id="5c4d6-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5c4d6-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c4d6-117">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="5c4d6-117">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="5c4d6-118">Представляет данные для добавления к папке свойство во время [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5c4d6-118">Represents data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="5c4d6-119">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="5c4d6-119">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="5c4d6-120">Представляет обновление для одного свойства папки в рамках одной [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5c4d6-120">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="5c4d6-121">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="5c4d6-121">DeleteFolderField</span></span>](deletefolderfield.md) <br/> |<span data-ttu-id="5c4d6-122">Представляет операцию удаление указанного свойства из папки при выполнении [операции UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5c4d6-122">Represents an operation to delete a given property from a folder during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c4d6-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5c4d6-123">Parent elements</span></span>

|<span data-ttu-id="5c4d6-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5c4d6-124">**Element**</span></span>|<span data-ttu-id="5c4d6-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5c4d6-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c4d6-126">FolderChange</span><span class="sxs-lookup"><span data-stu-id="5c4d6-126">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="5c4d6-127">Представляет коллекцию изменений выполняется на одной папке.</span><span class="sxs-lookup"><span data-stu-id="5c4d6-127">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="5c4d6-128">Ниже приведен выражение XPath для этого элемента.`/UpdateFolder/FolderChanges/FolderChange[i]`</span><span class="sxs-lookup"><span data-stu-id="5c4d6-128">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5c4d6-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="5c4d6-129">Remarks</span></span>

<span data-ttu-id="5c4d6-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5c4d6-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c4d6-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5c4d6-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c4d6-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5c4d6-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c4d6-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5c4d6-133">Schema Name</span></span>  <br/> |<span data-ttu-id="5c4d6-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5c4d6-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c4d6-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5c4d6-135">Validation File</span></span>  <br/> |<span data-ttu-id="5c4d6-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5c4d6-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c4d6-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5c4d6-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c4d6-138">False</span><span class="sxs-lookup"><span data-stu-id="5c4d6-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c4d6-139">См. также</span><span class="sxs-lookup"><span data-stu-id="5c4d6-139">See also</span></span>

- [<span data-ttu-id="5c4d6-140">Операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="5c4d6-140">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="5c4d6-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5c4d6-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

