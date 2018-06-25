---
title: Изменения (элементы)
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
ms.assetid: d3139fef-0455-4b89-babd-5d6783b50a58
description: Последовательность элемент изменения массивом типы изменений, которые представляют типы различия между элементами на стороне клиента и элементов на сервере Exchange.
ms.openlocfilehash: 8e38597276e3e3051a5c1494619d3220280e401f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761677"
---
# <a name="changes-items"></a><span data-ttu-id="57c31-103">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="57c31-103">Changes (Items)</span></span>

<span data-ttu-id="57c31-104">Последовательность элемент **изменения** массивом типы изменений, которые представляют типы различия между элементами на стороне клиента и элементов на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="57c31-104">The **Changes** element contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span> 
  
[<span data-ttu-id="57c31-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="57c31-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="57c31-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="57c31-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="57c31-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="57c31-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="57c31-108">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="57c31-108">Changes (Items)</span></span>](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="57c31-109">**SyncFolderItemsChangesType**</span><span class="sxs-lookup"><span data-stu-id="57c31-109">**SyncFolderItemsChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57c31-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="57c31-110">Attributes and elements</span></span>

<span data-ttu-id="57c31-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="57c31-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57c31-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="57c31-112">Attributes</span></span>

<span data-ttu-id="57c31-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="57c31-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57c31-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="57c31-114">Child elements</span></span>

|<span data-ttu-id="57c31-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57c31-115">**Element**</span></span>|<span data-ttu-id="57c31-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57c31-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57c31-117">Создание (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="57c31-117">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="57c31-118">Определяет один элемент для создания в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="57c31-118">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="57c31-119">Обновление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="57c31-119">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="57c31-120">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="57c31-120">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="57c31-121">Удаление (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="57c31-121">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="57c31-122">Определяет один элемент для удаления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="57c31-122">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="57c31-123">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="57c31-123">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="57c31-124">Возвращаются в [операции SyncFolderItems](syncfolderitems-operation.md) ответы прочтении элемента.</span><span class="sxs-lookup"><span data-stu-id="57c31-124">Returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="57c31-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57c31-125">This property is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57c31-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="57c31-126">Parent elements</span></span>

|<span data-ttu-id="57c31-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57c31-127">**Element**</span></span>|<span data-ttu-id="57c31-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57c31-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57c31-129">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="57c31-129">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="57c31-130">Содержит состояние и результат [операции SyncFolderItems](syncfolderitems-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="57c31-130">Contains the status and result of a [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="57c31-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="57c31-131">Remarks</span></span>

<span data-ttu-id="57c31-132">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="57c31-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57c31-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="57c31-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57c31-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="57c31-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57c31-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="57c31-135">Schema name</span></span>  <br/> |<span data-ttu-id="57c31-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="57c31-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57c31-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="57c31-137">Validation file</span></span>  <br/> |<span data-ttu-id="57c31-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="57c31-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57c31-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="57c31-139">Can be empty</span></span>  <br/> |<span data-ttu-id="57c31-140">False</span><span class="sxs-lookup"><span data-stu-id="57c31-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57c31-141">См. также</span><span class="sxs-lookup"><span data-stu-id="57c31-141">See also</span></span>



[<span data-ttu-id="57c31-142">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="57c31-142">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="57c31-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="57c31-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

