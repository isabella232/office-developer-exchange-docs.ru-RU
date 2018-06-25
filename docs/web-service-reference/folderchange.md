---
title: FolderChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChange
api_type:
- schema
ms.assetid: 23279750-131b-4e1a-b7d1-be235c4e0891
description: Элемент FolderChange представляет коллекцию изменений выполняется на одной папке.
ms.openlocfilehash: 3f8b42ff4ac88eaef53d1d4ec1d61212bc14b8c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762621"
---
# <a name="folderchange"></a><span data-ttu-id="c1c9b-103">FolderChange</span><span class="sxs-lookup"><span data-stu-id="c1c9b-103">FolderChange</span></span>

<span data-ttu-id="c1c9b-104">Элемент **FolderChange** представляет коллекцию изменений выполняется на одной папке.</span><span class="sxs-lookup"><span data-stu-id="c1c9b-104">The **FolderChange** element represents a collection of changes to be performed on a single folder.</span></span> 
  
[<span data-ttu-id="c1c9b-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="c1c9b-105">UpdateFolder</span></span>](updatefolder.md)
  
[<span data-ttu-id="c1c9b-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="c1c9b-106">FolderChanges</span></span>](folderchanges.md)
  
[<span data-ttu-id="c1c9b-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="c1c9b-107">FolderChange</span></span>](folderchange.md)
  
```xml
<FolderChange>
   <FolderId/>
   <Updates/>
</FolderChange>
```

 <span data-ttu-id="c1c9b-108">**FolderChangeType**</span><span class="sxs-lookup"><span data-stu-id="c1c9b-108">**FolderChangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1c9b-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c1c9b-109">Attributes and elements</span></span>

<span data-ttu-id="c1c9b-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c1c9b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1c9b-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c1c9b-111">Attributes</span></span>

<span data-ttu-id="c1c9b-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="c1c9b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1c9b-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c1c9b-113">Child elements</span></span>

|<span data-ttu-id="c1c9b-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1c9b-114">**Element**</span></span>|<span data-ttu-id="c1c9b-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1c9b-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1c9b-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="c1c9b-116">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="c1c9b-117">Содержит идентификатор и ключ изменения папки для обновления.</span><span class="sxs-lookup"><span data-stu-id="c1c9b-117">Contains the identifier and change key of a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="c1c9b-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c1c9b-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="c1c9b-119">Идентифицирует MicrosoftExchange Server 2007 папок, которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="c1c9b-119">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
|[<span data-ttu-id="c1c9b-120">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="c1c9b-120">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="c1c9b-121">Определяет тип обновления, который выполняется на папку, определяемую средством параметр [FolderId](folderid.md) или [DistinguishedFolderId](distinguishedfolderid.md) элемент.</span><span class="sxs-lookup"><span data-stu-id="c1c9b-121">Defines the type of update that is performed on a folder that is identified by either the [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1c9b-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c1c9b-122">Parent elements</span></span>

|<span data-ttu-id="c1c9b-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1c9b-123">**Element**</span></span>|<span data-ttu-id="c1c9b-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1c9b-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1c9b-125">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="c1c9b-125">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="c1c9b-126">Представляет коллекцию изменений для папки.</span><span class="sxs-lookup"><span data-stu-id="c1c9b-126">Represents a collection of changes for a folder.</span></span>  <br/> <span data-ttu-id="c1c9b-127">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="c1c9b-127">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c1c9b-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="c1c9b-128">Remarks</span></span>

<span data-ttu-id="c1c9b-129">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c1c9b-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1c9b-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c1c9b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1c9b-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c1c9b-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c1c9b-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c1c9b-132">Schema name</span></span>  <br/> |<span data-ttu-id="c1c9b-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c1c9b-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="c1c9b-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c1c9b-134">Validation file</span></span>  <br/> |<span data-ttu-id="c1c9b-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c1c9b-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c1c9b-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c1c9b-136">Can be empty</span></span>  <br/> |<span data-ttu-id="c1c9b-137">False</span><span class="sxs-lookup"><span data-stu-id="c1c9b-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1c9b-138">См. также</span><span class="sxs-lookup"><span data-stu-id="c1c9b-138">See also</span></span>



[<span data-ttu-id="c1c9b-139">Операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="c1c9b-139">UpdateFolder operation</span></span>](updatefolder-operation.md)

