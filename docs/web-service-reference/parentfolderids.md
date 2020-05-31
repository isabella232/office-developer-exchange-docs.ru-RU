---
title: парентфолдеридс
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
description: Элемент Парентфолдеридс определяет папки для операций FindItem и FindFolder для поиска.
ms.openlocfilehash: 7c4dcc98d1cabc8e97f2846880c73111dd307dfb
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354171"
---
# <a name="parentfolderids"></a><span data-ttu-id="bea71-103">парентфолдеридс</span><span class="sxs-lookup"><span data-stu-id="bea71-103">ParentFolderIds</span></span>

<span data-ttu-id="bea71-104">Элемент **парентфолдеридс** определяет папки для операций FindItem и FindFolder для поиска.</span><span class="sxs-lookup"><span data-stu-id="bea71-104">The **ParentFolderIds** element identifies folders for the FindItem and FindFolder operations to search.</span></span> 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
<ParentFolderIds>
```

```xml
<ParentFolderIds>
   <FolderId/> 
<ParentFolderIds>
```

<span data-ttu-id="bea71-105">**нонемптяррайофбасефолдеридстипе**</span><span class="sxs-lookup"><span data-stu-id="bea71-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bea71-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bea71-106">Attributes and elements</span></span>

<span data-ttu-id="bea71-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bea71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bea71-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bea71-108">Attributes</span></span>

<span data-ttu-id="bea71-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bea71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bea71-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bea71-110">Child elements</span></span>

|<span data-ttu-id="bea71-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bea71-111">**Element**</span></span>|<span data-ttu-id="bea71-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bea71-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bea71-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="bea71-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="bea71-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="bea71-114">Contains the identifier and change key of a folder.</span></span> <span data-ttu-id="bea71-115">Элемент **парентфолдеридс** должен использовать либо этот элемент, либо элемент [дистингуишедфолдерид](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="bea71-115">The **ParentFolderIds** element must use either this element or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="bea71-116">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="bea71-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="bea71-117">Определяет папки Microsoft Exchange Server 2007, на которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="bea71-117">Identifies Microsoft Exchange Server 2007 folders that can be referenced by name.</span></span> <span data-ttu-id="bea71-118">Элемент **парентфолдеридс** должен использовать либо этот элемент, либо элемент [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="bea71-118">The **ParentFolderIds** element must use either this element or the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bea71-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bea71-119">Parent elements</span></span>

|<span data-ttu-id="bea71-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bea71-120">**Element**</span></span>|<span data-ttu-id="bea71-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bea71-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bea71-122">FindFolder</span><span class="sxs-lookup"><span data-stu-id="bea71-122">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="bea71-123">Определяет запрос на идентификацию папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bea71-123">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bea71-124">FindItem</span><span class="sxs-lookup"><span data-stu-id="bea71-124">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="bea71-125">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="bea71-125">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bea71-126">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="bea71-126">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="bea71-127">Определяет запрос на разрешение неоднозначных имен.</span><span class="sxs-lookup"><span data-stu-id="bea71-127">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bea71-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="bea71-128">Remarks</span></span>

<span data-ttu-id="bea71-129">Элемент **парентфолдеридс** должен использовать элемент [FolderId](folderid.md) или [дистингуишедфолдерид](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="bea71-129">The **ParentFolderIds** element must use either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> <span data-ttu-id="bea71-130">Для поиска может быть определено неограниченное количество папок.</span><span class="sxs-lookup"><span data-stu-id="bea71-130">An unlimited number of folders can be defined for the search.</span></span> 
  
## <a name="example"></a><span data-ttu-id="bea71-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bea71-131">Example</span></span>

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

## <a name="element-information"></a><span data-ttu-id="bea71-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bea71-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bea71-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bea71-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bea71-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bea71-134">Schema Name</span></span>  <br/> |<span data-ttu-id="bea71-135">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bea71-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bea71-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bea71-136">Validation File</span></span>  <br/> |<span data-ttu-id="bea71-137">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bea71-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bea71-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bea71-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="bea71-139">False</span><span class="sxs-lookup"><span data-stu-id="bea71-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bea71-140">См. также</span><span class="sxs-lookup"><span data-stu-id="bea71-140">See also</span></span>

- [<span data-ttu-id="bea71-141">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="bea71-141">FindFolder operation</span></span>](findfolder-operation.md)  
- [<span data-ttu-id="bea71-142">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="bea71-142">FindItem operation</span></span>](finditem-operation.md) 
- [<span data-ttu-id="bea71-143">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="bea71-143">ResolveNames operation</span></span>](resolvenames-operation.md)

