---
title: конфликтингмитингкаунт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: Элемент Конфликтингмитингкаунт представляет количество собраний, которые конфликтуют с элементом календаря.
ms.openlocfilehash: ace800982c284cf65ff22d92c711197ee5ee1d06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761710"
---
# <a name="conflictingmeetingcount"></a><span data-ttu-id="989b1-103">конфликтингмитингкаунт</span><span class="sxs-lookup"><span data-stu-id="989b1-103">ConflictingMeetingCount</span></span>

<span data-ttu-id="989b1-104">Элемент **конфликтингмитингкаунт** представляет количество собраний, которые конфликтуют с элементом календаря.</span><span class="sxs-lookup"><span data-stu-id="989b1-104">The **ConflictingMeetingCount** element represents the number of meetings that conflict with the calendar item.</span></span> 
  
```xml
<ConflictingMeetingCount/>
```

 <span data-ttu-id="989b1-105">**int**</span><span class="sxs-lookup"><span data-stu-id="989b1-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="989b1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="989b1-106">Attributes and elements</span></span>

<span data-ttu-id="989b1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="989b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="989b1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="989b1-108">Attributes</span></span>

<span data-ttu-id="989b1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="989b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="989b1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="989b1-110">Child elements</span></span>

<span data-ttu-id="989b1-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="989b1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="989b1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="989b1-112">Parent elements</span></span>

|<span data-ttu-id="989b1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="989b1-113">**Element**</span></span>|<span data-ttu-id="989b1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="989b1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="989b1-115">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="989b1-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="989b1-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="989b1-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="989b1-117">календаритем</span><span class="sxs-lookup"><span data-stu-id="989b1-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="989b1-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="989b1-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="989b1-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="989b1-119">Text value</span></span>

<span data-ttu-id="989b1-120">Текстовое значение представляет целое число.</span><span class="sxs-lookup"><span data-stu-id="989b1-120">The text value represents an integer.</span></span> <span data-ttu-id="989b1-121">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="989b1-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="989b1-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="989b1-122">Remarks</span></span>

<span data-ttu-id="989b1-123">Элемент календаря считается конфликтующим, если он происходит, по крайней мере, частично, в то же время, что и другой элемент календаря в той же папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="989b1-123">A calendar item is considered conflicting if it occurs, at least in part, at the same time as another calendar item in the same calendar folder.</span></span> <span data-ttu-id="989b1-124">Если элемент календаря находится в папке "некалендарный", он сравнивается с элементами календаря в папке "Календарь" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="989b1-124">If a calendar item is in a noncalendar folder, it is compared with calendar items in the default calendar folder.</span></span> <span data-ttu-id="989b1-125">Приглашения на собрания сравниваются с элементами календаря в папке "Календарь" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="989b1-125">Meeting requests are compared with calendar items in the default calendar folder.</span></span>
  
<span data-ttu-id="989b1-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="989b1-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="989b1-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="989b1-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="989b1-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="989b1-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="989b1-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="989b1-129">Schema name</span></span>  <br/> |<span data-ttu-id="989b1-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="989b1-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="989b1-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="989b1-131">Validation file</span></span>  <br/> |<span data-ttu-id="989b1-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="989b1-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="989b1-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="989b1-133">Can be empty</span></span>  <br/> |<span data-ttu-id="989b1-134">False</span><span class="sxs-lookup"><span data-stu-id="989b1-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="989b1-135">См. также</span><span class="sxs-lookup"><span data-stu-id="989b1-135">See also</span></span>



- [<span data-ttu-id="989b1-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="989b1-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

