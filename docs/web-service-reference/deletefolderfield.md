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
ms.openlocfilehash: a0b48b667c8c8afbd5729d5deb84359a6a6ccc25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462159"
---
# <a name="deletefolderfield"></a><span data-ttu-id="1cba6-103">делетефолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="1cba6-103">DeleteFolderField</span></span>

<span data-ttu-id="1cba6-104">Элемент **делетефолдерфиелд** представляет операцию удаления определенного свойства из папки во время вызова операцию UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="1cba6-104">The **DeleteFolderField** element represents an operation to delete a given property from a folder during an UpdateFolder call.</span></span> 
  
- [<span data-ttu-id="1cba6-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="1cba6-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="1cba6-106">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="1cba6-106">FolderChanges</span></span>](folderchanges.md)  
- [<span data-ttu-id="1cba6-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="1cba6-107">FolderChange</span></span>](folderchange.md)  
- [<span data-ttu-id="1cba6-108">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="1cba6-108">Updates (Folder)</span></span>](updates-folder.md) 
- [<span data-ttu-id="1cba6-109">делетефолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="1cba6-109">DeleteFolderField</span></span>](deletefolderfield.md)
  
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

<span data-ttu-id="1cba6-110">**делетефолдерфиелдтипе**</span><span class="sxs-lookup"><span data-stu-id="1cba6-110">**DeleteFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1cba6-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1cba6-111">Attributes and elements</span></span>

<span data-ttu-id="1cba6-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1cba6-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cba6-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1cba6-113">Attributes</span></span>

<span data-ttu-id="1cba6-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1cba6-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cba6-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1cba6-115">Child elements</span></span>

|<span data-ttu-id="1cba6-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1cba6-116">**Element**</span></span>|<span data-ttu-id="1cba6-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1cba6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cba6-118">фиелдури</span><span class="sxs-lookup"><span data-stu-id="1cba6-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="1cba6-119">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="1cba6-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="1cba6-120">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="1cba6-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="1cba6-121">Определяет отдельные элементы свойства Dictionary.</span><span class="sxs-lookup"><span data-stu-id="1cba6-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="1cba6-122">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="1cba6-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="1cba6-123">Определяет расширенные свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="1cba6-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1cba6-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1cba6-124">Parent elements</span></span>

|<span data-ttu-id="1cba6-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1cba6-125">**Element**</span></span>|<span data-ttu-id="1cba6-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1cba6-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cba6-127">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="1cba6-127">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="1cba6-128">Содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств папки.</span><span class="sxs-lookup"><span data-stu-id="1cba6-128">Contains a set of elements that define append, set, and delete changes to folder properties.</span></span>  <br/> <span data-ttu-id="1cba6-129">Ниже приведено выражение XPath для этого элемента:`/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="1cba6-129">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1cba6-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="1cba6-130">Remarks</span></span>

<span data-ttu-id="1cba6-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1cba6-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cba6-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1cba6-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cba6-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1cba6-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1cba6-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1cba6-134">Schema Name</span></span>  <br/> |<span data-ttu-id="1cba6-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1cba6-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="1cba6-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1cba6-136">Validation File</span></span>  <br/> |<span data-ttu-id="1cba6-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1cba6-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1cba6-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1cba6-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cba6-139">False</span><span class="sxs-lookup"><span data-stu-id="1cba6-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cba6-140">См. также</span><span class="sxs-lookup"><span data-stu-id="1cba6-140">See also</span></span>

- [<span data-ttu-id="1cba6-141">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="1cba6-141">UpdateFolder operation</span></span>](updatefolder-operation.md)

