---
title: Создание (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: 6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1
description: Создать элемент идентифицирует одной папке для создания в локальном хранилище клиента.
ms.openlocfilehash: 867eecb89c115b008d4828e162b21d078eba695c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761850"
---
# <a name="create-foldersync"></a><span data-ttu-id="1b9be-103">Создание (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="1b9be-103">Create (FolderSync)</span></span>

<span data-ttu-id="1b9be-104">**Создать** элемент идентифицирует одной папке для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="1b9be-104">The **Create** element identifies a single folder to create in the local client store.</span></span> 
  
[<span data-ttu-id="1b9be-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="1b9be-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="1b9be-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1b9be-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="1b9be-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1b9be-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="1b9be-108">Изменения (иерархии)</span><span class="sxs-lookup"><span data-stu-id="1b9be-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
[<span data-ttu-id="1b9be-109">Создание (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="1b9be-109">Create (FolderSync)</span></span>](create-foldersync.md)
  
```xml
<Create>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</Create>
```

 <span data-ttu-id="1b9be-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="1b9be-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b9be-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1b9be-111">Attributes and elements</span></span>

<span data-ttu-id="1b9be-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1b9be-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b9be-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1b9be-113">Attributes</span></span>

<span data-ttu-id="1b9be-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="1b9be-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b9be-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1b9be-115">Child elements</span></span>

|<span data-ttu-id="1b9be-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b9be-116">**Element**</span></span>|<span data-ttu-id="1b9be-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b9be-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b9be-118">Folder</span><span class="sxs-lookup"><span data-stu-id="1b9be-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="1b9be-119">Определяет папку для создания, получение, найти, синхронизировать или обновить.</span><span class="sxs-lookup"><span data-stu-id="1b9be-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="1b9be-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="1b9be-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="1b9be-121">Представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="1b9be-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="1b9be-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="1b9be-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="1b9be-123">Представляет папке контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="1b9be-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1b9be-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="1b9be-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="1b9be-125">Представляет папку поиска, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="1b9be-125">Represents a search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1b9be-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="1b9be-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="1b9be-127">Представляет папку задач, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="1b9be-127">Represents a task folder contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1b9be-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1b9be-128">Parent elements</span></span>

|<span data-ttu-id="1b9be-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b9be-129">**Element**</span></span>|<span data-ttu-id="1b9be-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b9be-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b9be-131">Изменения (иерархии)</span><span class="sxs-lookup"><span data-stu-id="1b9be-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="1b9be-132">Содержит массив последовательности типов изменений, которые представляют тип различия между элементами на стороне клиента и элементов на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b9be-132">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1b9be-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="1b9be-133">Remarks</span></span>

<span data-ttu-id="1b9be-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1b9be-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b9be-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1b9be-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b9be-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1b9be-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1b9be-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1b9be-137">Schema name</span></span>  <br/> |<span data-ttu-id="1b9be-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1b9be-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="1b9be-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1b9be-139">Validation file</span></span>  <br/> |<span data-ttu-id="1b9be-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1b9be-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1b9be-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1b9be-141">Can be empty</span></span>  <br/> |<span data-ttu-id="1b9be-142">False</span><span class="sxs-lookup"><span data-stu-id="1b9be-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b9be-143">См. также</span><span class="sxs-lookup"><span data-stu-id="1b9be-143">See also</span></span>



[<span data-ttu-id="1b9be-144">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="1b9be-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="1b9be-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1b9be-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

