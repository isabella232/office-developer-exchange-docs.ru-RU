---
title: ParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderIds
api_type:
- schema
ms.assetid: e7998023-e5e0-465c-91fa-2aa6d1559f64
description: Элемент ParentFolderIds определяет папок для операций FindItem и FindFolder для поиска.
ms.openlocfilehash: 4dd23b45dcc397e29e67fc08b29dd773e50f0db1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834688"
---
# <a name="parentfolderids"></a><span data-ttu-id="713e0-103">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="713e0-103">ParentFolderIds</span></span>

<span data-ttu-id="713e0-104">Элемент **ParentFolderIds** определяет папок для операций FindItem и FindFolder для поиска.</span><span class="sxs-lookup"><span data-stu-id="713e0-104">The **ParentFolderIds** element identifies folders for the FindItem and FindFolder operations to search.</span></span> 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
<ParentFolderIds>
```

<span data-ttu-id="713e0-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="713e0-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="713e0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="713e0-106">Attributes and elements</span></span>

<span data-ttu-id="713e0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="713e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="713e0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="713e0-108">Attributes</span></span>

<span data-ttu-id="713e0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="713e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="713e0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="713e0-110">Child elements</span></span>

|<span data-ttu-id="713e0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="713e0-111">**Element**</span></span>|<span data-ttu-id="713e0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="713e0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="713e0-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="713e0-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="713e0-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="713e0-114">Contains the identifier and change key of a folder.</span></span> <span data-ttu-id="713e0-115">Элемент **ParentFolderIds** необходимо использовать этот элемент или элемент [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="713e0-115">The **ParentFolderIds** element must use either this element or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="713e0-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="713e0-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="713e0-117">Идентифицирует папок Microsoft Exchange Server 2007, которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="713e0-117">Identifies Microsoft Exchange Server 2007 folders that can be referenced by name.</span></span> <span data-ttu-id="713e0-118">Элемент **ParentFolderIds** необходимо использовать этот элемент или элемент [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="713e0-118">The **ParentFolderIds** element must use either this element or the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="713e0-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="713e0-119">Parent elements</span></span>

|<span data-ttu-id="713e0-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="713e0-120">**Element**</span></span>|<span data-ttu-id="713e0-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="713e0-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="713e0-122">FindFolder</span><span class="sxs-lookup"><span data-stu-id="713e0-122">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="713e0-123">Определяет запрос для определения папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="713e0-123">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="713e0-124">FindItem</span><span class="sxs-lookup"><span data-stu-id="713e0-124">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="713e0-125">Определяет запрос для поиска элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="713e0-125">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="713e0-126">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="713e0-126">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="713e0-127">Определяет запрос для разрешения неоднозначных имен.</span><span class="sxs-lookup"><span data-stu-id="713e0-127">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="713e0-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="713e0-128">Remarks</span></span>

<span data-ttu-id="713e0-129">Элемент **ParentFolderIds** необходимо использовать [FolderId](folderid.md) или элемент [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="713e0-129">The **ParentFolderIds** element must use either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> <span data-ttu-id="713e0-130">Неограниченное число папок, которые могут задаваться для поиска.</span><span class="sxs-lookup"><span data-stu-id="713e0-130">An unlimited number of folders can be defined for the search.</span></span> 
  
## <a name="example"></a><span data-ttu-id="713e0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="713e0-131">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="713e0-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="713e0-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="713e0-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="713e0-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="713e0-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="713e0-134">Schema Name</span></span>  <br/> |<span data-ttu-id="713e0-135">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="713e0-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="713e0-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="713e0-136">Validation File</span></span>  <br/> |<span data-ttu-id="713e0-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="713e0-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="713e0-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="713e0-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="713e0-139">False</span><span class="sxs-lookup"><span data-stu-id="713e0-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="713e0-140">См. также</span><span class="sxs-lookup"><span data-stu-id="713e0-140">See also</span></span>

- [<span data-ttu-id="713e0-141">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="713e0-141">FindFolder operation</span></span>](findfolder-operation.md)  
- [<span data-ttu-id="713e0-142">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="713e0-142">FindItem operation</span></span>](finditem-operation.md) 
- [<span data-ttu-id="713e0-143">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="713e0-143">ResolveNames operation</span></span>](resolvenames-operation.md)

