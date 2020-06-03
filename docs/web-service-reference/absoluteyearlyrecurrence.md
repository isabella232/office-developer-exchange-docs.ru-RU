---
title: абсолутэйеарлирекурренце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteYearlyRecurrence
api_type:
- schema
ms.assetid: 96f53e2c-3893-4f6e-a78a-ac179f45c5db
description: Элемент Абсолутэйеарлирекурренце представляет шаблон ежегодного повторения.
ms.openlocfilehash: 19b617dfd5c0a3d206d62439c880da084fd5f5f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460416"
---
# <a name="absoluteyearlyrecurrence"></a><span data-ttu-id="08ace-103">абсолутэйеарлирекурренце</span><span class="sxs-lookup"><span data-stu-id="08ace-103">AbsoluteYearlyRecurrence</span></span>

<span data-ttu-id="08ace-104">Элемент **абсолутэйеарлирекурренце** представляет шаблон ежегодного повторения.</span><span class="sxs-lookup"><span data-stu-id="08ace-104">The **AbsoluteYearlyRecurrence** element represents a yearly recurrence pattern.</span></span> 
  
```xml
<AbsoluteYearlyRecurrence>
   <DayOfMonth/>
   <Month/>
</AbsoluteYearlyRecurrence>
```

 <span data-ttu-id="08ace-105">**абсолутэйеарлирекурренцепаттернтипе**</span><span class="sxs-lookup"><span data-stu-id="08ace-105">**AbsoluteYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08ace-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="08ace-106">Attributes and elements</span></span>

<span data-ttu-id="08ace-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="08ace-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08ace-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="08ace-108">Attributes</span></span>

<span data-ttu-id="08ace-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="08ace-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08ace-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="08ace-110">Child elements</span></span>

|<span data-ttu-id="08ace-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08ace-111">**Element**</span></span>|<span data-ttu-id="08ace-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08ace-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08ace-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="08ace-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="08ace-114">Описывает день месяца, в который происходит повторяющийся элемент.</span><span class="sxs-lookup"><span data-stu-id="08ace-114">Describes the day in a month on which a recurring item occurs.</span></span> <span data-ttu-id="08ace-115">Диапазон значений этого свойства — от 1 до 31.</span><span class="sxs-lookup"><span data-stu-id="08ace-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="08ace-116">Если для определенного месяца это значение превышает количество дней в месяце, для этого свойства подразумевается последний день месяца.</span><span class="sxs-lookup"><span data-stu-id="08ace-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="08ace-117">Month (повторение элемента)</span><span class="sxs-lookup"><span data-stu-id="08ace-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="08ace-118">Описывает месяц, в который происходит ежегодно повторяющийся элемент.</span><span class="sxs-lookup"><span data-stu-id="08ace-118">Describes the month in which a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08ace-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="08ace-119">Parent elements</span></span>

|<span data-ttu-id="08ace-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08ace-120">**Element**</span></span>|<span data-ttu-id="08ace-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08ace-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08ace-122">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="08ace-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="08ace-123">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="08ace-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="08ace-124">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="08ace-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="08ace-125">Содержит шаблон повторения для элементов календаря и приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="08ace-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="08ace-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="08ace-126">Remarks</span></span>

<span data-ttu-id="08ace-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="08ace-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08ace-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="08ace-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08ace-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="08ace-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08ace-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="08ace-130">Schema Name</span></span>  <br/> |<span data-ttu-id="08ace-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="08ace-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="08ace-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="08ace-132">Validation File</span></span>  <br/> |<span data-ttu-id="08ace-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="08ace-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08ace-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="08ace-134">Can Be Empty</span></span>  <br/> |<span data-ttu-id="08ace-135">False</span><span class="sxs-lookup"><span data-stu-id="08ace-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08ace-136">См. также</span><span class="sxs-lookup"><span data-stu-id="08ace-136">See also</span></span>

- [<span data-ttu-id="08ace-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="08ace-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

