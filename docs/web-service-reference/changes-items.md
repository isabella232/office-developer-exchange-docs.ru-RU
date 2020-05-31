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
description: Элемент Changes содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange.
ms.openlocfilehash: 8e38597276e3e3051a5c1494619d3220280e401f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761677"
---
# <a name="changes-items"></a><span data-ttu-id="68a45-103">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="68a45-103">Changes (Items)</span></span>

<span data-ttu-id="68a45-104">Элемент **Changes** содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="68a45-104">The **Changes** element contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span> 
  
[<span data-ttu-id="68a45-105">синкфолдеритемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="68a45-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="68a45-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="68a45-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="68a45-107">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="68a45-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="68a45-108">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="68a45-108">Changes (Items)</span></span>](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="68a45-109">**синкфолдеритемсчанжестипе**</span><span class="sxs-lookup"><span data-stu-id="68a45-109">**SyncFolderItemsChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68a45-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="68a45-110">Attributes and elements</span></span>

<span data-ttu-id="68a45-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="68a45-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68a45-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="68a45-112">Attributes</span></span>

<span data-ttu-id="68a45-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="68a45-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68a45-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="68a45-114">Child elements</span></span>

|<span data-ttu-id="68a45-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68a45-115">**Element**</span></span>|<span data-ttu-id="68a45-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68a45-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68a45-117">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="68a45-117">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="68a45-118">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="68a45-118">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="68a45-119">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="68a45-119">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="68a45-120">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="68a45-120">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="68a45-121">Delete (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="68a45-121">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="68a45-122">Определяет один элемент, который необходимо удалить в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="68a45-122">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="68a45-123">реадфлагчанже</span><span class="sxs-lookup"><span data-stu-id="68a45-123">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="68a45-124">Возвращается в ответах [операции SyncFolderItems](syncfolderitems-operation.md) при чтении элемента.</span><span class="sxs-lookup"><span data-stu-id="68a45-124">Returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="68a45-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68a45-125">This property is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68a45-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="68a45-126">Parent elements</span></span>

|<span data-ttu-id="68a45-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68a45-127">**Element**</span></span>|<span data-ttu-id="68a45-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68a45-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68a45-129">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="68a45-129">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="68a45-130">Содержит состояние и результат запроса [операции SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="68a45-130">Contains the status and result of a [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="68a45-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="68a45-131">Remarks</span></span>

<span data-ttu-id="68a45-132">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="68a45-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68a45-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="68a45-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68a45-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="68a45-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="68a45-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="68a45-135">Schema name</span></span>  <br/> |<span data-ttu-id="68a45-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="68a45-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="68a45-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="68a45-137">Validation file</span></span>  <br/> |<span data-ttu-id="68a45-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="68a45-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68a45-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="68a45-139">Can be empty</span></span>  <br/> |<span data-ttu-id="68a45-140">False</span><span class="sxs-lookup"><span data-stu-id="68a45-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68a45-141">См. также</span><span class="sxs-lookup"><span data-stu-id="68a45-141">See also</span></span>



[<span data-ttu-id="68a45-142">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="68a45-142">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="68a45-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="68a45-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

