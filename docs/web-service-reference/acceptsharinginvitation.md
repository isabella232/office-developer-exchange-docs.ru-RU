---
title: акцептшарингинвитатион
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
description: Элемент Акцептшарингинвитатион используется для принятия приглашения, позволяющего получить доступ к данным календаря или контактов другого пользователя.
ms.openlocfilehash: c8cdae707bd122e74fa0e284163d1540d857c3de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461711"
---
# <a name="acceptsharinginvitation"></a><span data-ttu-id="e6b8f-103">акцептшарингинвитатион</span><span class="sxs-lookup"><span data-stu-id="e6b8f-103">AcceptSharingInvitation</span></span>

<span data-ttu-id="e6b8f-104">Элемент **акцептшарингинвитатион** используется для принятия приглашения, позволяющего получить доступ к данным календаря или контактов другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6b8f-104">The **AcceptSharingInvitation** element is used to accept an invitation that allows access to another user's calendar or contacts data.</span></span> 
  
```xml
<AcceptSharingInvitation>
   <ReferenceItemId/>
</AcceptSharingInvitation>
```

 <span data-ttu-id="e6b8f-105">**акцептшарингинвитатионтипе**</span><span class="sxs-lookup"><span data-stu-id="e6b8f-105">**AcceptSharingInvitationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6b8f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e6b8f-106">Attributes and elements</span></span>

<span data-ttu-id="e6b8f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e6b8f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6b8f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e6b8f-108">Attributes</span></span>

<span data-ttu-id="e6b8f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e6b8f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6b8f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e6b8f-110">Child elements</span></span>

|<span data-ttu-id="e6b8f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e6b8f-111">**Element**</span></span>|<span data-ttu-id="e6b8f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e6b8f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6b8f-113">референцеитемид</span><span class="sxs-lookup"><span data-stu-id="e6b8f-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="e6b8f-114">Определяет элемент, на который ссылается объект Response.</span><span class="sxs-lookup"><span data-stu-id="e6b8f-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e6b8f-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e6b8f-115">Parent elements</span></span>

|<span data-ttu-id="e6b8f-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e6b8f-116">**Element**</span></span>|<span data-ttu-id="e6b8f-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e6b8f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6b8f-118">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="e6b8f-118">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="e6b8f-119">Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6b8f-119">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e6b8f-120">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="e6b8f-120">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="e6b8f-121">Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="e6b8f-121">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e6b8f-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="e6b8f-122">Remarks</span></span>

<span data-ttu-id="e6b8f-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6b8f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6b8f-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e6b8f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6b8f-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e6b8f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e6b8f-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e6b8f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e6b8f-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e6b8f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="e6b8f-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e6b8f-128">Validation File</span></span>  <br/> |<span data-ttu-id="e6b8f-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e6b8f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e6b8f-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e6b8f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6b8f-131">False</span><span class="sxs-lookup"><span data-stu-id="e6b8f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6b8f-132">См. также</span><span class="sxs-lookup"><span data-stu-id="e6b8f-132">See also</span></span>

- [<span data-ttu-id="e6b8f-133">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="e6b8f-133">CreateItem (AcceptSharingInvitation)</span></span>](createitem-acceptsharinginvitation.md)
- [<span data-ttu-id="e6b8f-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e6b8f-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

