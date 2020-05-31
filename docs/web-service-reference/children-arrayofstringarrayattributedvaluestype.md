---
title: Дочерние элементы (Аррайофстрингаррайаттрибутедвалуестипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d37b3fd5-63f1-4003-a6ec-54adfce23d52
description: Элемент Children указывает массив дочерних имен и идентификаторов их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 7c98e7cb96cecad0d1b5122236b6cd0947c6b3d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761679"
---
# <a name="children-arrayofstringarrayattributedvaluestype"></a><span data-ttu-id="c7f9f-103">Дочерние элементы (Аррайофстрингаррайаттрибутедвалуестипе)</span><span class="sxs-lookup"><span data-stu-id="c7f9f-103">Children (ArrayOfStringArrayAttributedValuesType)</span></span>

<span data-ttu-id="c7f9f-104">Элемент **Children** указывает массив дочерних имен и идентификаторов их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7f9f-104">The **Children** element specifies an array of child names and identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Children>
    <StringAttributedValue></StringAttributedValue>
</Children>
```

 <span data-ttu-id="c7f9f-105">**аррайофстрингаррайаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="c7f9f-105">**ArrayOfStringArrayAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7f9f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c7f9f-106">Attributes and elements</span></span>

<span data-ttu-id="c7f9f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c7f9f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7f9f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c7f9f-108">Attributes</span></span>

<span data-ttu-id="c7f9f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c7f9f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7f9f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c7f9f-110">Child elements</span></span>

|<span data-ttu-id="c7f9f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c7f9f-111">**Element**</span></span>|<span data-ttu-id="c7f9f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c7f9f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7f9f-113">стрингаррайаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="c7f9f-113">StringArrayAttributedValue</span></span>](stringarrayattributedvalue.md) <br/> |<span data-ttu-id="c7f9f-114">Задает экземпляр массива строковых данных для элемента персоны.</span><span class="sxs-lookup"><span data-stu-id="c7f9f-114">Specifies an instance of an array of string data for a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7f9f-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c7f9f-115">Parent elements</span></span>

|<span data-ttu-id="c7f9f-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c7f9f-116">**Element**</span></span>|<span data-ttu-id="c7f9f-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c7f9f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7f9f-118">Роль</span><span class="sxs-lookup"><span data-stu-id="c7f9f-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="c7f9f-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="c7f9f-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c7f9f-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="c7f9f-120">Remarks</span></span>

<span data-ttu-id="c7f9f-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c7f9f-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c7f9f-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7f9f-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7f9f-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c7f9f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7f9f-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c7f9f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c7f9f-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c7f9f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c7f9f-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="c7f9f-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="c7f9f-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c7f9f-127">Validation File</span></span>  <br/> |<span data-ttu-id="c7f9f-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c7f9f-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c7f9f-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c7f9f-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c7f9f-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c7f9f-130">See also</span></span>



- [<span data-ttu-id="c7f9f-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c7f9f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

