---
title: фирстоккурренце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FirstOccurrence
api_type:
- schema
ms.assetid: d6748860-ce0d-4d2e-b7e4-9ed834f1e45a
description: Элемент Фирстоккурренце представляет первое вхождение повторяющегося элемента календаря.
ms.openlocfilehash: 22ee9018df1e89a3783c4dfb56aaf065b2c8ea6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466299"
---
# <a name="firstoccurrence"></a><span data-ttu-id="d855e-103">фирстоккурренце</span><span class="sxs-lookup"><span data-stu-id="d855e-103">FirstOccurrence</span></span>

<span data-ttu-id="d855e-104">Элемент **фирстоккурренце** представляет первое вхождение повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d855e-104">The **FirstOccurrence** element represents the first occurrence of a recurring calendar item.</span></span> 
  
```xml
<FirstOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</FirstOccurrence>
```

 <span data-ttu-id="d855e-105">**оккурренцеинфотипе**</span><span class="sxs-lookup"><span data-stu-id="d855e-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d855e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d855e-106">Attributes and elements</span></span>

<span data-ttu-id="d855e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d855e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d855e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d855e-108">Attributes</span></span>

<span data-ttu-id="d855e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d855e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d855e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d855e-110">Child elements</span></span>

|<span data-ttu-id="d855e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d855e-111">**Element**</span></span>|<span data-ttu-id="d855e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d855e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d855e-113">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="d855e-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d855e-114">Содержит уникальный идентификатор и меняет ключ первого экземпляра повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d855e-114">Contains the unique identifier and change key of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d855e-115">Начало</span><span class="sxs-lookup"><span data-stu-id="d855e-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="d855e-116">Представляет время начала первого вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d855e-116">Represents the start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d855e-117">Оканчиваться</span><span class="sxs-lookup"><span data-stu-id="d855e-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d855e-118">Представляет время окончания первого повторения элемента повторяющегося календаря.</span><span class="sxs-lookup"><span data-stu-id="d855e-118">Represents the end time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d855e-119">оригиналстарт</span><span class="sxs-lookup"><span data-stu-id="d855e-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="d855e-120">Представляет исходное время начала первого вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d855e-120">Represents the original start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d855e-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d855e-121">Parent elements</span></span>

|<span data-ttu-id="d855e-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d855e-122">**Element**</span></span>|<span data-ttu-id="d855e-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d855e-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d855e-124">календаритем</span><span class="sxs-lookup"><span data-stu-id="d855e-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d855e-125">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="d855e-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d855e-126">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="d855e-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d855e-127">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d855e-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d855e-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="d855e-128">Remarks</span></span>

<span data-ttu-id="d855e-129">Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.</span><span class="sxs-lookup"><span data-stu-id="d855e-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="d855e-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d855e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d855e-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d855e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d855e-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d855e-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d855e-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d855e-133">Schema name</span></span>  <br/> |<span data-ttu-id="d855e-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d855e-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d855e-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d855e-135">Validation file</span></span>  <br/> |<span data-ttu-id="d855e-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d855e-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d855e-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d855e-137">Can be empty</span></span>  <br/> |<span data-ttu-id="d855e-138">False</span><span class="sxs-lookup"><span data-stu-id="d855e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d855e-139">См. также</span><span class="sxs-lookup"><span data-stu-id="d855e-139">See also</span></span>



- [<span data-ttu-id="d855e-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d855e-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="d855e-141">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="d855e-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

