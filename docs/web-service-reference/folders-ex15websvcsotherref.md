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
ms.openlocfilehash: b087be0501f04390b80458458e7e7ccc24bf27bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530981"
---
# <a name="folders"></a><span data-ttu-id="a3273-103">Folders</span><span class="sxs-lookup"><span data-stu-id="a3273-103">Folders</span></span>

<span data-ttu-id="a3273-104">Элемент **Folders** содержит массив папок, которые используются в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="a3273-104">The **Folders** element contains an array of folders that are used in folder operations.</span></span> 
  
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

<span data-ttu-id="a3273-105">**Аррайоффолдерстипе** или **нонемптяррайоффолдерстипе**</span><span class="sxs-lookup"><span data-stu-id="a3273-105">**ArrayOfFoldersType** or **NonEmptyArrayOfFoldersType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a3273-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a3273-106">Attributes and elements</span></span>

<span data-ttu-id="a3273-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a3273-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3273-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a3273-108">Attributes</span></span>

<span data-ttu-id="a3273-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a3273-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3273-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a3273-110">Child elements</span></span>

|<span data-ttu-id="a3273-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a3273-111">**Element**</span></span>|<span data-ttu-id="a3273-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a3273-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3273-113">Folder</span><span class="sxs-lookup"><span data-stu-id="a3273-113">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="a3273-114">Определяет папку для создания, получения, поиска, синхронизации или обновления.</span><span class="sxs-lookup"><span data-stu-id="a3273-114">Identifies a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="a3273-115">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="a3273-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="a3273-116">Представляет папку, в которой в основном содержатся элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="a3273-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="a3273-117">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="a3273-117">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="a3273-118">Представляет папку "Контакты" в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a3273-118">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a3273-119">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="a3273-119">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="a3273-120">Представляет папку поиска, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a3273-120">Represents a Search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a3273-121">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="a3273-121">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="a3273-122">Представляет папку Tasks в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="a3273-122">Represents a Tasks folder in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3273-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a3273-123">Parent elements</span></span>

|<span data-ttu-id="a3273-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a3273-124">**Element**</span></span>|<span data-ttu-id="a3273-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a3273-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3273-126">копифолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a3273-126">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="a3273-127">Содержит состояние и результат одного запроса [операции CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a3273-127">Contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="a3273-128">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="a3273-128">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="a3273-129">Определяет запрос на создание папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3273-129">Defines a request to create a folder in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a3273-130">креатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a3273-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="a3273-131">Содержит состояние и результат одного запроса [операции CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a3273-131">Contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="a3273-132">креатеманажедфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a3273-132">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="a3273-133">Содержит состояние и результат одного запроса [операции CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a3273-133">Contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="a3273-134">жетфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a3273-134">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="a3273-135">Содержит состояние и результат запроса операции " [операция с папкой](getfolder-operation.md) ".</span><span class="sxs-lookup"><span data-stu-id="a3273-135">Contains the status and result of a [GetFolder operation](getfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="a3273-136">мовефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a3273-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="a3273-137">Содержит состояние и результат запроса [операции MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a3273-137">Contains the status and result of a [MoveFolder operation](movefolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="a3273-138">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="a3273-138">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="a3273-139">Определяет папку, в которой создается новая папка.</span><span class="sxs-lookup"><span data-stu-id="a3273-139">Identifies the folder where a new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="a3273-140">Рутфолдер (Финдфолдерреспонсемессаже)</span><span class="sxs-lookup"><span data-stu-id="a3273-140">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="a3273-141">Содержит результаты поиска в одной корневой папке во время [операции FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a3273-141">Contains the results from searching a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a3273-142">упдатефолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a3273-142">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="a3273-143">Содержит состояние и результат одного запроса [операции операцию UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a3273-143">Contains the status and result of a single [UpdateFolder operation](updatefolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a3273-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="a3273-144">Remarks</span></span>

<span data-ttu-id="a3273-145">Этот элемент является обязательным дочерним элементом элемента [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="a3273-145">This element is a required child element of the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span> 
  
<span data-ttu-id="a3273-146">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a3273-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3273-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a3273-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3273-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a3273-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a3273-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a3273-149">Schema Name</span></span>  <br/> |<span data-ttu-id="a3273-150">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a3273-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="a3273-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a3273-151">Validation File</span></span>  <br/> |<span data-ttu-id="a3273-152">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a3273-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a3273-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a3273-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3273-154">False</span><span class="sxs-lookup"><span data-stu-id="a3273-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3273-155">См. также</span><span class="sxs-lookup"><span data-stu-id="a3273-155">See also</span></span>

- [<span data-ttu-id="a3273-156">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="a3273-156">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)

