---
title: Delete (Итемсинк)
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
ms.assetid: 4f372d57-2e39-46af-9d83-6c8c55108587
description: Элемент Delete определяет отдельный элемент, который необходимо удалить из локального хранилища клиента.
ms.openlocfilehash: 6e30ddc7f7248fe7ff7136e19ba58c7d5d8a800f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454682"
---
# <a name="delete-itemsync"></a><span data-ttu-id="59a56-103">Delete (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="59a56-103">Delete (ItemSync)</span></span>

<span data-ttu-id="59a56-104">Элемент **Delete** определяет отдельный элемент, который необходимо удалить из локального хранилища клиента.</span><span class="sxs-lookup"><span data-stu-id="59a56-104">The **Delete** element identifies a single item to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="59a56-105">синкфолдеритемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="59a56-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)  
- [<span data-ttu-id="59a56-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="59a56-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="59a56-107">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="59a56-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="59a56-108">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="59a56-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="59a56-109">Delete (Итемсинк)</span><span class="sxs-lookup"><span data-stu-id="59a56-109">Delete (ItemSync)</span></span>](delete-itemsync.md)
  
```xml
<Delete>
   <ItemId/>
</Delete>
```

<span data-ttu-id="59a56-110">**синкфолдеритемсделететипе**</span><span class="sxs-lookup"><span data-stu-id="59a56-110">**SyncFolderItemsDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="59a56-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="59a56-111">Attributes and elements</span></span>

<span data-ttu-id="59a56-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="59a56-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59a56-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="59a56-113">Attributes</span></span>

<span data-ttu-id="59a56-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="59a56-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59a56-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="59a56-115">Child elements</span></span>

|<span data-ttu-id="59a56-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="59a56-116">**Element**</span></span>|<span data-ttu-id="59a56-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="59a56-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59a56-118">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="59a56-118">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="59a56-119">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="59a56-119">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59a56-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="59a56-120">Parent elements</span></span>

|<span data-ttu-id="59a56-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="59a56-121">**Element**</span></span>|<span data-ttu-id="59a56-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="59a56-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59a56-123">Изменения (элементы)</span><span class="sxs-lookup"><span data-stu-id="59a56-123">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="59a56-124">Содержит массив последовательности типов изменений, представляющих тип различий между элементами на клиенте и элементами на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="59a56-124">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59a56-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="59a56-125">Remarks</span></span>

<span data-ttu-id="59a56-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="59a56-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59a56-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="59a56-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59a56-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="59a56-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59a56-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="59a56-129">Schema name</span></span>  <br/> |<span data-ttu-id="59a56-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="59a56-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="59a56-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="59a56-131">Validation file</span></span>  <br/> |<span data-ttu-id="59a56-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="59a56-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59a56-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="59a56-133">Can be empty</span></span>  <br/> |<span data-ttu-id="59a56-134">False</span><span class="sxs-lookup"><span data-stu-id="59a56-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59a56-135">См. также</span><span class="sxs-lookup"><span data-stu-id="59a56-135">See also</span></span>

- [<span data-ttu-id="59a56-136">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="59a56-136">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="59a56-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="59a56-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

