---
title: Инициалы (Аррайофстрингаттрибутедвалуестипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 060c0cf1-c632-484c-87f5-f577017a7090
description: Элемент Initials указывает массив значений инициалов и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 16133192fa1d9ef066e46a181f490248a8197e5b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458203"
---
# <a name="initials-arrayofstringattributedvaluestype"></a><span data-ttu-id="8cfa4-103">Инициалы (Аррайофстрингаттрибутедвалуестипе)</span><span class="sxs-lookup"><span data-stu-id="8cfa4-103">Initials (ArrayOfStringAttributedValuesType)</span></span>

<span data-ttu-id="8cfa4-104">Элемент **Initials** указывает массив значений инициалов и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8cfa4-104">The **Initials** element specifies an array of initials values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Initials>
    <StringAttributedValue/>
</Initials>
```

 <span data-ttu-id="8cfa4-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="8cfa4-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8cfa4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8cfa4-106">Attributes and elements</span></span>

<span data-ttu-id="8cfa4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8cfa4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8cfa4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8cfa4-108">Attributes</span></span>

<span data-ttu-id="8cfa4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8cfa4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8cfa4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8cfa4-110">Child elements</span></span>

|<span data-ttu-id="8cfa4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8cfa4-111">**Element**</span></span>|<span data-ttu-id="8cfa4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8cfa4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8cfa4-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="8cfa4-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="8cfa4-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="8cfa4-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8cfa4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8cfa4-115">Parent elements</span></span>

|<span data-ttu-id="8cfa4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8cfa4-116">**Element**</span></span>|<span data-ttu-id="8cfa4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8cfa4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8cfa4-118">Роль</span><span class="sxs-lookup"><span data-stu-id="8cfa4-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="8cfa4-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="8cfa4-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8cfa4-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="8cfa4-120">Remarks</span></span>

<span data-ttu-id="8cfa4-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8cfa4-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8cfa4-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8cfa4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8cfa4-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8cfa4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8cfa4-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8cfa4-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8cfa4-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8cfa4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="8cfa4-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="8cfa4-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="8cfa4-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8cfa4-127">Validation File</span></span>  <br/> |<span data-ttu-id="8cfa4-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8cfa4-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8cfa4-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8cfa4-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8cfa4-130">См. также</span><span class="sxs-lookup"><span data-stu-id="8cfa4-130">See also</span></span>



- [<span data-ttu-id="8cfa4-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8cfa4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

