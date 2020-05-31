---
title: Атрибуты (Персонааттрибутионтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: Элемент Attribute указывает экземпляр в массиве атрибутов для элемента Персонатипе.
ms.openlocfilehash: 0e800c92c75bf0c475d4bffd33d6ab49f9ad9a9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761523"
---
# <a name="attribution-personaattributiontype"></a><span data-ttu-id="e9606-103">Атрибуты (Персонааттрибутионтипе)</span><span class="sxs-lookup"><span data-stu-id="e9606-103">Attribution (PersonaAttributionType)</span></span>

<span data-ttu-id="e9606-104">Элемент **Attribute** указывает экземпляр в массиве атрибутов для элемента **персонатипе** .</span><span class="sxs-lookup"><span data-stu-id="e9606-104">The **Attribution** element specifies an instance in an array of attributes for a **PersonaType** element.</span></span> 
  
```XML
<Attribution>
    <Id></Id>
    <SourceId></SourceId>
    <DisplayName></DisplayName>
    <IsWritable></IsWritable>
    <IsQuickContact></IsQuickContact>
    <IsHidden></IsHidden>
    <FolderId></FolderId>
</Attribution>
```

 <span data-ttu-id="e9606-105">**персонааттрибутионтипе**</span><span class="sxs-lookup"><span data-stu-id="e9606-105">**PersonaAttributionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9606-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e9606-106">Attributes and elements</span></span>

<span data-ttu-id="e9606-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e9606-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9606-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e9606-108">Attributes</span></span>

<span data-ttu-id="e9606-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e9606-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9606-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e9606-110">Child elements</span></span>

|<span data-ttu-id="e9606-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e9606-111">**Element**</span></span>|<span data-ttu-id="e9606-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e9606-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9606-113">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="e9606-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="e9606-114">Указывает строку, которая уникально идентифицирует приложение или атрибуты в имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="e9606-114">Specifies a string that uniquely identifies an app or an attribution in a persona.</span></span>  <br/> |
|[<span data-ttu-id="e9606-115">SourceId</span><span class="sxs-lookup"><span data-stu-id="e9606-115">SourceId</span></span>](sourceid.md) <br/> |<span data-ttu-id="e9606-116">Указывает идентификатор контакта или получателя Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e9606-116">Specifies the identifier of the contact or Active Directory recipient.</span></span>  <br/> |
|[<span data-ttu-id="e9606-117">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="e9606-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="e9606-118">Определяет отображаемое имя папки, контакта, списка рассылки, делегированного пользователя или правила.</span><span class="sxs-lookup"><span data-stu-id="e9606-118">Defines the display name of a folder, contact, distribution list, delegate user, or rule.</span></span>  <br/> |
|[<span data-ttu-id="e9606-119">Доступный для записи</span><span class="sxs-lookup"><span data-stu-id="e9606-119">IsWritable</span></span>](iswritable.md) <br/> |<span data-ttu-id="e9606-120">Указывает, можно ли записывать базового контакта или получателя Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e9606-120">Specifies whether the underlying contact or Active Directory recipient can be written to.</span></span>  <br/> |
|[<span data-ttu-id="e9606-121">искуиккконтакт</span><span class="sxs-lookup"><span data-stu-id="e9606-121">IsQuickContact</span></span>](isquickcontact.md) <br/> |<span data-ttu-id="e9606-122">Задает логическое значение, указывающее, является ли основной контакт или получатель Active Directory быстрым контактом.</span><span class="sxs-lookup"><span data-stu-id="e9606-122">Specifies a Boolean value that indicates whether the underlying contact or Active Directory recipient is a quick contact.</span></span>  <br/> |
|[<span data-ttu-id="e9606-123">IsHidden</span><span class="sxs-lookup"><span data-stu-id="e9606-123">IsHidden</span></span>](ishidden.md) <br/> |<span data-ttu-id="e9606-124">Содержит логическое значение, которое указывает, следует ли скрывать или показывать базовый контакт или получатель Active Directory в составе персонажа.</span><span class="sxs-lookup"><span data-stu-id="e9606-124">Contains a Boolean value that indicates whether the underlying contact or Active Directory recipient should be hidden or displayed as part of the persona.</span></span>  <br/> |
|[<span data-ttu-id="e9606-125">FolderId</span><span class="sxs-lookup"><span data-stu-id="e9606-125">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="e9606-126">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="e9606-126">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9606-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e9606-127">Parent elements</span></span>

|<span data-ttu-id="e9606-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e9606-128">**Element**</span></span>|<span data-ttu-id="e9606-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e9606-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9606-130">Атрибуты (Аррайофперсонааттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="e9606-130">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="e9606-131">Задает массив сведений о сопоставлении для одного или нескольких получателей контактов или Active Directory (AD), собранных в сопоставленный с ним пользователь.</span><span class="sxs-lookup"><span data-stu-id="e9606-131">Specifies an array of attribution information for one or more of the contacts or active directory (AD) recipients aggregated into the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9606-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="e9606-132">Remarks</span></span>

<span data-ttu-id="e9606-133">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e9606-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e9606-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9606-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9606-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e9606-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9606-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e9606-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9606-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e9606-137">Schema Name</span></span>  <br/> |<span data-ttu-id="e9606-138">Схема типа</span><span class="sxs-lookup"><span data-stu-id="e9606-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="e9606-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e9606-139">Validation File</span></span>  <br/> |<span data-ttu-id="e9606-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e9606-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9606-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e9606-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e9606-142">См. также</span><span class="sxs-lookup"><span data-stu-id="e9606-142">See also</span></span>

- [<span data-ttu-id="e9606-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e9606-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

