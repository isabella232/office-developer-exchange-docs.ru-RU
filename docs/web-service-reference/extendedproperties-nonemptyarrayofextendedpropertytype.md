---
title: Свойство ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a7034730-210d-4916-b992-dda342f890f8
description: Элемент ExtendedProperties указывает массив дополнительные свойства.
ms.openlocfilehash: b92108ecde63d4a3ac3cc80861c204c4d1950cc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762470"
---
# <a name="extendedproperties-nonemptyarrayofextendedpropertytype"></a><span data-ttu-id="3a5dd-103">Свойство ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="3a5dd-103">ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span></span>

<span data-ttu-id="3a5dd-104">Элемент **ExtendedProperties** указывает массив дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="3a5dd-104">The **ExtendedProperties** element specifies an array of additional properties.</span></span> 
  
```XML
<ExtendedProperties>
    <ExtendedProperty/>
</ExtendedProperties>
```

 <span data-ttu-id="3a5dd-105">**NonEmptyArrayOfExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="3a5dd-105">**NonEmptyArrayOfExtendedPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a5dd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3a5dd-106">Attributes and elements</span></span>

<span data-ttu-id="3a5dd-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3a5dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a5dd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3a5dd-108">Attributes</span></span>

<span data-ttu-id="3a5dd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3a5dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a5dd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3a5dd-110">Child elements</span></span>

|<span data-ttu-id="3a5dd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3a5dd-111">**Element**</span></span>|<span data-ttu-id="3a5dd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a5dd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a5dd-113">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="3a5dd-113">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="3a5dd-114">Задает расширенные свойства MAPI для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="3a5dd-114">Identifies extended MAPI properties on folders and items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a5dd-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3a5dd-115">Parent elements</span></span>

|<span data-ttu-id="3a5dd-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3a5dd-116">**Element**</span></span>|<span data-ttu-id="3a5dd-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a5dd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a5dd-118">ImGroup</span><span class="sxs-lookup"><span data-stu-id="3a5dd-118">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="3a5dd-119">Представляет группу мгновенного обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="3a5dd-119">Represents an instant messaging group.</span></span>  <br/> |
|[<span data-ttu-id="3a5dd-120">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="3a5dd-120">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="3a5dd-121">Указывает сначала 256 символов элемента почтового ящика для предварительной версии без открытия самого элемента.</span><span class="sxs-lookup"><span data-stu-id="3a5dd-121">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3a5dd-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="3a5dd-122">Remarks</span></span>

<span data-ttu-id="3a5dd-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3a5dd-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3a5dd-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a5dd-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a5dd-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3a5dd-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a5dd-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3a5dd-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3a5dd-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3a5dd-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3a5dd-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="3a5dd-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="3a5dd-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3a5dd-129">Validation File</span></span>  <br/> |<span data-ttu-id="3a5dd-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3a5dd-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3a5dd-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3a5dd-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3a5dd-132">См. также</span><span class="sxs-lookup"><span data-stu-id="3a5dd-132">See also</span></span>



- [<span data-ttu-id="3a5dd-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3a5dd-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

