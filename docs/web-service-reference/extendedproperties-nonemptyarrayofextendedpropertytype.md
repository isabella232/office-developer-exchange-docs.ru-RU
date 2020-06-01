---
title: Екстендедпропертиес (Нонемптяррайофекстендедпропертитипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a7034730-210d-4916-b992-dda342f890f8
description: Элемент Екстендедпропертиес указывает массив дополнительных свойств.
ms.openlocfilehash: 36011e0252ed391daefab190d4da679fb3a3f856
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463099"
---
# <a name="extendedproperties-nonemptyarrayofextendedpropertytype"></a><span data-ttu-id="84897-103">Екстендедпропертиес (Нонемптяррайофекстендедпропертитипе)</span><span class="sxs-lookup"><span data-stu-id="84897-103">ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span></span>

<span data-ttu-id="84897-104">Элемент **екстендедпропертиес** указывает массив дополнительных свойств.</span><span class="sxs-lookup"><span data-stu-id="84897-104">The **ExtendedProperties** element specifies an array of additional properties.</span></span> 
  
```XML
<ExtendedProperties>
    <ExtendedProperty/>
</ExtendedProperties>
```

 <span data-ttu-id="84897-105">**нонемптяррайофекстендедпропертитипе**</span><span class="sxs-lookup"><span data-stu-id="84897-105">**NonEmptyArrayOfExtendedPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84897-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="84897-106">Attributes and elements</span></span>

<span data-ttu-id="84897-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="84897-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84897-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="84897-108">Attributes</span></span>

<span data-ttu-id="84897-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="84897-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84897-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="84897-110">Child elements</span></span>

|<span data-ttu-id="84897-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="84897-111">**Element**</span></span>|<span data-ttu-id="84897-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="84897-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84897-113">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="84897-113">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="84897-114">Определяет расширенные свойства MAPI для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="84897-114">Identifies extended MAPI properties on folders and items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="84897-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="84897-115">Parent elements</span></span>

|<span data-ttu-id="84897-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="84897-116">**Element**</span></span>|<span data-ttu-id="84897-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="84897-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84897-118">Группа</span><span class="sxs-lookup"><span data-stu-id="84897-118">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="84897-119">Представляет группу мгновенных сообщений.</span><span class="sxs-lookup"><span data-stu-id="84897-119">Represents an instant messaging group.</span></span>  <br/> |
|[<span data-ttu-id="84897-120">сеарчпревиевитем</span><span class="sxs-lookup"><span data-stu-id="84897-120">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="84897-121">Задает первые 256 символов элемента почтового ящика для предварительного просмотра без открытия элемента.</span><span class="sxs-lookup"><span data-stu-id="84897-121">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="84897-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="84897-122">Remarks</span></span>

<span data-ttu-id="84897-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="84897-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="84897-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="84897-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84897-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="84897-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84897-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="84897-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="84897-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="84897-127">Schema Name</span></span>  <br/> |<span data-ttu-id="84897-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="84897-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="84897-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="84897-129">Validation File</span></span>  <br/> |<span data-ttu-id="84897-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="84897-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="84897-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="84897-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="84897-132">См. также</span><span class="sxs-lookup"><span data-stu-id="84897-132">See also</span></span>



- [<span data-ttu-id="84897-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="84897-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

