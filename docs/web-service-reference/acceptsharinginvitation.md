---
title: AcceptSharingInvitation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AcceptSharingInvitation
api_type:
- schema
ms.assetid: 3c2a47d6-490d-425b-8893-089a4f8882cd
description: Элемент AcceptSharingInvitation используется для принятия приглашения, которая позволяет получить доступ к календарю другого пользователя или данных контактов.
ms.openlocfilehash: 06439739e6cc544d5039ac9d18e0452b1d42a0ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762481"
---
# <a name="acceptsharinginvitation"></a><span data-ttu-id="a5a38-103">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="a5a38-103">AcceptSharingInvitation</span></span>

<span data-ttu-id="a5a38-104">Элемент **AcceptSharingInvitation** используется для принятия приглашения, которая позволяет получить доступ к календарю другого пользователя или данных контактов.</span><span class="sxs-lookup"><span data-stu-id="a5a38-104">The **AcceptSharingInvitation** element is used to accept an invitation that allows access to another user's calendar or contacts data.</span></span> 
  
```xml
<AcceptSharingInvitation>
   <ReferenceItemId/>
</AcceptSharingInvitation>
```

 <span data-ttu-id="a5a38-105">**AcceptSharingInvitationType**</span><span class="sxs-lookup"><span data-stu-id="a5a38-105">**AcceptSharingInvitationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5a38-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a5a38-106">Attributes and elements</span></span>

<span data-ttu-id="a5a38-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a5a38-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5a38-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a5a38-108">Attributes</span></span>

<span data-ttu-id="a5a38-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5a38-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5a38-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a5a38-110">Child elements</span></span>

|<span data-ttu-id="a5a38-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5a38-111">**Element**</span></span>|<span data-ttu-id="a5a38-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5a38-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5a38-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="a5a38-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="a5a38-114">Определяет элемент, к которому относится объект ответа.</span><span class="sxs-lookup"><span data-stu-id="a5a38-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a5a38-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a5a38-115">Parent elements</span></span>

|<span data-ttu-id="a5a38-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5a38-116">**Element**</span></span>|<span data-ttu-id="a5a38-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5a38-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5a38-118">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="a5a38-118">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="a5a38-119">Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5a38-119">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a5a38-120">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="a5a38-120">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="a5a38-121">Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="a5a38-121">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a5a38-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="a5a38-122">Remarks</span></span>

<span data-ttu-id="a5a38-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5a38-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5a38-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a5a38-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5a38-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a5a38-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a5a38-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a5a38-126">Schema Name</span></span>  <br/> |<span data-ttu-id="a5a38-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a5a38-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="a5a38-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a5a38-128">Validation File</span></span>  <br/> |<span data-ttu-id="a5a38-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a5a38-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a5a38-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a5a38-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5a38-131">False</span><span class="sxs-lookup"><span data-stu-id="a5a38-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5a38-132">См. также</span><span class="sxs-lookup"><span data-stu-id="a5a38-132">See also</span></span>

- [<span data-ttu-id="a5a38-133">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="a5a38-133">CreateItem (AcceptSharingInvitation)</span></span>](createitem-acceptsharinginvitation.md)
- [<span data-ttu-id="a5a38-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a5a38-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

