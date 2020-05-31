---
title: Папки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: Элемент Folders содержит массив папок, которые используются в операциях с папками.
ms.openlocfilehash: 34372f2480825c7a9977eeae8e730c201307f36b
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353590"
---
# <a name="folders"></a><span data-ttu-id="9b977-103">Folders</span><span class="sxs-lookup"><span data-stu-id="9b977-103">Folders</span></span>

<span data-ttu-id="9b977-104">Элемент **Folders** содержит массив папок, которые используются в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="9b977-104">The **Folders** element contains an array of folders that are used in folder operations.</span></span> 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

```xml
<Folders>
   <ContactsFolder/> 
</Folders>
```

```xml
<Folders>
   <TasksFolder/>
</Folders>
```

```xml
<Folders>
   <CalendarFolder/>
</Folders>
```

```xml
<Folders>
   <SearchFolder/> 
</Folders>
```

<span data-ttu-id="9b977-105">**Аррайоффолдерстипе** или **нонемптяррайоффолдерстипе**</span><span class="sxs-lookup"><span data-stu-id="9b977-105">**ArrayOfFoldersType** or **NonEmptyArrayOfFoldersType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9b977-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9b977-106">Attributes and elements</span></span>

<span data-ttu-id="9b977-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9b977-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b977-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9b977-108">Attributes</span></span>

<span data-ttu-id="9b977-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9b977-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b977-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9b977-110">Child elements</span></span>

|<span data-ttu-id="9b977-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b977-111">**Element**</span></span>|<span data-ttu-id="9b977-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b977-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b977-113">Folder</span><span class="sxs-lookup"><span data-stu-id="9b977-113">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="9b977-114">Определяет папку для создания, получения, поиска, синхронизации или обновления.</span><span class="sxs-lookup"><span data-stu-id="9b977-114">Identifies a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="9b977-115">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="9b977-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="9b977-116">Представляет папку, в которой в основном содержатся элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="9b977-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="9b977-117">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="9b977-117">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="9b977-118">Представляет папку "Контакты" в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9b977-118">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9b977-119">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="9b977-119">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="9b977-120">Представляет папку поиска, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9b977-120">Represents a Search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9b977-121">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="9b977-121">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="9b977-122">Представляет папку Tasks в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9b977-122">Represents a Tasks folder in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b977-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9b977-123">Parent elements</span></span>

|<span data-ttu-id="9b977-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b977-124">**Element**</span></span>|<span data-ttu-id="9b977-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b977-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b977-126">копифолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9b977-126">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="9b977-127">Содержит состояние и результат одного запроса [операции CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9b977-127">Contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9b977-128">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="9b977-128">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="9b977-129">Определяет запрос на создание папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b977-129">Defines a request to create a folder in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9b977-130">креатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9b977-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="9b977-131">Содержит состояние и результат одного запроса [операции CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9b977-131">Contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9b977-132">креатеманажедфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9b977-132">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="9b977-133">Содержит состояние и результат одного запроса [операции CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9b977-133">Contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9b977-134">жетфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9b977-134">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="9b977-135">Содержит состояние и результат запроса операции " [операция с папкой](getfolder-operation.md) ".</span><span class="sxs-lookup"><span data-stu-id="9b977-135">Contains the status and result of a [GetFolder operation](getfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9b977-136">мовефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9b977-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="9b977-137">Содержит состояние и результат запроса [операции MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9b977-137">Contains the status and result of a [MoveFolder operation](movefolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="9b977-138">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="9b977-138">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="9b977-139">Определяет папку, в которой создается новая папка.</span><span class="sxs-lookup"><span data-stu-id="9b977-139">Identifies the folder where a new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="9b977-140">Рутфолдер (Финдфолдерреспонсемессаже)</span><span class="sxs-lookup"><span data-stu-id="9b977-140">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="9b977-141">Содержит результаты поиска в одной корневой папке во время [операции FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9b977-141">Contains the results from searching a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="9b977-142">упдатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="9b977-142">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="9b977-143">Содержит состояние и результат одного запроса [операции операцию UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9b977-143">Contains the status and result of a single [UpdateFolder operation](updatefolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b977-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="9b977-144">Remarks</span></span>

<span data-ttu-id="9b977-145">Этот элемент является обязательным дочерним элементом элемента [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="9b977-145">This element is a required child element of the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span> 
  
<span data-ttu-id="9b977-146">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9b977-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b977-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9b977-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b977-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9b977-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b977-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9b977-149">Schema Name</span></span>  <br/> |<span data-ttu-id="9b977-150">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9b977-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b977-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9b977-151">Validation File</span></span>  <br/> |<span data-ttu-id="9b977-152">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9b977-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b977-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9b977-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b977-154">False</span><span class="sxs-lookup"><span data-stu-id="9b977-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b977-155">См. также</span><span class="sxs-lookup"><span data-stu-id="9b977-155">See also</span></span>

- [<span data-ttu-id="9b977-156">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="9b977-156">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)

