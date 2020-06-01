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
ms.openlocfilehash: 6fda7b5602f172bae84ad7b211db2811def4f883
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463267"
---
# <a name="changes-items"></a><span data-ttu-id="ee11e-103">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="ee11e-103">Changes (Items)</span></span>

<span data-ttu-id="ee11e-104">Элемент **Changes** содержит массив последовательности типов изменений, которые представляют типы различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee11e-104">The **Changes** element contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span> 
  
[<span data-ttu-id="ee11e-105">синкфолдеритемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="ee11e-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="ee11e-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="ee11e-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="ee11e-107">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ee11e-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="ee11e-108">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="ee11e-108">Changes (Items)</span></span>](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="ee11e-109">**синкфолдеритемсчанжестипе**</span><span class="sxs-lookup"><span data-stu-id="ee11e-109">**SyncFolderItemsChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee11e-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ee11e-110">Attributes and elements</span></span>

<span data-ttu-id="ee11e-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ee11e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee11e-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ee11e-112">Attributes</span></span>

<span data-ttu-id="ee11e-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ee11e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee11e-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ee11e-114">Child elements</span></span>

|<span data-ttu-id="ee11e-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ee11e-115">**Element**</span></span>|<span data-ttu-id="ee11e-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ee11e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee11e-117">Create (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="ee11e-117">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="ee11e-118">Определяет один элемент, который необходимо создать в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="ee11e-118">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ee11e-119">Обновление (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="ee11e-119">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="ee11e-120">Определяет один элемент для обновления в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="ee11e-120">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ee11e-121">Delete (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="ee11e-121">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="ee11e-122">Определяет один элемент, который необходимо удалить в локальном хранилище клиента.</span><span class="sxs-lookup"><span data-stu-id="ee11e-122">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ee11e-123">реадфлагчанже</span><span class="sxs-lookup"><span data-stu-id="ee11e-123">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="ee11e-124">Возвращается в ответах [операции SyncFolderItems](syncfolderitems-operation.md) при чтении элемента.</span><span class="sxs-lookup"><span data-stu-id="ee11e-124">Returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="ee11e-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee11e-125">This property is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ee11e-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ee11e-126">Parent elements</span></span>

|<span data-ttu-id="ee11e-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ee11e-127">**Element**</span></span>|<span data-ttu-id="ee11e-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ee11e-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee11e-129">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ee11e-129">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="ee11e-130">Содержит состояние и результат запроса [операции SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ee11e-130">Contains the status and result of a [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ee11e-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="ee11e-131">Remarks</span></span>

<span data-ttu-id="ee11e-132">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ee11e-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee11e-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ee11e-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee11e-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ee11e-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ee11e-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ee11e-135">Schema name</span></span>  <br/> |<span data-ttu-id="ee11e-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ee11e-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ee11e-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ee11e-137">Validation file</span></span>  <br/> |<span data-ttu-id="ee11e-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ee11e-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ee11e-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ee11e-139">Can be empty</span></span>  <br/> |<span data-ttu-id="ee11e-140">False</span><span class="sxs-lookup"><span data-stu-id="ee11e-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee11e-141">См. также</span><span class="sxs-lookup"><span data-stu-id="ee11e-141">See also</span></span>



[<span data-ttu-id="ee11e-142">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="ee11e-142">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="ee11e-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ee11e-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

