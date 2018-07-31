---
title: SetFolderField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetFolderField
api_type:
- schema
ms.assetid: 8c69db7b-54b5-4ae2-abca-4d6e0937a790
description: Элемент SetFolderField представляет обновление, которое задает значение для одного свойства для папки в рамках одной операции UpdateFolder.
ms.openlocfilehash: ed5c055c697865d5eb728d269c6f4c7ce60f4b5c
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353289"
---
# <a name="setfolderfield"></a><span data-ttu-id="7e669-103">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="7e669-103">SetFolderField</span></span>

<span data-ttu-id="7e669-104">Элемент **SetFolderField** представляет обновление, которое задает значение для одного свойства для папки в рамках одной операции UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="7e669-104">The **SetFolderField** element represents an update that sets the value for a single property on a folder in an UpdateFolder operation.</span></span> 

```xml
<SetFolderField>
   <FieldURI/>
   <Folder/>
</SetFolderField>
```
  
```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <SearchFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <TasksFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <SearchFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <Folder/> 
</SetFolderField>
```

```xml
<SetFolderField>
    <IndexedFieldURI/> 
    <TasksFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <SearchFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <TasksFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <Folder/>
</SetFolderField>
```

```xml
<SetFolderField>
    <FieldURI/> 
    <ContactsFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <ContactsFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <ContactsFolder/> 
</SetFolderField>
```


<span data-ttu-id="7e669-105">**SetFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="7e669-105">**SetFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7e669-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7e669-106">Attributes and elements</span></span>

<span data-ttu-id="7e669-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7e669-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e669-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7e669-108">Attributes</span></span>

<span data-ttu-id="7e669-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7e669-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e669-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7e669-110">Child elements</span></span>

|<span data-ttu-id="7e669-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7e669-111">**Element**</span></span>|<span data-ttu-id="7e669-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e669-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e669-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="7e669-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="7e669-114">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="7e669-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="7e669-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="7e669-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="7e669-116">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="7e669-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="7e669-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="7e669-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="7e669-118">Задает расширенные свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="7e669-118">Identifies extended MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="7e669-119">Folder</span><span class="sxs-lookup"><span data-stu-id="7e669-119">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="7e669-120">Определяет папку для обновления.</span><span class="sxs-lookup"><span data-stu-id="7e669-120">Identifies a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="7e669-121">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="7e669-121">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="7e669-122">Представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="7e669-122">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="7e669-123">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="7e669-123">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="7e669-124">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="7e669-124">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7e669-125">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="7e669-125">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="7e669-126">Представляет папку поиска, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="7e669-126">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7e669-127">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="7e669-127">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="7e669-128">Представляет папку задачи, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="7e669-128">Represents a Tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e669-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7e669-129">Parent elements</span></span>

|<span data-ttu-id="7e669-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7e669-130">**Element**</span></span>|<span data-ttu-id="7e669-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e669-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e669-132">Updates (Folder)</span><span class="sxs-lookup"><span data-stu-id="7e669-132">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="7e669-133">Содержит набор элементов, определяющий добавьте, Установка и удаление изменения свойств папки.</span><span class="sxs-lookup"><span data-stu-id="7e669-133">Contains a set of elements that defines append, set, and delete changes to folder properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e669-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="7e669-134">Remarks</span></span>

<span data-ttu-id="7e669-135">Если свойство существует, значение свойства имеет значение до указанного значения.</span><span class="sxs-lookup"><span data-stu-id="7e669-135">If the property exists, the property value is set to the specified value.</span></span> <span data-ttu-id="7e669-136">Если свойство не существует, свойство будет создан с указанным значением.</span><span class="sxs-lookup"><span data-stu-id="7e669-136">If the property does not exist, the property is created with the specified value.</span></span>
  
<span data-ttu-id="7e669-137">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7e669-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e669-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7e669-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e669-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7e669-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e669-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7e669-140">Schema Name</span></span>  <br/> |<span data-ttu-id="7e669-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7e669-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e669-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7e669-142">Validation File</span></span>  <br/> |<span data-ttu-id="7e669-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e669-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e669-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7e669-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e669-145">False</span><span class="sxs-lookup"><span data-stu-id="7e669-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e669-146">См. также</span><span class="sxs-lookup"><span data-stu-id="7e669-146">See also</span></span>

- [<span data-ttu-id="7e669-147">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="7e669-147">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="7e669-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7e669-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

