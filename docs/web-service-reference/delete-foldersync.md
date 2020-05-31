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
ms.openlocfilehash: 5cad36c6fcff782195fdb285e2d3c4f3c5ec0f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762015"
---
# <a name="delete-foldersync"></a><span data-ttu-id="6584c-103">Delete (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="6584c-103">Delete (FolderSync)</span></span>

<span data-ttu-id="6584c-104">Элемент **Delete** определяет отдельную папку, которую необходимо удалить из локального хранилища клиентов.</span><span class="sxs-lookup"><span data-stu-id="6584c-104">The **Delete** element identifies a single folder to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="6584c-105">синкфолдерхиерарчиреспонсе</span><span class="sxs-lookup"><span data-stu-id="6584c-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)  
- [<span data-ttu-id="6584c-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="6584c-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="6584c-107">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6584c-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="6584c-108">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="6584c-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)  
- [<span data-ttu-id="6584c-109">Delete (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="6584c-109">Delete (FolderSync)</span></span>](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

<span data-ttu-id="6584c-110">**синкфолдерхиерарчиделететипе**</span><span class="sxs-lookup"><span data-stu-id="6584c-110">**SyncFolderHierarchyDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6584c-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6584c-111">Attributes and elements</span></span>

<span data-ttu-id="6584c-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6584c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6584c-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6584c-113">Attributes</span></span>

<span data-ttu-id="6584c-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="6584c-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6584c-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6584c-115">Child elements</span></span>

|<span data-ttu-id="6584c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6584c-116">**Element**</span></span>|<span data-ttu-id="6584c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6584c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6584c-118">FolderId</span><span class="sxs-lookup"><span data-stu-id="6584c-118">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="6584c-119">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="6584c-119">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6584c-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6584c-120">Parent elements</span></span>

|<span data-ttu-id="6584c-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6584c-121">**Element**</span></span>|<span data-ttu-id="6584c-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6584c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6584c-123">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="6584c-123">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="6584c-124">Содержит упорядоченный массив типов изменений, которые представляют тип различий между папками на клиенте и папками на компьютере, на котором работает Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="6584c-124">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6584c-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="6584c-125">Remarks</span></span>

<span data-ttu-id="6584c-126">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера Exchange 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6584c-126">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6584c-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6584c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6584c-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6584c-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6584c-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6584c-129">Schema name</span></span>  <br/> |<span data-ttu-id="6584c-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6584c-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="6584c-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6584c-131">Validation file</span></span>  <br/> |<span data-ttu-id="6584c-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6584c-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6584c-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6584c-133">Can be empty</span></span>  <br/> |<span data-ttu-id="6584c-134">False</span><span class="sxs-lookup"><span data-stu-id="6584c-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6584c-135">См. также</span><span class="sxs-lookup"><span data-stu-id="6584c-135">See also</span></span>

- [<span data-ttu-id="6584c-136">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="6584c-136">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="6584c-137">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="6584c-137">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="6584c-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6584c-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

