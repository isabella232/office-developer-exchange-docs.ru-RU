---
title: SharingEffectiveRights (PermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: 808bb4a1-aa2d-48c5-94b3-551b52c348bd
description: Элемент SharingEffectiveRights указывает разрешения, которые пользователь имеет для контактных данных, общий.
ms.openlocfilehash: 19e67827dd2dbff6fb70423980d670da5cc257a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835486"
---
# <a name="sharingeffectiverights-permissionreadaccesstype"></a><span data-ttu-id="458aa-103">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="458aa-103">SharingEffectiveRights (PermissionReadAccessType)</span></span>

<span data-ttu-id="458aa-104">Элемент **SharingEffectiveRights** указывает разрешения, которые пользователь имеет для контактных данных, общий.</span><span class="sxs-lookup"><span data-stu-id="458aa-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the contact data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | FullDetails</SharingEffectiveRights >
```

 <span data-ttu-id="458aa-105">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="458aa-105">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="458aa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="458aa-106">Attributes and elements</span></span>

<span data-ttu-id="458aa-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="458aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="458aa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="458aa-108">Attributes</span></span>

<span data-ttu-id="458aa-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="458aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="458aa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="458aa-110">Child elements</span></span>

<span data-ttu-id="458aa-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="458aa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="458aa-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="458aa-112">Parent elements</span></span>

|<span data-ttu-id="458aa-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="458aa-113">**Element**</span></span>|<span data-ttu-id="458aa-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="458aa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="458aa-115">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="458aa-115">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="458aa-116">Представляет папку Контакты, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="458aa-116">Represents a Contacts folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="458aa-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="458aa-117">Text value</span></span>

<span data-ttu-id="458aa-118">В следующей таблице приведены возможные значения для элемента **SharingEffectiveRights** .</span><span class="sxs-lookup"><span data-stu-id="458aa-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
<span data-ttu-id="458aa-119">**SharingEffectiveRights элемент текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="458aa-119">**SharingEffectiveRights element text values**</span></span>

|<span data-ttu-id="458aa-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="458aa-120">**Value**</span></span>|<span data-ttu-id="458aa-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="458aa-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="458aa-122">Нет</span><span class="sxs-lookup"><span data-stu-id="458aa-122">None</span></span>  <br/> |<span data-ttu-id="458aa-123">Указывает, что пользователь не имеет разрешения на чтение элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="458aa-123">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="458aa-124">FullDetails</span><span class="sxs-lookup"><span data-stu-id="458aa-124">FullDetails</span></span>  <br/> |<span data-ttu-id="458aa-125">Указывает, что пользователь имеет разрешение на чтение всех элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="458aa-125">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="458aa-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="458aa-126">Remarks</span></span>

<span data-ttu-id="458aa-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="458aa-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="458aa-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="458aa-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="458aa-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="458aa-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="458aa-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="458aa-130">Schema Name</span></span>  <br/> |<span data-ttu-id="458aa-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="458aa-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="458aa-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="458aa-132">Validation File</span></span>  <br/> |<span data-ttu-id="458aa-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="458aa-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="458aa-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="458aa-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="458aa-135">False</span><span class="sxs-lookup"><span data-stu-id="458aa-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="458aa-136">См. также</span><span class="sxs-lookup"><span data-stu-id="458aa-136">See also</span></span>



- [<span data-ttu-id="458aa-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="458aa-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

