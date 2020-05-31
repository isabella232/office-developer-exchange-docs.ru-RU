---
title: ластоккурренце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LastOccurrence
api_type:
- schema
ms.assetid: c9ef0fcb-4265-4e60-9986-fff0f211d00b
description: Элемент Ластоккурренце представляет последнее вхождение повторяющегося элемента календаря.
ms.openlocfilehash: 2c8fdfc0005e86c9dda84a48ae1d3692b5134ca8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834209"
---
# <a name="lastoccurrence"></a><span data-ttu-id="d9d3f-103">ластоккурренце</span><span class="sxs-lookup"><span data-stu-id="d9d3f-103">LastOccurrence</span></span>

<span data-ttu-id="d9d3f-104">Элемент **ластоккурренце** представляет последнее вхождение повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-104">The **LastOccurrence** element represents the last occurrence of a recurring calendar item.</span></span> 
  
```xml
<LastOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</LastOccurrence>
```

 <span data-ttu-id="d9d3f-105">**оккурренцеинфотипе**</span><span class="sxs-lookup"><span data-stu-id="d9d3f-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9d3f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d9d3f-106">Attributes and elements</span></span>

<span data-ttu-id="d9d3f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9d3f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d9d3f-108">Attributes</span></span>

<span data-ttu-id="d9d3f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9d3f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d9d3f-110">Child elements</span></span>

|<span data-ttu-id="d9d3f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d9d3f-111">**Element**</span></span>|<span data-ttu-id="d9d3f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d9d3f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9d3f-113">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="d9d3f-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d9d3f-114">Содержит уникальный идентификатор и ключ изменения последнего вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-114">Contains the unique identifier and change key of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d9d3f-115">Начало</span><span class="sxs-lookup"><span data-stu-id="d9d3f-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="d9d3f-116">Представляет время начала последнего повторения элемента повторяющегося календаря.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-116">Represents the start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d9d3f-117">Оканчиваться</span><span class="sxs-lookup"><span data-stu-id="d9d3f-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d9d3f-118">Представляет время окончания последнего повторения элемента повторяющегося календаря.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-118">Represents the end time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d9d3f-119">оригиналстарт</span><span class="sxs-lookup"><span data-stu-id="d9d3f-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="d9d3f-120">Представляет исходное время начала последнего вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-120">Represents the original start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d9d3f-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d9d3f-121">Parent elements</span></span>

|<span data-ttu-id="d9d3f-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d9d3f-122">**Element**</span></span>|<span data-ttu-id="d9d3f-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d9d3f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9d3f-124">календаритем</span><span class="sxs-lookup"><span data-stu-id="d9d3f-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d9d3f-125">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d9d3f-126">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="d9d3f-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d9d3f-127">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d9d3f-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="d9d3f-128">Remarks</span></span>

<span data-ttu-id="d9d3f-129">Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="d9d3f-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d9d3f-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9d3f-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d9d3f-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9d3f-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d9d3f-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9d3f-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d9d3f-133">Schema name</span></span>  <br/> |<span data-ttu-id="d9d3f-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d9d3f-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9d3f-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d9d3f-135">Validation file</span></span>  <br/> |<span data-ttu-id="d9d3f-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d9d3f-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9d3f-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d9d3f-137">Can be empty</span></span>  <br/> |<span data-ttu-id="d9d3f-138">False</span><span class="sxs-lookup"><span data-stu-id="d9d3f-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9d3f-139">См. также</span><span class="sxs-lookup"><span data-stu-id="d9d3f-139">See also</span></span>



- [<span data-ttu-id="d9d3f-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d9d3f-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="d9d3f-141">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="d9d3f-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

