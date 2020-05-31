---
title: делетефолдерфиелд
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderField
api_type:
- schema
ms.assetid: f9c2187b-4c60-4358-b4b4-ede50eadae48
description: Элемент Делетефолдерфиелд представляет операцию удаления определенного свойства из папки во время вызова операцию UpdateFolder.
ms.openlocfilehash: 60d4a5c19d89c109913e83fea99c2f7910566c72
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354094"
---
# <a name="deletefolderfield"></a><span data-ttu-id="d2a20-103">делетефолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="d2a20-103">DeleteFolderField</span></span>

<span data-ttu-id="d2a20-104">Элемент **делетефолдерфиелд** представляет операцию удаления определенного свойства из папки во время вызова операцию UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="d2a20-104">The **DeleteFolderField** element represents an operation to delete a given property from a folder during an UpdateFolder call.</span></span> 
  
- [<span data-ttu-id="d2a20-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="d2a20-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="d2a20-106">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="d2a20-106">FolderChanges</span></span>](folderchanges.md)  
- [<span data-ttu-id="d2a20-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="d2a20-107">FolderChange</span></span>](folderchange.md)  
- [<span data-ttu-id="d2a20-108">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="d2a20-108">Updates (Folder)</span></span>](updates-folder.md) 
- [<span data-ttu-id="d2a20-109">делетефолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="d2a20-109">DeleteFolderField</span></span>](deletefolderfield.md)
  
```xml
<DeleteFolderField>
   <FieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <ExtendedFieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <IndexedFieldURI/>
</DeleteFolderField>
```

<span data-ttu-id="d2a20-110">**делетефолдерфиелдтипе**</span><span class="sxs-lookup"><span data-stu-id="d2a20-110">**DeleteFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d2a20-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d2a20-111">Attributes and elements</span></span>

<span data-ttu-id="d2a20-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d2a20-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2a20-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d2a20-113">Attributes</span></span>

<span data-ttu-id="d2a20-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="d2a20-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2a20-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d2a20-115">Child elements</span></span>

|<span data-ttu-id="d2a20-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d2a20-116">**Element**</span></span>|<span data-ttu-id="d2a20-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d2a20-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2a20-118">фиелдури</span><span class="sxs-lookup"><span data-stu-id="d2a20-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="d2a20-119">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="d2a20-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="d2a20-120">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="d2a20-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="d2a20-121">Определяет отдельные элементы свойства Dictionary.</span><span class="sxs-lookup"><span data-stu-id="d2a20-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="d2a20-122">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="d2a20-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="d2a20-123">Определяет расширенные свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="d2a20-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2a20-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d2a20-124">Parent elements</span></span>

|<span data-ttu-id="d2a20-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d2a20-125">**Element**</span></span>|<span data-ttu-id="d2a20-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d2a20-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2a20-127">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="d2a20-127">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="d2a20-128">Содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств папки.</span><span class="sxs-lookup"><span data-stu-id="d2a20-128">Contains a set of elements that define append, set, and delete changes to folder properties.</span></span>  <br/> <span data-ttu-id="d2a20-129">Ниже приведено выражение XPath для этого элемента:`/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="d2a20-129">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2a20-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="d2a20-130">Remarks</span></span>

<span data-ttu-id="d2a20-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d2a20-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2a20-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d2a20-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2a20-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d2a20-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2a20-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d2a20-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d2a20-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d2a20-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="d2a20-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d2a20-136">Validation File</span></span>  <br/> |<span data-ttu-id="d2a20-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d2a20-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2a20-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d2a20-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2a20-139">False</span><span class="sxs-lookup"><span data-stu-id="d2a20-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2a20-140">См. также</span><span class="sxs-lookup"><span data-stu-id="d2a20-140">See also</span></span>

- [<span data-ttu-id="d2a20-141">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="d2a20-141">UpdateFolder operation</span></span>](updatefolder-operation.md)

