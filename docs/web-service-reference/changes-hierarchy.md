---
title: Изменения (иерархия)
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
description: Элемент Changes содержит упорядоченный массив типов изменений, представляющий тип различий между папками на клиенте и папками на компьютере, на котором работает Microsoft Exchange Server 2007.
ms.openlocfilehash: a296d87f23e85d42b4c8c858e92eddfb586a8324
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463274"
---
# <a name="changes-hierarchy"></a><span data-ttu-id="f05f1-103">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="f05f1-103">Changes (Hierarchy)</span></span>

<span data-ttu-id="f05f1-104">Элемент **Changes** содержит упорядоченный массив типов изменений, представляющий тип различий между папками на клиенте и папками на компьютере, на котором работает Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="f05f1-104">The **Changes** element contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="f05f1-105">синкфолдерхиерарчиреспонсе</span><span class="sxs-lookup"><span data-stu-id="f05f1-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="f05f1-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f05f1-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="f05f1-107">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f05f1-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="f05f1-108">Изменения (иерархия)</span><span class="sxs-lookup"><span data-stu-id="f05f1-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="f05f1-109">**синкфолдерхиерарчичанжестипе**</span><span class="sxs-lookup"><span data-stu-id="f05f1-109">**SyncFolderHierarchyChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f05f1-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f05f1-110">Attributes and elements</span></span>

<span data-ttu-id="f05f1-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f05f1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f05f1-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f05f1-112">Attributes</span></span>

<span data-ttu-id="f05f1-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f05f1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f05f1-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f05f1-114">Child elements</span></span>

|<span data-ttu-id="f05f1-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f05f1-115">**Element**</span></span>|<span data-ttu-id="f05f1-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f05f1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f05f1-117">Create (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="f05f1-117">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="f05f1-118">Определяет одну папку для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="f05f1-118">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="f05f1-119">Обновление (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="f05f1-119">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="f05f1-120">Определяет одну папку для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="f05f1-120">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="f05f1-121">Delete (Фолдерсинк)</span><span class="sxs-lookup"><span data-stu-id="f05f1-121">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="f05f1-122">Определяет одну папку для удаления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="f05f1-122">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f05f1-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f05f1-123">Parent elements</span></span>

|<span data-ttu-id="f05f1-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f05f1-124">**Element**</span></span>|<span data-ttu-id="f05f1-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f05f1-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f05f1-126">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f05f1-126">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="f05f1-127">Содержит состояние и результат запроса SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="f05f1-127">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f05f1-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f05f1-128">Text value</span></span>

<span data-ttu-id="f05f1-129">Текстовое значение, представляющее логическое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="f05f1-129">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f05f1-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="f05f1-130">Remarks</span></span>

<span data-ttu-id="f05f1-131">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера Exchange 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f05f1-131">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f05f1-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f05f1-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f05f1-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f05f1-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f05f1-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f05f1-134">Schema name</span></span>  <br/> |<span data-ttu-id="f05f1-135">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f05f1-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f05f1-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f05f1-136">Validation file</span></span>  <br/> |<span data-ttu-id="f05f1-137">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f05f1-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f05f1-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f05f1-138">Can be empty</span></span>  <br/> |<span data-ttu-id="f05f1-139">False</span><span class="sxs-lookup"><span data-stu-id="f05f1-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f05f1-140">См. также</span><span class="sxs-lookup"><span data-stu-id="f05f1-140">See also</span></span>



[<span data-ttu-id="f05f1-141">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="f05f1-141">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


[<span data-ttu-id="f05f1-142">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="f05f1-142">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
  
- [<span data-ttu-id="f05f1-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f05f1-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

