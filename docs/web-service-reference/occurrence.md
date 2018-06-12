---
title: Вхождение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: d292b99c-b896-40b7-be5d-2cb314c9481f
description: Элемент вхождение представляет измененной вхождения повторяющегося элемента календаря.
ms.openlocfilehash: 5a40faa9b885a235d30e7f41830d1eefe2ed23c3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834653"
---
# <a name="occurrence"></a><span data-ttu-id="90952-103">Вхождение</span><span class="sxs-lookup"><span data-stu-id="90952-103">Occurrence</span></span>

<span data-ttu-id="90952-104">Элемент **вхождение** представляет измененной вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="90952-104">The **Occurrence** element represents a single modified occurrence of a recurring calendar item.</span></span> 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

<span data-ttu-id="90952-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="90952-105">**OccurrenceInfoType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="90952-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="90952-106">Attributes and elements</span></span>

<span data-ttu-id="90952-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="90952-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90952-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="90952-108">Attributes</span></span>

<span data-ttu-id="90952-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="90952-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90952-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="90952-110">Child elements</span></span>

|<span data-ttu-id="90952-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="90952-111">**Element**</span></span>|<span data-ttu-id="90952-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="90952-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90952-113">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="90952-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="90952-114">Содержит уникальный идентификатор и меняет ключ измененная копия повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="90952-114">Contains the unique identifier and change key of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="90952-115">Start</span><span class="sxs-lookup"><span data-stu-id="90952-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="90952-116">Представляет время начала измененная копия повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="90952-116">Represents the start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="90952-117">End</span><span class="sxs-lookup"><span data-stu-id="90952-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="90952-118">Представляет время окончания измененные вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="90952-118">Represents the end time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="90952-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="90952-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="90952-120">Представляет исходное время начала измененные вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="90952-120">Represents the original start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90952-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="90952-121">Parent elements</span></span>

|<span data-ttu-id="90952-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="90952-122">**Element**</span></span>|<span data-ttu-id="90952-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="90952-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90952-124">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="90952-124">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="90952-125">Содержит коллекцию повторяющихся вхождения элемента календаря, которые были изменены, отличного от элемента шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="90952-125">Contains a collection of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="90952-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="90952-126">Remarks</span></span>

<span data-ttu-id="90952-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="90952-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90952-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="90952-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90952-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="90952-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90952-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="90952-130">Schema name</span></span>  <br/> |<span data-ttu-id="90952-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="90952-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="90952-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="90952-132">Validation file</span></span>  <br/> |<span data-ttu-id="90952-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="90952-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90952-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="90952-134">Can be empty</span></span>  <br/> |<span data-ttu-id="90952-135">False</span><span class="sxs-lookup"><span data-stu-id="90952-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90952-136">См. также</span><span class="sxs-lookup"><span data-stu-id="90952-136">See also</span></span>

- [<span data-ttu-id="90952-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="90952-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

