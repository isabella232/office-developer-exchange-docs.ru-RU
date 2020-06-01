---
title: Ожида
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 637560b5-2b08-4787-a5d8-e0467f83acca
description: Элемент поколений указывает массив значений создания и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: a3ef0e2c73e2ebd7c121f817b8ea97c5e4d4d333
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463015"
---
# <a name="generations"></a><span data-ttu-id="02cde-103">Ожида</span><span class="sxs-lookup"><span data-stu-id="02cde-103">Generations</span></span>

<span data-ttu-id="02cde-104">Элемент **поколений** указывает массив значений создания и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="02cde-104">The **Generations** element specifies an array of generation values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Generations>
    <StringAttributedValue/>
</Generations>
```

 <span data-ttu-id="02cde-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="02cde-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02cde-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02cde-106">Attributes and elements</span></span>

<span data-ttu-id="02cde-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="02cde-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02cde-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="02cde-108">Attributes</span></span>

<span data-ttu-id="02cde-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="02cde-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02cde-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="02cde-110">Child elements</span></span>

|<span data-ttu-id="02cde-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="02cde-111">**Element**</span></span>|<span data-ttu-id="02cde-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02cde-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02cde-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="02cde-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="02cde-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="02cde-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02cde-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="02cde-115">Parent elements</span></span>

|<span data-ttu-id="02cde-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="02cde-116">**Element**</span></span>|<span data-ttu-id="02cde-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02cde-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02cde-118">Роль</span><span class="sxs-lookup"><span data-stu-id="02cde-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="02cde-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="02cde-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="02cde-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="02cde-120">Remarks</span></span>

<span data-ttu-id="02cde-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="02cde-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="02cde-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="02cde-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02cde-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="02cde-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02cde-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="02cde-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="02cde-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="02cde-125">Schema Name</span></span>  <br/> |<span data-ttu-id="02cde-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="02cde-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="02cde-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="02cde-127">Validation File</span></span>  <br/> |<span data-ttu-id="02cde-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="02cde-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="02cde-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="02cde-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="02cde-130">См. также</span><span class="sxs-lookup"><span data-stu-id="02cde-130">See also</span></span>



- [<span data-ttu-id="02cde-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="02cde-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

