---
title: дисплайнамепрефиксес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04250f8d-1b83-43ae-8d2f-e052079bf2fc
description: Элемент Дисплайнамепрефиксес указывает массив префиксов отображаемого имени и идентификаторы их исходных атрибутов для соответствующего пользователя.
ms.openlocfilehash: 09e1e974cbe84ec8c7a4848c3367f2501269b797
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530749"
---
# <a name="displaynameprefixes"></a><span data-ttu-id="ade8b-103">дисплайнамепрефиксес</span><span class="sxs-lookup"><span data-stu-id="ade8b-103">DisplayNamePrefixes</span></span>

<span data-ttu-id="ade8b-104">Элемент **дисплайнамепрефиксес** указывает массив префиксов отображаемого имени и идентификаторы их исходных атрибутов для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="ade8b-104">The **DisplayNamePrefixes** element specifies an array of display name prefixes and the identifiers of their source attributions for the associated persona.</span></span> 
  
```xml
<DisplayNamePrefixes>
    <StringAttributedValue></StringAttributedValue>
</DisplayNamePrefixes>
```

 <span data-ttu-id="ade8b-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="ade8b-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ade8b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ade8b-106">Attributes and elements</span></span>

<span data-ttu-id="ade8b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ade8b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ade8b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ade8b-108">Attributes</span></span>

<span data-ttu-id="ade8b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ade8b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ade8b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ade8b-110">Child elements</span></span>

|<span data-ttu-id="ade8b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ade8b-111">**Element**</span></span>|<span data-ttu-id="ade8b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ade8b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ade8b-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="ade8b-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="ade8b-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="ade8b-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ade8b-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ade8b-115">Parent elements</span></span>

|<span data-ttu-id="ade8b-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ade8b-116">**Element**</span></span>|<span data-ttu-id="ade8b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ade8b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ade8b-118">Роль</span><span class="sxs-lookup"><span data-stu-id="ade8b-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="ade8b-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="ade8b-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ade8b-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="ade8b-120">Remarks</span></span>

<span data-ttu-id="ade8b-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ade8b-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ade8b-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ade8b-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ade8b-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ade8b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ade8b-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ade8b-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ade8b-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ade8b-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ade8b-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="ade8b-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="ade8b-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ade8b-127">Validation File</span></span>  <br/> |<span data-ttu-id="ade8b-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ade8b-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ade8b-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ade8b-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ade8b-130">См. также</span><span class="sxs-lookup"><span data-stu-id="ade8b-130">See also</span></span>

- [<span data-ttu-id="ade8b-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ade8b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

