---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: Элемент SavedItemFolderId определяет папку назначения для операций, обновление, отправка и создавать элементы в почтовом ящике.
ms.openlocfilehash: 3f46070a538f5e03007925565a8888efe06b62b7
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354164"
---
# <a name="saveditemfolderid"></a><span data-ttu-id="e5d13-103">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="e5d13-103">SavedItemFolderId</span></span>

<span data-ttu-id="e5d13-104">Элемент **SavedItemFolderId** определяет папку назначения для операций, обновление, отправка и создавать элементы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e5d13-104">The **SavedItemFolderId** element identifies the target folder for operations that update, send, and create items in a mailbox.</span></span> 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

```xml
<SavedItemFolderId>
   <DistinguishedFolderId/>
</SavedItemFolderId>
```

<span data-ttu-id="e5d13-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="e5d13-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e5d13-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e5d13-106">Attributes and elements</span></span>

<span data-ttu-id="e5d13-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e5d13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5d13-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e5d13-108">Attributes</span></span>

<span data-ttu-id="e5d13-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e5d13-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5d13-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e5d13-110">Child elements</span></span>

|<span data-ttu-id="e5d13-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e5d13-111">**Element**</span></span>|<span data-ttu-id="e5d13-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e5d13-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5d13-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="e5d13-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="e5d13-114">Содержит идентификатор и меняет ключ папку назначения для операций обновления, отправки и создания элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5d13-114">Contains the identifier and change key of a target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e5d13-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="e5d13-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="e5d13-116">Определяет целевой папке по именованные идентификатор для операций, обновление, отправка и создания элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5d13-116">Identifies a target folder by a named identifier for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e5d13-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e5d13-117">Parent elements</span></span>

|<span data-ttu-id="e5d13-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e5d13-118">**Element**</span></span>|<span data-ttu-id="e5d13-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e5d13-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5d13-120">CreateItem</span><span class="sxs-lookup"><span data-stu-id="e5d13-120">CreateItem</span></span>](createitem.md) <br/> |<span data-ttu-id="e5d13-121">Определяет запрос на создание элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5d13-121">Defines a request to create an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="e5d13-122">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e5d13-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateItem` <br/> |
|[<span data-ttu-id="e5d13-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="e5d13-123">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="e5d13-124">Определяет запрос на обновление элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5d13-124">Defines a request to update an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="e5d13-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e5d13-125">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
|[<span data-ttu-id="e5d13-126">SendItem</span><span class="sxs-lookup"><span data-stu-id="e5d13-126">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="e5d13-127">Определяет запрос для отправки элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5d13-127">Defines a request to send an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="e5d13-128">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e5d13-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e5d13-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="e5d13-129">Remarks</span></span>

<span data-ttu-id="e5d13-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e5d13-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5d13-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e5d13-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5d13-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e5d13-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e5d13-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e5d13-133">Schema Name</span></span>  <br/> |<span data-ttu-id="e5d13-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e5d13-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e5d13-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e5d13-135">Validation File</span></span>  <br/> |<span data-ttu-id="e5d13-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e5d13-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e5d13-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e5d13-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5d13-138">False</span><span class="sxs-lookup"><span data-stu-id="e5d13-138">False</span></span>  <br/> |
   

