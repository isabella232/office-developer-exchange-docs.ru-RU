---
title: Departments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0a6b0a4-f0dd-4945-af69-628da93f5452
description: Элемент Departments указывает массив названий отделов и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 17590793e00a914cb53b479994bcc89e37bb0e31
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467937"
---
# <a name="departments"></a><span data-ttu-id="94c25-103">Departments</span><span class="sxs-lookup"><span data-stu-id="94c25-103">Departments</span></span>

<span data-ttu-id="94c25-104">Элемент **Departments** указывает массив названий отделов и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="94c25-104">The **Departments** element specifies an array of department names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Departments>
    <StringAttributedValue></StringAttributedValue>
</Departments>
```

 <span data-ttu-id="94c25-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="94c25-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94c25-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="94c25-106">Attributes and elements</span></span>

<span data-ttu-id="94c25-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="94c25-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94c25-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="94c25-108">Attributes</span></span>

<span data-ttu-id="94c25-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="94c25-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94c25-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="94c25-110">Child elements</span></span>

|<span data-ttu-id="94c25-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="94c25-111">**Element**</span></span>|<span data-ttu-id="94c25-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="94c25-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94c25-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="94c25-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="94c25-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="94c25-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94c25-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="94c25-115">Parent elements</span></span>

|<span data-ttu-id="94c25-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="94c25-116">**Element**</span></span>|<span data-ttu-id="94c25-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="94c25-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94c25-118">Роль</span><span class="sxs-lookup"><span data-stu-id="94c25-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="94c25-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="94c25-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="94c25-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="94c25-120">Remarks</span></span>

<span data-ttu-id="94c25-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="94c25-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="94c25-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="94c25-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94c25-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="94c25-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94c25-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="94c25-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94c25-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="94c25-125">Schema Name</span></span>  <br/> |<span data-ttu-id="94c25-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="94c25-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="94c25-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="94c25-127">Validation File</span></span>  <br/> |<span data-ttu-id="94c25-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="94c25-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="94c25-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="94c25-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="94c25-130">См. также</span><span class="sxs-lookup"><span data-stu-id="94c25-130">See also</span></span>

- [<span data-ttu-id="94c25-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="94c25-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

