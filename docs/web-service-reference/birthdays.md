---
title: Дни рождения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5a84c19e-57cd-448e-af4f-c8005fd5f2a2
description: Элемент рождения указывает массив рождения, сохраненных в виде строки и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: 2511a2acf0eb2eb24f06e98a1c660d289687bd02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761564"
---
# <a name="birthdays"></a><span data-ttu-id="56a67-103">Дни рождения</span><span class="sxs-lookup"><span data-stu-id="56a67-103">Birthdays</span></span>

<span data-ttu-id="56a67-104">Элемент **рождения** указывает массив рождения, сохраненных в виде строки и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="56a67-104">The **Birthdays** element specifies an array of birthdays, stored as strings, and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Birthdays>
   <StringAttributedValue/>
</Birthdays>
```

 <span data-ttu-id="56a67-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="56a67-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56a67-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="56a67-106">Attributes and elements</span></span>

<span data-ttu-id="56a67-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="56a67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56a67-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="56a67-108">Attributes</span></span>

<span data-ttu-id="56a67-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="56a67-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56a67-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="56a67-110">Child elements</span></span>

|<span data-ttu-id="56a67-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="56a67-111">**Element**</span></span>|<span data-ttu-id="56a67-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="56a67-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56a67-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="56a67-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="56a67-114">Задает экземпляр в массиве атрибутов, связанных с элементом пользователя.</span><span class="sxs-lookup"><span data-stu-id="56a67-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="56a67-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="56a67-115">Parent elements</span></span>

|<span data-ttu-id="56a67-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="56a67-116">**Element**</span></span>|<span data-ttu-id="56a67-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="56a67-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56a67-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="56a67-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="56a67-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="56a67-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="56a67-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="56a67-120">Remarks</span></span>

<span data-ttu-id="56a67-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="56a67-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="56a67-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="56a67-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56a67-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="56a67-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56a67-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="56a67-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56a67-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="56a67-125">Schema Name</span></span>  <br/> |<span data-ttu-id="56a67-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="56a67-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="56a67-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="56a67-127">Validation File</span></span>  <br/> |<span data-ttu-id="56a67-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="56a67-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="56a67-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="56a67-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="56a67-130">См. также</span><span class="sxs-lookup"><span data-stu-id="56a67-130">See also</span></span>



- [<span data-ttu-id="56a67-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="56a67-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

