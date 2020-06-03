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
ms.openlocfilehash: 6bc4b9cfe96c6c83cbeb623ec176e33177356bbc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465431"
---
# <a name="parentfolderids"></a><span data-ttu-id="71e4d-103">парентфолдеридс</span><span class="sxs-lookup"><span data-stu-id="71e4d-103">ParentFolderIds</span></span>

<span data-ttu-id="71e4d-104">Элемент **парентфолдеридс** определяет папки для операций FindItem и FindFolder для поиска.</span><span class="sxs-lookup"><span data-stu-id="71e4d-104">The **ParentFolderIds** element identifies folders for the FindItem and FindFolder operations to search.</span></span> 
  
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

<span data-ttu-id="71e4d-105">**нонемптяррайофбасефолдеридстипе**</span><span class="sxs-lookup"><span data-stu-id="71e4d-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="71e4d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="71e4d-106">Attributes and elements</span></span>

<span data-ttu-id="71e4d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="71e4d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71e4d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="71e4d-108">Attributes</span></span>

<span data-ttu-id="71e4d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="71e4d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71e4d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="71e4d-110">Child elements</span></span>

|<span data-ttu-id="71e4d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71e4d-111">**Element**</span></span>|<span data-ttu-id="71e4d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71e4d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71e4d-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="71e4d-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="71e4d-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="71e4d-114">Contains the identifier and change key of a folder.</span></span> <span data-ttu-id="71e4d-115">Элемент **парентфолдеридс** должен использовать либо этот элемент, либо элемент [дистингуишедфолдерид](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="71e4d-115">The **ParentFolderIds** element must use either this element or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="71e4d-116">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="71e4d-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="71e4d-117">Определяет папки Microsoft Exchange Server 2007, на которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="71e4d-117">Identifies Microsoft Exchange Server 2007 folders that can be referenced by name.</span></span> <span data-ttu-id="71e4d-118">Элемент **парентфолдеридс** должен использовать либо этот элемент, либо элемент [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="71e4d-118">The **ParentFolderIds** element must use either this element or the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71e4d-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="71e4d-119">Parent elements</span></span>

|<span data-ttu-id="71e4d-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71e4d-120">**Element**</span></span>|<span data-ttu-id="71e4d-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71e4d-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71e4d-122">FindFolder</span><span class="sxs-lookup"><span data-stu-id="71e4d-122">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="71e4d-123">Определяет запрос на идентификацию папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="71e4d-123">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="71e4d-124">FindItem</span><span class="sxs-lookup"><span data-stu-id="71e4d-124">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="71e4d-125">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="71e4d-125">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="71e4d-126">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="71e4d-126">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="71e4d-127">Определяет запрос на разрешение неоднозначных имен.</span><span class="sxs-lookup"><span data-stu-id="71e4d-127">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="71e4d-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="71e4d-128">Remarks</span></span>

<span data-ttu-id="71e4d-129">Элемент **парентфолдеридс** должен использовать элемент [FolderId](folderid.md) или [дистингуишедфолдерид](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="71e4d-129">The **ParentFolderIds** element must use either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> <span data-ttu-id="71e4d-130">Для поиска может быть определено неограниченное количество папок.</span><span class="sxs-lookup"><span data-stu-id="71e4d-130">An unlimited number of folders can be defined for the search.</span></span> 
  
## <a name="example"></a><span data-ttu-id="71e4d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="71e4d-131">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="71e4d-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="71e4d-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71e4d-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="71e4d-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="71e4d-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="71e4d-134">Schema Name</span></span>  <br/> |<span data-ttu-id="71e4d-135">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="71e4d-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="71e4d-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="71e4d-136">Validation File</span></span>  <br/> |<span data-ttu-id="71e4d-137">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="71e4d-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="71e4d-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="71e4d-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="71e4d-139">False</span><span class="sxs-lookup"><span data-stu-id="71e4d-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71e4d-140">См. также</span><span class="sxs-lookup"><span data-stu-id="71e4d-140">See also</span></span>

- [<span data-ttu-id="71e4d-141">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="71e4d-141">FindFolder operation</span></span>](findfolder-operation.md)  
- [<span data-ttu-id="71e4d-142">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="71e4d-142">FindItem operation</span></span>](finditem-operation.md) 
- [<span data-ttu-id="71e4d-143">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="71e4d-143">ResolveNames operation</span></span>](resolvenames-operation.md)

