---
title: GlobalParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f5fcbcb-05ed-462a-99cf-a6b112a4aef6
description: Элемент GlobalParentFolderIds указывает идентификаторы глобального родительских папок.
ms.openlocfilehash: b0ff9ab00f3e46351b5a2db9bc4b6282fa4385cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833747"
---
# <a name="globalparentfolderids"></a><span data-ttu-id="6defd-103">GlobalParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="6defd-103">GlobalParentFolderIds</span></span>

<span data-ttu-id="6defd-104">Элемент **GlobalParentFolderIds** указывает идентификаторы глобального родительских папок.</span><span class="sxs-lookup"><span data-stu-id="6defd-104">The **GlobalParentFolderIds** element specifies the identifiers of the global parent folders.</span></span> 
  
```XML
<GlobalParentFolderIds>
    <FolderId/>
    <DistinguishedFolderId/>
</GlobalParentFolderIds>
```

 <span data-ttu-id="6defd-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="6defd-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6defd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6defd-106">Attributes and elements</span></span>

<span data-ttu-id="6defd-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6defd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6defd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6defd-108">Attributes</span></span>

<span data-ttu-id="6defd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6defd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6defd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6defd-110">Child elements</span></span>

|<span data-ttu-id="6defd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6defd-111">**Element**</span></span>|<span data-ttu-id="6defd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6defd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6defd-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="6defd-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="6defd-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="6defd-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="6defd-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="6defd-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="6defd-116">Идентифицирует папки, которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="6defd-116">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6defd-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6defd-117">Parent elements</span></span>

|<span data-ttu-id="6defd-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6defd-118">**Element**</span></span>|<span data-ttu-id="6defd-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6defd-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6defd-120">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6defd-120">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="6defd-121">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="6defd-121">Represents a single conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6defd-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="6defd-122">Remarks</span></span>

<span data-ttu-id="6defd-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6defd-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6defd-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6defd-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6defd-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6defd-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6defd-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6defd-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6defd-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6defd-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6defd-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="6defd-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="6defd-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6defd-129">Validation File</span></span>  <br/> |<span data-ttu-id="6defd-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6defd-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6defd-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6defd-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6defd-132">См. также</span><span class="sxs-lookup"><span data-stu-id="6defd-132">See also</span></span>



- [<span data-ttu-id="6defd-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6defd-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

