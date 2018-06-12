---
title: DeletedOccurrenceStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a9c01c64-e76c-4adc-8b04-88af97bd0cc8
description: DeletedOccurrenceStateDefinition указывает состояние для удаленных вхождение элемента календаря.
ms.openlocfilehash: ad0434d604ee78ebf1905b60857929e1af4d45f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762028"
---
# <a name="deletedoccurrencestatedefinition"></a><span data-ttu-id="cdaa3-103">DeletedOccurrenceStateDefinition</span><span class="sxs-lookup"><span data-stu-id="cdaa3-103">DeletedOccurrenceStateDefinition</span></span>

<span data-ttu-id="cdaa3-104">**DeletedOccurrenceStateDefinition** указывает состояние для удаленных вхождение элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-104">The **DeletedOccurrenceStateDefinition** specifies the state for a deleted occurrence of a calendar item.</span></span> 
  
```XML
<DeletedOccurrenceStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeletedOccurrenceStateDefinition>
```

 <span data-ttu-id="cdaa3-105">**DeletedOccurrenceStateDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="cdaa3-105">**DeletedOccurrenceStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cdaa3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cdaa3-106">Attributes and elements</span></span>

<span data-ttu-id="cdaa3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cdaa3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cdaa3-108">Attributes</span></span>

<span data-ttu-id="cdaa3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cdaa3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cdaa3-110">Child elements</span></span>

|<span data-ttu-id="cdaa3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cdaa3-111">**Element**</span></span>|<span data-ttu-id="cdaa3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cdaa3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cdaa3-113">Вхождение (часовой пояс переходов)</span><span class="sxs-lookup"><span data-stu-id="cdaa3-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="cdaa3-114">Указывает дату вхождение элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="cdaa3-115">IsOccurrencePresent</span><span class="sxs-lookup"><span data-stu-id="cdaa3-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="cdaa3-116">Задает логическое значение, которое указывает наличие вхождения элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cdaa3-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cdaa3-117">Parent elements</span></span>

|<span data-ttu-id="cdaa3-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cdaa3-118">**Element**</span></span>|<span data-ttu-id="cdaa3-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cdaa3-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cdaa3-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="cdaa3-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="cdaa3-121">Задает определение состояний.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cdaa3-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="cdaa3-122">Remarks</span></span>

<span data-ttu-id="cdaa3-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cdaa3-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cdaa3-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cdaa3-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cdaa3-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cdaa3-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cdaa3-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cdaa3-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cdaa3-127">Schema Name</span></span>  <br/> |<span data-ttu-id="cdaa3-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="cdaa3-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="cdaa3-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cdaa3-129">Validation File</span></span>  <br/> |<span data-ttu-id="cdaa3-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cdaa3-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="cdaa3-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cdaa3-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cdaa3-132">См. также</span><span class="sxs-lookup"><span data-stu-id="cdaa3-132">See also</span></span>

- [<span data-ttu-id="cdaa3-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cdaa3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

