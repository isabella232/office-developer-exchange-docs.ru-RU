---
title: Create (Фолдерсинк)
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
description: Элемент create определяет одну папку для создания в локальном хранилище клиента.
ms.openlocfilehash: 43f6a6b3c084c8ecae767c512181bbdf50c7e786
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458378"
---
# <a name="create-foldersync"></a><span data-ttu-id="59dd0-103">Create (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="59dd0-103">Create (FolderSync)</span></span>

<span data-ttu-id="59dd0-104">Элемент **CREATE** определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="59dd0-104">The **Create** element identifies a single folder to create in the local client store.</span></span> 
  
[<span data-ttu-id="59dd0-105">синкфолдерхиерарчиреспонсе</span><span class="sxs-lookup"><span data-stu-id="59dd0-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="59dd0-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="59dd0-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="59dd0-107">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="59dd0-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="59dd0-108">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="59dd0-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
[<span data-ttu-id="59dd0-109">Create (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="59dd0-109">Create (FolderSync)</span></span>](create-foldersync.md)
  
```xml
<Create>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</Create>
```

 <span data-ttu-id="59dd0-110">**синкфолдерхиерарчикреатеорупдатетипе**</span><span class="sxs-lookup"><span data-stu-id="59dd0-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59dd0-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="59dd0-111">Attributes and elements</span></span>

<span data-ttu-id="59dd0-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="59dd0-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59dd0-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="59dd0-113">Attributes</span></span>

<span data-ttu-id="59dd0-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="59dd0-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59dd0-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="59dd0-115">Child elements</span></span>

|<span data-ttu-id="59dd0-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="59dd0-116">**Element**</span></span>|<span data-ttu-id="59dd0-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="59dd0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59dd0-118">Folder</span><span class="sxs-lookup"><span data-stu-id="59dd0-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="59dd0-119">Определяет папку для создания, получения, поиска, синхронизации или обновления.</span><span class="sxs-lookup"><span data-stu-id="59dd0-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="59dd0-120">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="59dd0-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="59dd0-121">Представляет папку, в которой в основном содержатся элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="59dd0-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="59dd0-122">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="59dd0-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="59dd0-123">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="59dd0-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="59dd0-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="59dd0-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="59dd0-125">Представляет папку поиска, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="59dd0-125">Represents a search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="59dd0-126">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="59dd0-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="59dd0-127">Представляет папку задач, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="59dd0-127">Represents a task folder contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59dd0-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="59dd0-128">Parent elements</span></span>

|<span data-ttu-id="59dd0-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="59dd0-129">**Element**</span></span>|<span data-ttu-id="59dd0-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="59dd0-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59dd0-131">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="59dd0-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="59dd0-132">Содержит массив последовательности типов изменений, представляющих тип различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="59dd0-132">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59dd0-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="59dd0-133">Remarks</span></span>

<span data-ttu-id="59dd0-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="59dd0-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59dd0-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="59dd0-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59dd0-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="59dd0-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59dd0-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="59dd0-137">Schema name</span></span>  <br/> |<span data-ttu-id="59dd0-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="59dd0-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="59dd0-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="59dd0-139">Validation file</span></span>  <br/> |<span data-ttu-id="59dd0-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="59dd0-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59dd0-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="59dd0-141">Can be empty</span></span>  <br/> |<span data-ttu-id="59dd0-142">False</span><span class="sxs-lookup"><span data-stu-id="59dd0-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59dd0-143">См. также</span><span class="sxs-lookup"><span data-stu-id="59dd0-143">See also</span></span>



[<span data-ttu-id="59dd0-144">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="59dd0-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="59dd0-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="59dd0-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

