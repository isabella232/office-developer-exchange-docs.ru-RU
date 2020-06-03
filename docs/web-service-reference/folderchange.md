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
description: Элемент Фолдерчанже представляет коллекцию изменений, которые необходимо выполнить для одной папки.
ms.openlocfilehash: e4a025bef100fdd478be545b6448b15886e47c60
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530241"
---
# <a name="folderchange"></a><span data-ttu-id="d6425-103">FolderChange</span><span class="sxs-lookup"><span data-stu-id="d6425-103">FolderChange</span></span>

<span data-ttu-id="d6425-104">Элемент **фолдерчанже** представляет коллекцию изменений, которые необходимо выполнить для одной папки.</span><span class="sxs-lookup"><span data-stu-id="d6425-104">The **FolderChange** element represents a collection of changes to be performed on a single folder.</span></span> 
  
- [<span data-ttu-id="d6425-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="d6425-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="d6425-106">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="d6425-106">FolderChanges</span></span>](folderchanges.md) 
- [<span data-ttu-id="d6425-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="d6425-107">FolderChange</span></span>](folderchange.md)
  
```xml
<FolderChange>
   <FolderId/>
   <Updates/>
</FolderChange>
```

```xml
<FolderChange>
   <DistinguishedFolderId/>
   <Updates/>
</FolderChange>
```

<span data-ttu-id="d6425-108">**фолдерчанжетипе**</span><span class="sxs-lookup"><span data-stu-id="d6425-108">**FolderChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d6425-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d6425-109">Attributes and elements</span></span>

<span data-ttu-id="d6425-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d6425-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6425-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d6425-111">Attributes</span></span>

<span data-ttu-id="d6425-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d6425-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6425-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d6425-113">Child elements</span></span>

|<span data-ttu-id="d6425-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d6425-114">**Element**</span></span>|<span data-ttu-id="d6425-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6425-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6425-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="d6425-116">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d6425-117">Содержит идентификатор и ключ изменения папки, которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="d6425-117">Contains the identifier and change key of a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="d6425-118">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="d6425-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="d6425-119">Определяет Майкрософт Exchange Server 2007 папок, на которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="d6425-119">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
|[<span data-ttu-id="d6425-120">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="d6425-120">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="d6425-121">Определяет тип обновления, выполняемого для папки, которая идентифицируется с помощью элемента [FolderId](folderid.md) или [дистингуишедфолдерид](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="d6425-121">Defines the type of update that is performed on a folder that is identified by either the [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6425-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d6425-122">Parent elements</span></span>

|<span data-ttu-id="d6425-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d6425-123">**Element**</span></span>|<span data-ttu-id="d6425-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6425-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6425-125">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="d6425-125">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="d6425-126">Представляет коллекцию изменений для папки.</span><span class="sxs-lookup"><span data-stu-id="d6425-126">Represents a collection of changes for a folder.</span></span>  <br/> <span data-ttu-id="d6425-127">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="d6425-127">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d6425-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="d6425-128">Remarks</span></span>

<span data-ttu-id="d6425-129">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server 2007 с ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d6425-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6425-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d6425-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6425-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d6425-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6425-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d6425-132">Schema name</span></span>  <br/> |<span data-ttu-id="d6425-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d6425-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d6425-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d6425-134">Validation file</span></span>  <br/> |<span data-ttu-id="d6425-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d6425-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6425-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d6425-136">Can be empty</span></span>  <br/> |<span data-ttu-id="d6425-137">False</span><span class="sxs-lookup"><span data-stu-id="d6425-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6425-138">См. также</span><span class="sxs-lookup"><span data-stu-id="d6425-138">See also</span></span>

- [<span data-ttu-id="d6425-139">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="d6425-139">UpdateFolder operation</span></span>](updatefolder-operation.md)

