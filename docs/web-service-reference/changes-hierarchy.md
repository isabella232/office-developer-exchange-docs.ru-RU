---
title: Изменения (иерархии)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: Элемент изменения содержит виртуализированный массив типы изменений, которые представляют тип различия между папками на стороне клиента и папки на компьютере, на котором выполняется Microsoft Exchange Server 2007.
ms.openlocfilehash: 15e4f9f37c5e4a4083260dcf379a49beb2260030
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761681"
---
# <a name="changes-hierarchy"></a><span data-ttu-id="98c52-103">Изменения (иерархии)</span><span class="sxs-lookup"><span data-stu-id="98c52-103">Changes (Hierarchy)</span></span>

<span data-ttu-id="98c52-104">Элемент **изменения** содержит виртуализированный массив типы изменений, которые представляют тип различия между папками на стороне клиента и папки на компьютере, на котором выполняется Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="98c52-104">The **Changes** element contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="98c52-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="98c52-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="98c52-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="98c52-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="98c52-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="98c52-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="98c52-108">Изменения (иерархии)</span><span class="sxs-lookup"><span data-stu-id="98c52-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="98c52-109">**SyncFolderHierarchyChangesType**</span><span class="sxs-lookup"><span data-stu-id="98c52-109">**SyncFolderHierarchyChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98c52-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="98c52-110">Attributes and elements</span></span>

<span data-ttu-id="98c52-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="98c52-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98c52-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="98c52-112">Attributes</span></span>

<span data-ttu-id="98c52-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="98c52-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98c52-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="98c52-114">Child elements</span></span>

|<span data-ttu-id="98c52-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="98c52-115">**Element**</span></span>|<span data-ttu-id="98c52-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="98c52-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98c52-117">Создание (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="98c52-117">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="98c52-118">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="98c52-118">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="98c52-119">Обновление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="98c52-119">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="98c52-120">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="98c52-120">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="98c52-121">Удаление (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="98c52-121">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="98c52-122">Определяет одну папку для удаления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="98c52-122">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="98c52-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="98c52-123">Parent elements</span></span>

|<span data-ttu-id="98c52-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="98c52-124">**Element**</span></span>|<span data-ttu-id="98c52-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="98c52-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98c52-126">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="98c52-126">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="98c52-127">Содержит состояние и результат запроса SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="98c52-127">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98c52-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="98c52-128">Text value</span></span>

<span data-ttu-id="98c52-129">Текстовое значение, представляющее логическое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="98c52-129">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="98c52-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="98c52-130">Remarks</span></span>

<span data-ttu-id="98c52-131">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера Exchange 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="98c52-131">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98c52-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="98c52-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98c52-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="98c52-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="98c52-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="98c52-134">Schema name</span></span>  <br/> |<span data-ttu-id="98c52-135">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="98c52-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="98c52-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="98c52-136">Validation file</span></span>  <br/> |<span data-ttu-id="98c52-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="98c52-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="98c52-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="98c52-138">Can be empty</span></span>  <br/> |<span data-ttu-id="98c52-139">False</span><span class="sxs-lookup"><span data-stu-id="98c52-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98c52-140">См. также</span><span class="sxs-lookup"><span data-stu-id="98c52-140">See also</span></span>



[<span data-ttu-id="98c52-141">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="98c52-141">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


[<span data-ttu-id="98c52-142">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="98c52-142">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
  
- [<span data-ttu-id="98c52-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="98c52-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

