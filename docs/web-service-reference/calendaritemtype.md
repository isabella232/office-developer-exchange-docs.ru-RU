---
title: CalendarItemType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItemType
api_type:
- schema
ms.assetid: 1feb0788-adf7-4a7c-830c-005214ad930f
description: Элемент CalendarItemType представляет тип элемента календаря.
ms.openlocfilehash: 3fe95c86ea24e6dfeb4740ead5e787bd63b5190d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761647"
---
# <a name="calendaritemtype"></a><span data-ttu-id="64120-103">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="64120-103">CalendarItemType</span></span>

<span data-ttu-id="64120-104">Элемент **CalendarItemType** представляет тип элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="64120-104">The **CalendarItemType** element represents the type of a calendar item.</span></span> 
  
```xml
<CalendarItemType/>
```

 <span data-ttu-id="64120-105">**CalendarItemTypeType**</span><span class="sxs-lookup"><span data-stu-id="64120-105">**CalendarItemTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64120-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="64120-106">Attributes and elements</span></span>

<span data-ttu-id="64120-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="64120-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64120-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="64120-108">Attributes</span></span>

<span data-ttu-id="64120-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="64120-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64120-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64120-110">Child elements</span></span>

<span data-ttu-id="64120-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="64120-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="64120-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="64120-112">Parent elements</span></span>

|<span data-ttu-id="64120-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64120-113">**Element**</span></span>|<span data-ttu-id="64120-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64120-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64120-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="64120-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="64120-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="64120-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="64120-117">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="64120-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="64120-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="64120-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="64120-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="64120-119">Text value</span></span>

<span data-ttu-id="64120-120">Текстовое значение является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="64120-120">A text value is required if this element is used.</span></span> <span data-ttu-id="64120-121">Ниже приведены возможные значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="64120-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="64120-122">**Один** Элемент не связан с повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="64120-122">**Single** The item is not associated with a recurring calendar item.</span></span> 
    
- <span data-ttu-id="64120-123">**Вхождение** Элемент — это вхождение повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="64120-123">**Occurrence** The item is an occurrence of a recurring calendar item.</span></span> 
    
- <span data-ttu-id="64120-124">**Исключение** Элемент является исключением для повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="64120-124">**Exception** The item is an exception to a recurring calendar item.</span></span> 
    
- <span data-ttu-id="64120-125">**RecurringMaster** Элемент главной для набора повторяющихся элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="64120-125">**RecurringMaster** The item is master for a set of recurring calendar items.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="64120-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="64120-126">Remarks</span></span>

<span data-ttu-id="64120-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="64120-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64120-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="64120-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64120-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="64120-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64120-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="64120-130">Schema name</span></span>  <br/> |<span data-ttu-id="64120-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="64120-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="64120-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="64120-132">Validation file</span></span>  <br/> |<span data-ttu-id="64120-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="64120-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64120-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="64120-134">Can be empty</span></span>  <br/> |<span data-ttu-id="64120-135">False</span><span class="sxs-lookup"><span data-stu-id="64120-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64120-136">См. также</span><span class="sxs-lookup"><span data-stu-id="64120-136">See also</span></span>



- [<span data-ttu-id="64120-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="64120-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

