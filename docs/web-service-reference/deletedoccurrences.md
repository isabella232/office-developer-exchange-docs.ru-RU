---
title: делетедоккурренцес
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
description: Элемент Делетедоккурренцес содержит массив удаленных вхождений повторяющегося элемента календаря.
ms.openlocfilehash: be39ff95b5529481a36b7549e638818a20e01283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463708"
---
# <a name="deletedoccurrences"></a><span data-ttu-id="c07df-103">делетедоккурренцес</span><span class="sxs-lookup"><span data-stu-id="c07df-103">DeletedOccurrences</span></span>

<span data-ttu-id="c07df-104">Элемент **делетедоккурренцес** содержит массив удаленных вхождений повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="c07df-104">The **DeletedOccurrences** element contains an array of deleted occurrences of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrences>
   <DeletedOccurrence/>
</DeletedOccurrences>
```

 <span data-ttu-id="c07df-105">**нонемптяррайофделетедоккурренцестипе**</span><span class="sxs-lookup"><span data-stu-id="c07df-105">**NonEmptyArrayOfDeletedOccurrencesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c07df-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c07df-106">Attributes and elements</span></span>

<span data-ttu-id="c07df-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c07df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c07df-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c07df-108">Attributes</span></span>

<span data-ttu-id="c07df-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c07df-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c07df-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c07df-110">Child elements</span></span>

|<span data-ttu-id="c07df-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c07df-111">**Element**</span></span>|<span data-ttu-id="c07df-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c07df-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c07df-113">делетедоккурренце</span><span class="sxs-lookup"><span data-stu-id="c07df-113">DeletedOccurrence</span></span>](deletedoccurrence.md) <br/> |<span data-ttu-id="c07df-114">Представляет удаленное вхождение повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="c07df-114">Represents a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c07df-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c07df-115">Parent elements</span></span>

|<span data-ttu-id="c07df-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c07df-116">**Element**</span></span>|<span data-ttu-id="c07df-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c07df-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c07df-118">календаритем</span><span class="sxs-lookup"><span data-stu-id="c07df-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c07df-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="c07df-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c07df-120">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="c07df-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c07df-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c07df-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c07df-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="c07df-122">Remarks</span></span>

<span data-ttu-id="c07df-123">Этот элемент является допустимым, если для элемента [календаритемтипе](calendaritemtype.md) используется текстовое значение рекуррингмастер.</span><span class="sxs-lookup"><span data-stu-id="c07df-123">This element is valid if the RecurringMaster text value is used for the [CalendarItemType](calendaritemtype.md) element.</span></span> 
  
<span data-ttu-id="c07df-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c07df-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c07df-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c07df-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c07df-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c07df-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c07df-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c07df-127">Schema name</span></span>  <br/> |<span data-ttu-id="c07df-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c07df-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="c07df-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c07df-129">Validation file</span></span>  <br/> |<span data-ttu-id="c07df-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c07df-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c07df-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c07df-131">Can be empty</span></span>  <br/> |<span data-ttu-id="c07df-132">False</span><span class="sxs-lookup"><span data-stu-id="c07df-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c07df-133">См. также</span><span class="sxs-lookup"><span data-stu-id="c07df-133">See also</span></span>

- [<span data-ttu-id="c07df-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c07df-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="c07df-135">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="c07df-135">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

