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
ms.openlocfilehash: 1919c335197c83999875a17397e9c9d4405d1e3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835407"
---
# <a name="setfolderfield"></a><span data-ttu-id="418ff-103">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="418ff-103">SetFolderField</span></span>

<span data-ttu-id="418ff-104">Элемент **SetFolderField** представляет обновление, которое задает значение для одного свойства для папки в рамках одной операции UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="418ff-104">The **SetFolderField** element represents an update that sets the value for a single property on a folder in an UpdateFolder operation.</span></span> 
  
```xml
<SetFolderField>
   <FieldURI/>
   <Folder/>
</SetFolderField>
```

 <span data-ttu-id="418ff-105">**SetFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="418ff-105">**SetFolderFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="418ff-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="418ff-106">Attributes and elements</span></span>

<span data-ttu-id="418ff-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="418ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="418ff-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="418ff-108">Attributes</span></span>

<span data-ttu-id="418ff-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="418ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="418ff-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="418ff-110">Child elements</span></span>

|<span data-ttu-id="418ff-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="418ff-111">**Element**</span></span>|<span data-ttu-id="418ff-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="418ff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="418ff-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="418ff-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="418ff-114">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="418ff-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="418ff-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="418ff-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="418ff-116">Идентифицирует отдельных элементов словаря.</span><span class="sxs-lookup"><span data-stu-id="418ff-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="418ff-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="418ff-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="418ff-118">Задает расширенные свойства MAPI.</span><span class="sxs-lookup"><span data-stu-id="418ff-118">Identifies extended MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="418ff-119">Folder</span><span class="sxs-lookup"><span data-stu-id="418ff-119">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="418ff-120">Определяет папку для обновления.</span><span class="sxs-lookup"><span data-stu-id="418ff-120">Identifies a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="418ff-121">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="418ff-121">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="418ff-122">Представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="418ff-122">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="418ff-123">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="418ff-123">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="418ff-124">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="418ff-124">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="418ff-125">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="418ff-125">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="418ff-126">Представляет папку поиска, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="418ff-126">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="418ff-127">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="418ff-127">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="418ff-128">Представляет папку задачи, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="418ff-128">Represents a Tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="418ff-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="418ff-129">Parent elements</span></span>

|<span data-ttu-id="418ff-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="418ff-130">**Element**</span></span>|<span data-ttu-id="418ff-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="418ff-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="418ff-132">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="418ff-132">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="418ff-133">Содержит набор элементов, определяющий добавьте, Установка и удаление изменения свойств папки.</span><span class="sxs-lookup"><span data-stu-id="418ff-133">Contains a set of elements that defines append, set, and delete changes to folder properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="418ff-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="418ff-134">Remarks</span></span>

<span data-ttu-id="418ff-135">Если свойство существует, значение свойства имеет значение до указанного значения.</span><span class="sxs-lookup"><span data-stu-id="418ff-135">If the property exists, the property value is set to the specified value.</span></span> <span data-ttu-id="418ff-136">Если свойство не существует, свойство будет создан с указанным значением.</span><span class="sxs-lookup"><span data-stu-id="418ff-136">If the property does not exist, the property is created with the specified value.</span></span>
  
<span data-ttu-id="418ff-137">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="418ff-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="418ff-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="418ff-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="418ff-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="418ff-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="418ff-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="418ff-140">Schema Name</span></span>  <br/> |<span data-ttu-id="418ff-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="418ff-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="418ff-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="418ff-142">Validation File</span></span>  <br/> |<span data-ttu-id="418ff-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="418ff-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="418ff-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="418ff-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="418ff-145">False</span><span class="sxs-lookup"><span data-stu-id="418ff-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="418ff-146">См. также</span><span class="sxs-lookup"><span data-stu-id="418ff-146">See also</span></span>



[<span data-ttu-id="418ff-147">Операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="418ff-147">UpdateFolder operation</span></span>](updatefolder-operation.md)


- [<span data-ttu-id="418ff-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="418ff-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

