---
title: сетфолдерфиелд
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
description: Элемент Сетфолдерфиелд представляет обновление, которое задает значение для одного свойства папки в операции операцию UpdateFolder.
ms.openlocfilehash: ed5c055c697865d5eb728d269c6f4c7ce60f4b5c
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353289"
---
# <a name="setfolderfield"></a><span data-ttu-id="f9451-103">сетфолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="f9451-103">SetFolderField</span></span>

<span data-ttu-id="f9451-104">Элемент **сетфолдерфиелд** представляет обновление, которое задает значение для одного свойства папки в операции операцию UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="f9451-104">The **SetFolderField** element represents an update that sets the value for a single property on a folder in an UpdateFolder operation.</span></span> 

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


<span data-ttu-id="f9451-105">**сетфолдерфиелдтипе**</span><span class="sxs-lookup"><span data-stu-id="f9451-105">**SetFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f9451-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f9451-106">Attributes and elements</span></span>

<span data-ttu-id="f9451-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f9451-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9451-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f9451-108">Attributes</span></span>

<span data-ttu-id="f9451-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f9451-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9451-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f9451-110">Child elements</span></span>

|<span data-ttu-id="f9451-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f9451-111">**Element**</span></span>|<span data-ttu-id="f9451-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f9451-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9451-113">фиелдури</span><span class="sxs-lookup"><span data-stu-id="f9451-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="f9451-114">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="f9451-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="f9451-115">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="f9451-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="f9451-116">Определяет отдельные элементы словаря.</span><span class="sxs-lookup"><span data-stu-id="f9451-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="f9451-117">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="f9451-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="f9451-118">Определяет расширенные свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="f9451-118">Identifies extended MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="f9451-119">Folder</span><span class="sxs-lookup"><span data-stu-id="f9451-119">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="f9451-120">Определяет папку, которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="f9451-120">Identifies a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="f9451-121">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="f9451-121">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="f9451-122">Представляет папку, в которой в основном содержатся элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="f9451-122">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="f9451-123">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="f9451-123">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="f9451-124">Представляет папку "Контакты" в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f9451-124">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f9451-125">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="f9451-125">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="f9451-126">Представляет папку поиска, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f9451-126">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f9451-127">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="f9451-127">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="f9451-128">Представляет папку Tasks, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f9451-128">Represents a Tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f9451-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f9451-129">Parent elements</span></span>

|<span data-ttu-id="f9451-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f9451-130">**Element**</span></span>|<span data-ttu-id="f9451-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f9451-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9451-132">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="f9451-132">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="f9451-133">Содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств папки.</span><span class="sxs-lookup"><span data-stu-id="f9451-133">Contains a set of elements that defines append, set, and delete changes to folder properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9451-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="f9451-134">Remarks</span></span>

<span data-ttu-id="f9451-135">Если свойство существует, значение свойства задается равным указанному значению.</span><span class="sxs-lookup"><span data-stu-id="f9451-135">If the property exists, the property value is set to the specified value.</span></span> <span data-ttu-id="f9451-136">Если свойство не существует, свойство создается с указанным значением.</span><span class="sxs-lookup"><span data-stu-id="f9451-136">If the property does not exist, the property is created with the specified value.</span></span>
  
<span data-ttu-id="f9451-137">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f9451-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9451-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f9451-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9451-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f9451-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9451-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f9451-140">Schema Name</span></span>  <br/> |<span data-ttu-id="f9451-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f9451-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9451-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f9451-142">Validation File</span></span>  <br/> |<span data-ttu-id="f9451-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f9451-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9451-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f9451-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9451-145">False</span><span class="sxs-lookup"><span data-stu-id="f9451-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9451-146">См. также</span><span class="sxs-lookup"><span data-stu-id="f9451-146">See also</span></span>

- [<span data-ttu-id="f9451-147">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="f9451-147">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="f9451-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f9451-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

