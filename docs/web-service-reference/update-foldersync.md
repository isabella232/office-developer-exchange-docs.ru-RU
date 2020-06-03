---
title: Обновление (Фолдерсинк)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 47ed8edb-2a94-471b-b965-93f91456252e
description: Элемент Update определяет одну папку для обновления в локальном хранилище клиента.
ms.openlocfilehash: 5c1b5b1fd87e4651125293eac431c56f732c6c02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467139"
---
# <a name="update-foldersync"></a><span data-ttu-id="76ae1-103">Обновление (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="76ae1-103">Update (FolderSync)</span></span>

<span data-ttu-id="76ae1-104">Элемент **Update** определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="76ae1-104">The **Update** element identifies a single folder to update in the local client store.</span></span> 
  
- [<span data-ttu-id="76ae1-105">синкфолдерхиерарчиреспонсе</span><span class="sxs-lookup"><span data-stu-id="76ae1-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="76ae1-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="76ae1-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="76ae1-107">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="76ae1-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="76ae1-108">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="76ae1-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md) 
- [<span data-ttu-id="76ae1-109">Обновление (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="76ae1-109">Update (FolderSync)</span></span>](update-foldersync.md)
  
```xml
<Update>
   <Folder/>
</Update>
```

```xml
<Update>
   <CalendarFolder/>
</Update>
```

```xml
<Update>
   <ContactsFolder/>
</Update>
```

```xml
<Update>
   <TasksFolder/>
</Update>
```

```xml
<Update>
   <SearchFolder/>
</Update>
```

<span data-ttu-id="76ae1-110">**синкфолдерхиерарчикреатеорупдатетипе**</span><span class="sxs-lookup"><span data-stu-id="76ae1-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="76ae1-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="76ae1-111">Attributes and elements</span></span>

<span data-ttu-id="76ae1-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="76ae1-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76ae1-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="76ae1-113">Attributes</span></span>

<span data-ttu-id="76ae1-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="76ae1-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76ae1-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="76ae1-115">Child elements</span></span>

|<span data-ttu-id="76ae1-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="76ae1-116">**Element**</span></span>|<span data-ttu-id="76ae1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="76ae1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76ae1-118">Folder</span><span class="sxs-lookup"><span data-stu-id="76ae1-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="76ae1-119">Определяет папку для создания, получения, поиска, синхронизации или обновления.</span><span class="sxs-lookup"><span data-stu-id="76ae1-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="76ae1-120">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="76ae1-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="76ae1-121">Представляет папку, в которой в основном содержатся элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="76ae1-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="76ae1-122">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="76ae1-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="76ae1-123">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="76ae1-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76ae1-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="76ae1-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="76ae1-125">Представляет папку поиска, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="76ae1-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="76ae1-126">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="76ae1-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="76ae1-127">Представляет папку задач "t" — сконтаинед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="76ae1-127">Represents a task folder t is thcontained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76ae1-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="76ae1-128">Parent elements</span></span>

|<span data-ttu-id="76ae1-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="76ae1-129">**Element**</span></span>|<span data-ttu-id="76ae1-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="76ae1-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76ae1-131">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="76ae1-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="76ae1-132">Содержит упорядоченный массив типов изменений, представляющий тип различий между папками на клиенте и папками на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="76ae1-132">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="76ae1-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="76ae1-133">Remarks</span></span>

<span data-ttu-id="76ae1-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="76ae1-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76ae1-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="76ae1-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76ae1-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="76ae1-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="76ae1-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="76ae1-137">Schema name</span></span>  <br/> |<span data-ttu-id="76ae1-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="76ae1-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="76ae1-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="76ae1-139">Validation file</span></span>  <br/> |<span data-ttu-id="76ae1-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="76ae1-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="76ae1-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="76ae1-141">Can be empty</span></span>  <br/> |<span data-ttu-id="76ae1-142">False</span><span class="sxs-lookup"><span data-stu-id="76ae1-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76ae1-143">См. также</span><span class="sxs-lookup"><span data-stu-id="76ae1-143">See also</span></span>

- [<span data-ttu-id="76ae1-144">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="76ae1-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="76ae1-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="76ae1-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

