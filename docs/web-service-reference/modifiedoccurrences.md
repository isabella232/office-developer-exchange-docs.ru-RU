---
title: модифиедоккурренцес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedOccurrences
api_type:
- schema
ms.assetid: 552932fc-b3b4-486e-8d73-32c0bb10bd68
description: Элемент Модифиедоккурренцес содержит массив повторяющихся повторений элементов календаря, измененный таким образом, что они отличаются от элемента шаблона повторения.
ms.openlocfilehash: d599e3d232bfffc5bedd37f3dae4d8b10a82ffde
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530424"
---
# <a name="modifiedoccurrences"></a><span data-ttu-id="9c3f4-103">модифиедоккурренцес</span><span class="sxs-lookup"><span data-stu-id="9c3f4-103">ModifiedOccurrences</span></span>

<span data-ttu-id="9c3f4-104">Элемент **модифиедоккурренцес** содержит массив повторяющихся повторений элементов календаря, измененный таким образом, что они отличаются от элемента шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="9c3f4-104">The **ModifiedOccurrences** element contains an array of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span> 
  
```xml
<ModifiedOccurrences>
   <Occurrence/>
</ModifiedOccurrences>
```

 <span data-ttu-id="9c3f4-105">**нонемптяррайофоккурренцеинфотипе**</span><span class="sxs-lookup"><span data-stu-id="9c3f4-105">**NonEmptyArrayOfOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c3f4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9c3f4-106">Attributes and elements</span></span>

<span data-ttu-id="9c3f4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9c3f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c3f4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9c3f4-108">Attributes</span></span>

<span data-ttu-id="9c3f4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9c3f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c3f4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9c3f4-110">Child elements</span></span>

|<span data-ttu-id="9c3f4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9c3f4-111">**Element**</span></span>|<span data-ttu-id="9c3f4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9c3f4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c3f4-113">Экземпляр</span><span class="sxs-lookup"><span data-stu-id="9c3f4-113">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="9c3f4-114">Представляет один измененный экземпляр повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="9c3f4-114">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c3f4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9c3f4-115">Parent elements</span></span>

|<span data-ttu-id="9c3f4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9c3f4-116">**Element**</span></span>|<span data-ttu-id="9c3f4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9c3f4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c3f4-118">календаритем</span><span class="sxs-lookup"><span data-stu-id="9c3f4-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9c3f4-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c3f4-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9c3f4-120">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="9c3f4-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9c3f4-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c3f4-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9c3f4-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="9c3f4-122">Remarks</span></span>

<span data-ttu-id="9c3f4-123">Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.</span><span class="sxs-lookup"><span data-stu-id="9c3f4-123">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="9c3f4-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9c3f4-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c3f4-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9c3f4-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c3f4-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9c3f4-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c3f4-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9c3f4-127">Schema name</span></span>  <br/> |<span data-ttu-id="9c3f4-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9c3f4-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c3f4-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9c3f4-129">Validation file</span></span>  <br/> |<span data-ttu-id="9c3f4-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9c3f4-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c3f4-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9c3f4-131">Can be empty</span></span>  <br/> |<span data-ttu-id="9c3f4-132">False</span><span class="sxs-lookup"><span data-stu-id="9c3f4-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c3f4-133">См. также</span><span class="sxs-lookup"><span data-stu-id="9c3f4-133">See also</span></span>



- [<span data-ttu-id="9c3f4-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9c3f4-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

