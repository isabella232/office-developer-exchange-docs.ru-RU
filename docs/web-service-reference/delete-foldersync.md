---
title: Удаление (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: c4397d91-43ef-40a9-a80e-d31501a33caa
description: Удалить элемент определяет одну папку для удаления в локальном хранилище клиента.
ms.openlocfilehash: 5cad36c6fcff782195fdb285e2d3c4f3c5ec0f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/21/2018
ms.locfileid: "19762015"
---
# <a name="delete-foldersync"></a><span data-ttu-id="bf159-103">Удаление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="bf159-103">Delete (FolderSync)</span></span>

<span data-ttu-id="bf159-104">**Удалить** элемент определяет одну папку для удаления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="bf159-104">The **Delete** element identifies a single folder to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="bf159-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="bf159-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)  
- [<span data-ttu-id="bf159-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bf159-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="bf159-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bf159-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="bf159-108">Изменения (иерархии)</span><span class="sxs-lookup"><span data-stu-id="bf159-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)  
- [<span data-ttu-id="bf159-109">Удаление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="bf159-109">Delete (FolderSync)</span></span>](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

<span data-ttu-id="bf159-110">**SyncFolderHierarchyDeleteType**</span><span class="sxs-lookup"><span data-stu-id="bf159-110">**SyncFolderHierarchyDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bf159-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bf159-111">Attributes and elements</span></span>

<span data-ttu-id="bf159-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bf159-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf159-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bf159-113">Attributes</span></span>

<span data-ttu-id="bf159-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="bf159-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf159-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bf159-115">Child elements</span></span>

|<span data-ttu-id="bf159-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bf159-116">**Element**</span></span>|<span data-ttu-id="bf159-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf159-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf159-118">FolderId</span><span class="sxs-lookup"><span data-stu-id="bf159-118">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="bf159-119">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="bf159-119">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bf159-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bf159-120">Parent elements</span></span>

|<span data-ttu-id="bf159-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bf159-121">**Element**</span></span>|<span data-ttu-id="bf159-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf159-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf159-123">Изменения (иерархии)</span><span class="sxs-lookup"><span data-stu-id="bf159-123">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="bf159-124">Содержит виртуализированный массив типов изменений, которые представляют тип различия между папками на стороне клиента и папки на компьютере, на котором выполняется Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="bf159-124">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bf159-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="bf159-125">Remarks</span></span>

<span data-ttu-id="bf159-126">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера Exchange 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bf159-126">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf159-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bf159-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf159-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bf159-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf159-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bf159-129">Schema name</span></span>  <br/> |<span data-ttu-id="bf159-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bf159-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="bf159-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bf159-131">Validation file</span></span>  <br/> |<span data-ttu-id="bf159-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bf159-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf159-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bf159-133">Can be empty</span></span>  <br/> |<span data-ttu-id="bf159-134">False</span><span class="sxs-lookup"><span data-stu-id="bf159-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf159-135">См. также</span><span class="sxs-lookup"><span data-stu-id="bf159-135">See also</span></span>

- [<span data-ttu-id="bf159-136">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="bf159-136">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="bf159-137">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="bf159-137">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="bf159-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bf159-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

