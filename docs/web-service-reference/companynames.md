---
title: компанинамес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 615fa52d-86ff-4630-b188-5fdb9391eee2
description: Элемент Компанинамес содержит массив имен компаний и идентификаторы их исходных атрибутов для соответствующего пользователя.
ms.openlocfilehash: 25daa43873fe00837004217e3f814a7201638450
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463260"
---
# <a name="companynames"></a><span data-ttu-id="4a46e-103">компанинамес</span><span class="sxs-lookup"><span data-stu-id="4a46e-103">CompanyNames</span></span>

<span data-ttu-id="4a46e-104">Элемент **компанинамес** содержит массив имен компаний и идентификаторы их исходных атрибутов для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="4a46e-104">The **CompanyNames** element contains an array of company names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CompanyNames>
    <StringAttributedValue></StringAttributedValue>
</CompanyNames>
```

 <span data-ttu-id="4a46e-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="4a46e-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a46e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4a46e-106">Attributes and elements</span></span>

<span data-ttu-id="4a46e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4a46e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a46e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4a46e-108">Attributes</span></span>

<span data-ttu-id="4a46e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4a46e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a46e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4a46e-110">Child elements</span></span>

|<span data-ttu-id="4a46e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4a46e-111">**Element**</span></span>|<span data-ttu-id="4a46e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4a46e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a46e-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="4a46e-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="4a46e-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="4a46e-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a46e-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4a46e-115">Parent elements</span></span>

|<span data-ttu-id="4a46e-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4a46e-116">**Element**</span></span>|<span data-ttu-id="4a46e-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4a46e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a46e-118">Роль</span><span class="sxs-lookup"><span data-stu-id="4a46e-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="4a46e-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="4a46e-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4a46e-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="4a46e-120">Remarks</span></span>

<span data-ttu-id="4a46e-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4a46e-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4a46e-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4a46e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a46e-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4a46e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a46e-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4a46e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a46e-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4a46e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4a46e-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="4a46e-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4a46e-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4a46e-127">Validation File</span></span>  <br/> |<span data-ttu-id="4a46e-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4a46e-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a46e-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4a46e-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4a46e-130">См. также</span><span class="sxs-lookup"><span data-stu-id="4a46e-130">See also</span></span>



- [<span data-ttu-id="4a46e-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4a46e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

