---
title: Атрибуты (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: Атрибуты элемента экземпляр в массиве атрибутов элемента PersonaType.
ms.openlocfilehash: 0e800c92c75bf0c475d4bffd33d6ab49f9ad9a9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761523"
---
# <a name="attribution-personaattributiontype"></a><span data-ttu-id="7e8e7-103">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="7e8e7-103">Attribution (PersonaAttributionType)</span></span>

<span data-ttu-id="7e8e7-104">**Атрибуты** элемента экземпляр в массиве атрибутов элемента **PersonaType** .</span><span class="sxs-lookup"><span data-stu-id="7e8e7-104">The **Attribution** element specifies an instance in an array of attributes for a **PersonaType** element.</span></span> 
  
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

 <span data-ttu-id="7e8e7-105">**PersonaAttributionType**</span><span class="sxs-lookup"><span data-stu-id="7e8e7-105">**PersonaAttributionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e8e7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7e8e7-106">Attributes and elements</span></span>

<span data-ttu-id="7e8e7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e8e7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7e8e7-108">Attributes</span></span>

<span data-ttu-id="7e8e7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e8e7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7e8e7-110">Child elements</span></span>

|<span data-ttu-id="7e8e7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7e8e7-111">**Element**</span></span>|<span data-ttu-id="7e8e7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e8e7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e8e7-113">Идентификатор (строка)</span><span class="sxs-lookup"><span data-stu-id="7e8e7-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="7e8e7-114">Задает строку, которая уникально идентифицирует приложение или атрибуты в пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-114">Specifies a string that uniquely identifies an app or an attribution in a persona.</span></span>  <br/> |
|[<span data-ttu-id="7e8e7-115">SourceId</span><span class="sxs-lookup"><span data-stu-id="7e8e7-115">SourceId</span></span>](sourceid.md) <br/> |<span data-ttu-id="7e8e7-116">Задает идентификатор получателя Active Directory или контакта.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-116">Specifies the identifier of the contact or Active Directory recipient.</span></span>  <br/> |
|[<span data-ttu-id="7e8e7-117">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="7e8e7-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="7e8e7-118">Задает отображаемое имя папки, контактов, список рассылки, делегата или правило.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-118">Defines the display name of a folder, contact, distribution list, delegate user, or rule.</span></span>  <br/> |
|[<span data-ttu-id="7e8e7-119">IsWritable</span><span class="sxs-lookup"><span data-stu-id="7e8e7-119">IsWritable</span></span>](iswritable.md) <br/> |<span data-ttu-id="7e8e7-120">Указывает, можно ли запись базовым контакт или получателя Active Directory для.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-120">Specifies whether the underlying contact or Active Directory recipient can be written to.</span></span>  <br/> |
|[<span data-ttu-id="7e8e7-121">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="7e8e7-121">IsQuickContact</span></span>](isquickcontact.md) <br/> |<span data-ttu-id="7e8e7-122">Задает логическое значение, которое указывает, является ли базовый контакт или получателя Active Directory быстрого контакта.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-122">Specifies a Boolean value that indicates whether the underlying contact or Active Directory recipient is a quick contact.</span></span>  <br/> |
|[<span data-ttu-id="7e8e7-123">IsHidden</span><span class="sxs-lookup"><span data-stu-id="7e8e7-123">IsHidden</span></span>](ishidden.md) <br/> |<span data-ttu-id="7e8e7-124">Содержит логическое значение, указывающее, ли базовый контакт или получателя Active Directory необходимо скрыть или отобразить как часть пользователя.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-124">Contains a Boolean value that indicates whether the underlying contact or Active Directory recipient should be hidden or displayed as part of the persona.</span></span>  <br/> |
|[<span data-ttu-id="7e8e7-125">FolderId</span><span class="sxs-lookup"><span data-stu-id="7e8e7-125">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="7e8e7-126">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-126">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e8e7-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7e8e7-127">Parent elements</span></span>

|<span data-ttu-id="7e8e7-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7e8e7-128">**Element**</span></span>|<span data-ttu-id="7e8e7-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e8e7-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e8e7-130">Атрибуты (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="7e8e7-130">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="7e8e7-131">Указывает массив атрибуты сведения для одной или нескольких контактов или объединить в связанного пользователя active directory (AD) получателей.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-131">Specifies an array of attribution information for one or more of the contacts or active directory (AD) recipients aggregated into the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e8e7-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="7e8e7-132">Remarks</span></span>

<span data-ttu-id="7e8e7-133">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7e8e7-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e8e7-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e8e7-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7e8e7-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e8e7-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7e8e7-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e8e7-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7e8e7-137">Schema Name</span></span>  <br/> |<span data-ttu-id="7e8e7-138">Схема типа</span><span class="sxs-lookup"><span data-stu-id="7e8e7-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="7e8e7-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7e8e7-139">Validation File</span></span>  <br/> |<span data-ttu-id="7e8e7-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e8e7-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e8e7-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7e8e7-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7e8e7-142">См. также</span><span class="sxs-lookup"><span data-stu-id="7e8e7-142">See also</span></span>

- [<span data-ttu-id="7e8e7-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7e8e7-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

