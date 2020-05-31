---
title: саведитемфолдерид
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
description: Элемент Саведитемфолдерид определяет целевую папку для операций обновления, отправки и создания элементов в почтовом ящике.
ms.openlocfilehash: 3f46070a538f5e03007925565a8888efe06b62b7
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354164"
---
# <a name="saveditemfolderid"></a><span data-ttu-id="125d4-103">саведитемфолдерид</span><span class="sxs-lookup"><span data-stu-id="125d4-103">SavedItemFolderId</span></span>

<span data-ttu-id="125d4-104">Элемент **саведитемфолдерид** определяет целевую папку для операций обновления, отправки и создания элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="125d4-104">The **SavedItemFolderId** element identifies the target folder for operations that update, send, and create items in a mailbox.</span></span> 
  
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

<span data-ttu-id="125d4-105">**таржетфолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="125d4-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="125d4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="125d4-106">Attributes and elements</span></span>

<span data-ttu-id="125d4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="125d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="125d4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="125d4-108">Attributes</span></span>

<span data-ttu-id="125d4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="125d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="125d4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="125d4-110">Child elements</span></span>

|<span data-ttu-id="125d4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="125d4-111">**Element**</span></span>|<span data-ttu-id="125d4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="125d4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="125d4-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="125d4-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="125d4-114">Содержит идентификатор и ключ изменения целевой папки для операций, которые обновляют, отправляют и создают элементы в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="125d4-114">Contains the identifier and change key of a target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="125d4-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="125d4-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="125d4-116">Определяет целевую папку с помощью именованного идентификатора для операций, которые обновляют, отправляют и создают элементы в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="125d4-116">Identifies a target folder by a named identifier for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="125d4-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="125d4-117">Parent elements</span></span>

|<span data-ttu-id="125d4-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="125d4-118">**Element**</span></span>|<span data-ttu-id="125d4-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="125d4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="125d4-120">CreateItem</span><span class="sxs-lookup"><span data-stu-id="125d4-120">CreateItem</span></span>](createitem.md) <br/> |<span data-ttu-id="125d4-121">Определяет запрос на создание элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="125d4-121">Defines a request to create an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="125d4-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="125d4-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateItem` <br/> |
|[<span data-ttu-id="125d4-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="125d4-123">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="125d4-124">Определяет запрос на обновление элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="125d4-124">Defines a request to update an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="125d4-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="125d4-125">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
|[<span data-ttu-id="125d4-126">SendItem</span><span class="sxs-lookup"><span data-stu-id="125d4-126">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="125d4-127">Определяет запрос на отправку элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="125d4-127">Defines a request to send an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="125d4-128">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="125d4-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="125d4-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="125d4-129">Remarks</span></span>

<span data-ttu-id="125d4-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="125d4-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="125d4-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="125d4-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="125d4-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="125d4-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="125d4-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="125d4-133">Schema Name</span></span>  <br/> |<span data-ttu-id="125d4-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="125d4-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="125d4-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="125d4-135">Validation File</span></span>  <br/> |<span data-ttu-id="125d4-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="125d4-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="125d4-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="125d4-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="125d4-138">False</span><span class="sxs-lookup"><span data-stu-id="125d4-138">False</span></span>  <br/> |
   

