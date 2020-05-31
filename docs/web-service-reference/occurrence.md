---
title: Экземпляр
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
description: Элемент вхождения представляет один измененный экземпляр повторяющегося элемента календаря.
ms.openlocfilehash: 5a40faa9b885a235d30e7f41830d1eefe2ed23c3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834653"
---
# <a name="occurrence"></a><span data-ttu-id="44e39-103">Экземпляр</span><span class="sxs-lookup"><span data-stu-id="44e39-103">Occurrence</span></span>

<span data-ttu-id="44e39-104">Элемент **вхождения** представляет один измененный экземпляр повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="44e39-104">The **Occurrence** element represents a single modified occurrence of a recurring calendar item.</span></span> 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

<span data-ttu-id="44e39-105">**оккурренцеинфотипе**</span><span class="sxs-lookup"><span data-stu-id="44e39-105">**OccurrenceInfoType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="44e39-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="44e39-106">Attributes and elements</span></span>

<span data-ttu-id="44e39-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="44e39-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44e39-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="44e39-108">Attributes</span></span>

<span data-ttu-id="44e39-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="44e39-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44e39-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="44e39-110">Child elements</span></span>

|<span data-ttu-id="44e39-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="44e39-111">**Element**</span></span>|<span data-ttu-id="44e39-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="44e39-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44e39-113">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="44e39-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="44e39-114">Содержит уникальный идентификатор и изменяет ключ измененного экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="44e39-114">Contains the unique identifier and change key of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="44e39-115">Начало</span><span class="sxs-lookup"><span data-stu-id="44e39-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="44e39-116">Представляет время начала измененного экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="44e39-116">Represents the start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="44e39-117">Оканчиваться</span><span class="sxs-lookup"><span data-stu-id="44e39-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="44e39-118">Представляет время окончания измененного экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="44e39-118">Represents the end time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="44e39-119">оригиналстарт</span><span class="sxs-lookup"><span data-stu-id="44e39-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="44e39-120">Представляет исходное время начала измененного экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="44e39-120">Represents the original start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="44e39-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="44e39-121">Parent elements</span></span>

|<span data-ttu-id="44e39-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="44e39-122">**Element**</span></span>|<span data-ttu-id="44e39-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="44e39-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44e39-124">модифиедоккурренцес</span><span class="sxs-lookup"><span data-stu-id="44e39-124">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="44e39-125">Содержит коллекцию повторяющихся экземпляров повторяющихся элементов календаря, которые были изменены таким образом, что они отличаются от элемента шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="44e39-125">Contains a collection of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="44e39-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="44e39-126">Remarks</span></span>

<span data-ttu-id="44e39-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="44e39-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44e39-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="44e39-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44e39-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="44e39-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44e39-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="44e39-130">Schema name</span></span>  <br/> |<span data-ttu-id="44e39-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="44e39-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="44e39-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="44e39-132">Validation file</span></span>  <br/> |<span data-ttu-id="44e39-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="44e39-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="44e39-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="44e39-134">Can be empty</span></span>  <br/> |<span data-ttu-id="44e39-135">False</span><span class="sxs-lookup"><span data-stu-id="44e39-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44e39-136">См. также</span><span class="sxs-lookup"><span data-stu-id="44e39-136">See also</span></span>

- [<span data-ttu-id="44e39-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="44e39-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

