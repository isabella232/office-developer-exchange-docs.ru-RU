---
title: бусинесшомепажес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9961c0c2-7cac-4af1-84ac-0eafdce0a6ab
description: Элемент Бусинесшомепажес указывает массив рабочих домашних страниц и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: f0e85e0b3c857e44d94bd42c6d3ea757d015eb25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465914"
---
# <a name="businesshomepages"></a><span data-ttu-id="4b255-103">бусинесшомепажес</span><span class="sxs-lookup"><span data-stu-id="4b255-103">BusinessHomePages</span></span>

<span data-ttu-id="4b255-104">Элемент **бусинесшомепажес** указывает массив рабочих домашних страниц и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4b255-104">The **BusinessHomePages** element specifies an array of business home pages and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessHomePages>
    <StringAttributedValue></StringAttributedValue>
</BusinessHomePages>
```

 <span data-ttu-id="4b255-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="4b255-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b255-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4b255-106">Attributes and elements</span></span>

<span data-ttu-id="4b255-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4b255-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b255-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4b255-108">Attributes</span></span>

<span data-ttu-id="4b255-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4b255-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b255-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4b255-110">Child elements</span></span>

|<span data-ttu-id="4b255-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4b255-111">**Element**</span></span>|<span data-ttu-id="4b255-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4b255-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b255-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="4b255-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="4b255-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="4b255-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b255-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4b255-115">Parent elements</span></span>

|<span data-ttu-id="4b255-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4b255-116">**Element**</span></span>|<span data-ttu-id="4b255-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4b255-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b255-118">Роль</span><span class="sxs-lookup"><span data-stu-id="4b255-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="4b255-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="4b255-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4b255-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="4b255-120">Remarks</span></span>

<span data-ttu-id="4b255-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4b255-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4b255-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b255-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b255-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4b255-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b255-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4b255-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b255-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4b255-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4b255-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="4b255-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4b255-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4b255-127">Validation File</span></span>  <br/> |<span data-ttu-id="4b255-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4b255-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4b255-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4b255-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4b255-130">См. также</span><span class="sxs-lookup"><span data-stu-id="4b255-130">See also</span></span>



- [<span data-ttu-id="4b255-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4b255-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

