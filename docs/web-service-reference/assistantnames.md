---
title: AssistantNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4e69022d-1cef-4744-877c-848a0b5c4f40
description: Элемент AssistantNames указывает массив имен помощник по и идентификаторы их атрибуты источника для связанного пользователя.
ms.openlocfilehash: 7414caa74dc8221d0b1b471c3d5ed09552f7e200
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761503"
---
# <a name="assistantnames"></a><span data-ttu-id="0ce97-103">AssistantNames</span><span class="sxs-lookup"><span data-stu-id="0ce97-103">AssistantNames</span></span>

<span data-ttu-id="0ce97-104">Элемент **AssistantNames** указывает массив имен помощник по и идентификаторы их атрибуты источника для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0ce97-104">The **AssistantNames** element specifies an array of assistant names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantNames>
    <StringAttributedValue></StringAttributedValue>
</AssistantNames>
```

 <span data-ttu-id="0ce97-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="0ce97-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ce97-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0ce97-106">Attributes and elements</span></span>

<span data-ttu-id="0ce97-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0ce97-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ce97-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0ce97-108">Attributes</span></span>

<span data-ttu-id="0ce97-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0ce97-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ce97-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0ce97-110">Child elements</span></span>

|<span data-ttu-id="0ce97-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0ce97-111">**Element**</span></span>|<span data-ttu-id="0ce97-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ce97-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ce97-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="0ce97-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="0ce97-114">Задает экземпляр в массиве атрибутов, связанных с элементом пользователя.</span><span class="sxs-lookup"><span data-stu-id="0ce97-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ce97-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0ce97-115">Parent elements</span></span>

|<span data-ttu-id="0ce97-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0ce97-116">**Element**</span></span>|<span data-ttu-id="0ce97-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ce97-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ce97-118">Пользователь</span><span class="sxs-lookup"><span data-stu-id="0ce97-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="0ce97-119">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="0ce97-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0ce97-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="0ce97-120">Remarks</span></span>

<span data-ttu-id="0ce97-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0ce97-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0ce97-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ce97-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ce97-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0ce97-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ce97-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0ce97-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ce97-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0ce97-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0ce97-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="0ce97-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="0ce97-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0ce97-127">Validation File</span></span>  <br/> |<span data-ttu-id="0ce97-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0ce97-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ce97-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0ce97-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0ce97-130">См. также</span><span class="sxs-lookup"><span data-stu-id="0ce97-130">See also</span></span>

- [<span data-ttu-id="0ce97-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0ce97-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

