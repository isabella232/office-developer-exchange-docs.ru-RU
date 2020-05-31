---
title: DisplayName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dedd43c8-c1d6-4671-89c5-ce7ab3979fda
description: Элемент DisplayName указывает массив отображаемых имен и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 66f10edd26a467af290535196778fbcb550c16ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762185"
---
# <a name="displaynames"></a><span data-ttu-id="93e20-103">DisplayName</span><span class="sxs-lookup"><span data-stu-id="93e20-103">DisplayNames</span></span>

<span data-ttu-id="93e20-104">Элемент **DisplayName** указывает массив отображаемых имен и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="93e20-104">The **DisplayNames** element specifies an array of display names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```xml
<DisplayNames>
    <StringAttributedValue></StringAttributedValue>
</DisplayNames>
```

 <span data-ttu-id="93e20-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="93e20-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93e20-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93e20-106">Attributes and elements</span></span>

<span data-ttu-id="93e20-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="93e20-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93e20-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93e20-108">Attributes</span></span>

<span data-ttu-id="93e20-109">Нет</span><span class="sxs-lookup"><span data-stu-id="93e20-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93e20-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93e20-110">Child elements</span></span>

|<span data-ttu-id="93e20-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93e20-111">**Element**</span></span>|<span data-ttu-id="93e20-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93e20-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93e20-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="93e20-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="93e20-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="93e20-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93e20-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93e20-115">Parent elements</span></span>

|<span data-ttu-id="93e20-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93e20-116">**Element**</span></span>|<span data-ttu-id="93e20-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93e20-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93e20-118">Роль</span><span class="sxs-lookup"><span data-stu-id="93e20-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="93e20-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="93e20-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93e20-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="93e20-120">Remarks</span></span>

<span data-ttu-id="93e20-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="93e20-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="93e20-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="93e20-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93e20-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93e20-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93e20-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93e20-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93e20-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93e20-125">Schema Name</span></span>  <br/> |<span data-ttu-id="93e20-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="93e20-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="93e20-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93e20-127">Validation File</span></span>  <br/> |<span data-ttu-id="93e20-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="93e20-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="93e20-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93e20-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="93e20-130">См. также</span><span class="sxs-lookup"><span data-stu-id="93e20-130">See also</span></span>

- [<span data-ttu-id="93e20-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="93e20-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

