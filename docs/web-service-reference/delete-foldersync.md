---
title: Delete (Фолдерсинк)
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
description: Элемент Delete определяет отдельную папку, которую необходимо удалить из локального хранилища клиентов.
ms.openlocfilehash: 68f8687b8cf0723d7fd63a3d55da8ef7c2f98f8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454983"
---
# <a name="delete-foldersync"></a><span data-ttu-id="44a68-103">Delete (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="44a68-103">Delete (FolderSync)</span></span>

<span data-ttu-id="44a68-104">Элемент **Delete** определяет отдельную папку, которую необходимо удалить из локального хранилища клиентов.</span><span class="sxs-lookup"><span data-stu-id="44a68-104">The **Delete** element identifies a single folder to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="44a68-105">синкфолдерхиерарчиреспонсе</span><span class="sxs-lookup"><span data-stu-id="44a68-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)  
- [<span data-ttu-id="44a68-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="44a68-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="44a68-107">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="44a68-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="44a68-108">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="44a68-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)  
- [<span data-ttu-id="44a68-109">Delete (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="44a68-109">Delete (FolderSync)</span></span>](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

<span data-ttu-id="44a68-110">**синкфолдерхиерарчиделететипе**</span><span class="sxs-lookup"><span data-stu-id="44a68-110">**SyncFolderHierarchyDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="44a68-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="44a68-111">Attributes and elements</span></span>

<span data-ttu-id="44a68-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="44a68-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44a68-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="44a68-113">Attributes</span></span>

<span data-ttu-id="44a68-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="44a68-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44a68-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="44a68-115">Child elements</span></span>

|<span data-ttu-id="44a68-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="44a68-116">**Element**</span></span>|<span data-ttu-id="44a68-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="44a68-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44a68-118">FolderId</span><span class="sxs-lookup"><span data-stu-id="44a68-118">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="44a68-119">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="44a68-119">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="44a68-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="44a68-120">Parent elements</span></span>

|<span data-ttu-id="44a68-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="44a68-121">**Element**</span></span>|<span data-ttu-id="44a68-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="44a68-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44a68-123">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="44a68-123">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="44a68-124">Содержит упорядоченный массив типов изменений, которые представляют тип различий между папками на клиенте и папками на компьютере, на котором работает Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="44a68-124">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="44a68-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="44a68-125">Remarks</span></span>

<span data-ttu-id="44a68-126">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера Exchange 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="44a68-126">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44a68-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="44a68-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44a68-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="44a68-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44a68-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="44a68-129">Schema name</span></span>  <br/> |<span data-ttu-id="44a68-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="44a68-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="44a68-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="44a68-131">Validation file</span></span>  <br/> |<span data-ttu-id="44a68-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="44a68-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="44a68-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="44a68-133">Can be empty</span></span>  <br/> |<span data-ttu-id="44a68-134">False</span><span class="sxs-lookup"><span data-stu-id="44a68-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44a68-135">См. также</span><span class="sxs-lookup"><span data-stu-id="44a68-135">See also</span></span>

- [<span data-ttu-id="44a68-136">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="44a68-136">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="44a68-137">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="44a68-137">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="44a68-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="44a68-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

