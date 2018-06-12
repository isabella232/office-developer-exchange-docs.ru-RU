---
title: DeletedOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrences
api_type:
- schema
ms.assetid: 736fb305-9528-4be8-ad37-65d7556edbf2
description: Элемент DeletedOccurrences содержит массив удаленных вхождения повторяющегося элемента календаря.
ms.openlocfilehash: 269c1176913cd642f93987462286dd1fee3a7339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762030"
---
# <a name="deletedoccurrences"></a><span data-ttu-id="730c1-103">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="730c1-103">DeletedOccurrences</span></span>

<span data-ttu-id="730c1-104">Элемент **DeletedOccurrences** содержит массив удаленных вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="730c1-104">The **DeletedOccurrences** element contains an array of deleted occurrences of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrences>
   <DeletedOccurrence/>
</DeletedOccurrences>
```

 <span data-ttu-id="730c1-105">**NonEmptyArrayOfDeletedOccurrencesType**</span><span class="sxs-lookup"><span data-stu-id="730c1-105">**NonEmptyArrayOfDeletedOccurrencesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="730c1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="730c1-106">Attributes and elements</span></span>

<span data-ttu-id="730c1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="730c1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="730c1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="730c1-108">Attributes</span></span>

<span data-ttu-id="730c1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="730c1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="730c1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="730c1-110">Child elements</span></span>

|<span data-ttu-id="730c1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="730c1-111">**Element**</span></span>|<span data-ttu-id="730c1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="730c1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="730c1-113">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="730c1-113">DeletedOccurrence</span></span>](deletedoccurrence.md) <br/> |<span data-ttu-id="730c1-114">Представляет удаленных вхождение повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="730c1-114">Represents a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="730c1-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="730c1-115">Parent elements</span></span>

|<span data-ttu-id="730c1-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="730c1-116">**Element**</span></span>|<span data-ttu-id="730c1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="730c1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="730c1-118">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="730c1-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="730c1-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="730c1-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="730c1-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="730c1-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="730c1-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="730c1-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="730c1-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="730c1-122">Remarks</span></span>

<span data-ttu-id="730c1-123">Этот элемент является допустимым, если используется значение RecurringMaster текст для элемента [CalendarItemType](calendaritemtype.md) .</span><span class="sxs-lookup"><span data-stu-id="730c1-123">This element is valid if the RecurringMaster text value is used for the [CalendarItemType](calendaritemtype.md) element.</span></span> 
  
<span data-ttu-id="730c1-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="730c1-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="730c1-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="730c1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="730c1-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="730c1-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="730c1-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="730c1-127">Schema name</span></span>  <br/> |<span data-ttu-id="730c1-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="730c1-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="730c1-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="730c1-129">Validation file</span></span>  <br/> |<span data-ttu-id="730c1-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="730c1-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="730c1-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="730c1-131">Can be empty</span></span>  <br/> |<span data-ttu-id="730c1-132">False</span><span class="sxs-lookup"><span data-stu-id="730c1-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="730c1-133">См. также</span><span class="sxs-lookup"><span data-stu-id="730c1-133">See also</span></span>

- [<span data-ttu-id="730c1-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="730c1-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="730c1-135">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="730c1-135">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

