---
title: Обновление (FolderSync)
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
description: Элемент обновления определяет одну папку для обновления в локальном хранилище клиента.
ms.openlocfilehash: 6d4a6233df41ea95e1fd9b394502bfb2728bddb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840313"
---
# <a name="update-foldersync"></a><span data-ttu-id="bafe4-103">Обновление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="bafe4-103">Update (FolderSync)</span></span>

<span data-ttu-id="bafe4-104">**Обновить** элемент определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="bafe4-104">The **Update** element identifies a single folder to update in the local client store.</span></span> 
  
[<span data-ttu-id="bafe4-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="bafe4-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="bafe4-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bafe4-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="bafe4-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bafe4-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="bafe4-108">Изменения (иерархии)</span><span class="sxs-lookup"><span data-stu-id="bafe4-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
[<span data-ttu-id="bafe4-109">Обновление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="bafe4-109">Update (FolderSync)</span></span>](update-foldersync.md)
  
```xml
<Update>
   <Folder/>
</Update>
```

 <span data-ttu-id="bafe4-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="bafe4-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bafe4-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bafe4-111">Attributes and elements</span></span>

<span data-ttu-id="bafe4-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bafe4-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bafe4-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bafe4-113">Attributes</span></span>

<span data-ttu-id="bafe4-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="bafe4-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bafe4-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bafe4-115">Child elements</span></span>

|<span data-ttu-id="bafe4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bafe4-116">**Element**</span></span>|<span data-ttu-id="bafe4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bafe4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bafe4-118">Folder</span><span class="sxs-lookup"><span data-stu-id="bafe4-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="bafe4-119">Определяет папку для создания, получение, найти, синхронизировать или обновить.</span><span class="sxs-lookup"><span data-stu-id="bafe4-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="bafe4-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="bafe4-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="bafe4-121">Представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="bafe4-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="bafe4-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="bafe4-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="bafe4-123">Представляет папке контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bafe4-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bafe4-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="bafe4-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="bafe4-125">Представляет папку поиска, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bafe4-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bafe4-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="bafe4-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="bafe4-127">Представляет задачу папки t — это thcontained в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bafe4-127">Represents a task folder t is thcontained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bafe4-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bafe4-128">Parent elements</span></span>

|<span data-ttu-id="bafe4-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bafe4-129">**Element**</span></span>|<span data-ttu-id="bafe4-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bafe4-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bafe4-131">Изменения (иерархии)</span><span class="sxs-lookup"><span data-stu-id="bafe4-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="bafe4-132">Содержит виртуализированный массив типов изменений, которые представляют тип различия между папками на стороне клиента и папки на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="bafe4-132">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bafe4-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="bafe4-133">Remarks</span></span>

<span data-ttu-id="bafe4-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bafe4-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bafe4-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bafe4-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bafe4-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bafe4-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bafe4-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bafe4-137">Schema name</span></span>  <br/> |<span data-ttu-id="bafe4-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bafe4-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="bafe4-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bafe4-139">Validation file</span></span>  <br/> |<span data-ttu-id="bafe4-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bafe4-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bafe4-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bafe4-141">Can be empty</span></span>  <br/> |<span data-ttu-id="bafe4-142">False</span><span class="sxs-lookup"><span data-stu-id="bafe4-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bafe4-143">См. также</span><span class="sxs-lookup"><span data-stu-id="bafe4-143">See also</span></span>



[<span data-ttu-id="bafe4-144">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="bafe4-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="bafe4-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bafe4-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

