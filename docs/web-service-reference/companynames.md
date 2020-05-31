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
ms.openlocfilehash: b9024b08cb46d2ccbfcc7b07acb4645894cc5f4c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761692"
---
# <a name="companynames"></a><span data-ttu-id="8a2c4-103">компанинамес</span><span class="sxs-lookup"><span data-stu-id="8a2c4-103">CompanyNames</span></span>

<span data-ttu-id="8a2c4-104">Элемент **компанинамес** содержит массив имен компаний и идентификаторы их исходных атрибутов для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-104">The **CompanyNames** element contains an array of company names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CompanyNames>
    <StringAttributedValue></StringAttributedValue>
</CompanyNames>
```

 <span data-ttu-id="8a2c4-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="8a2c4-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a2c4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8a2c4-106">Attributes and elements</span></span>

<span data-ttu-id="8a2c4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a2c4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8a2c4-108">Attributes</span></span>

<span data-ttu-id="8a2c4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a2c4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8a2c4-110">Child elements</span></span>

|<span data-ttu-id="8a2c4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a2c4-111">**Element**</span></span>|<span data-ttu-id="8a2c4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a2c4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a2c4-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="8a2c4-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="8a2c4-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a2c4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8a2c4-115">Parent elements</span></span>

|<span data-ttu-id="8a2c4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a2c4-116">**Element**</span></span>|<span data-ttu-id="8a2c4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a2c4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a2c4-118">Роль</span><span class="sxs-lookup"><span data-stu-id="8a2c4-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="8a2c4-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="8a2c4-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8a2c4-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="8a2c4-120">Remarks</span></span>

<span data-ttu-id="8a2c4-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8a2c4-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a2c4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a2c4-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8a2c4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a2c4-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8a2c4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a2c4-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8a2c4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8a2c4-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="8a2c4-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="8a2c4-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8a2c4-127">Validation File</span></span>  <br/> |<span data-ttu-id="8a2c4-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8a2c4-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a2c4-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8a2c4-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8a2c4-130">См. также</span><span class="sxs-lookup"><span data-stu-id="8a2c4-130">See also</span></span>



- [<span data-ttu-id="8a2c4-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2c4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

