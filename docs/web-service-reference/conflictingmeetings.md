---
title: конфликтингмитингс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetings
api_type:
- schema
ms.assetid: cfff7a11-7b3a-4995-9815-afedd45ebb0f
description: Элемент Конфликтингмитингс определяет все элементы календаря, которые конфликтуют с временем собрания.
ms.openlocfilehash: dc897c9dc33117d379d89bb9bb41104ca02def1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460178"
---
# <a name="conflictingmeetings"></a><span data-ttu-id="e0e82-103">конфликтингмитингс</span><span class="sxs-lookup"><span data-stu-id="e0e82-103">ConflictingMeetings</span></span>

<span data-ttu-id="e0e82-104">Элемент **конфликтингмитингс** определяет все элементы календаря, которые конфликтуют с временем собрания.</span><span class="sxs-lookup"><span data-stu-id="e0e82-104">The **ConflictingMeetings** element identifies all calendar items that conflict with a meeting time.</span></span> 
  
```xml
<ConflictingMeetings>
   <CalendarItem/>
</ConflictingMeetings>
```

 <span data-ttu-id="e0e82-105">**нонемптяррайофаллитемстипе**</span><span class="sxs-lookup"><span data-stu-id="e0e82-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0e82-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e0e82-106">Attributes and elements</span></span>

<span data-ttu-id="e0e82-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e0e82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0e82-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e0e82-108">Attributes</span></span>

<span data-ttu-id="e0e82-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e0e82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e0e82-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e0e82-110">Child elements</span></span>

|<span data-ttu-id="e0e82-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e0e82-111">**Element**</span></span>|<span data-ttu-id="e0e82-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0e82-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0e82-113">календаритем</span><span class="sxs-lookup"><span data-stu-id="e0e82-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e0e82-114">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0e82-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e0e82-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e0e82-115">Parent elements</span></span>

|<span data-ttu-id="e0e82-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e0e82-116">**Element**</span></span>|<span data-ttu-id="e0e82-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0e82-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0e82-118">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="e0e82-118">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e0e82-119">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0e82-119">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e0e82-120">календаритем</span><span class="sxs-lookup"><span data-stu-id="e0e82-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e0e82-121">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0e82-121">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e0e82-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="e0e82-122">Remarks</span></span>

<span data-ttu-id="e0e82-123">Если этот элемент используется, он должен содержать один или несколько дочерних элементов.</span><span class="sxs-lookup"><span data-stu-id="e0e82-123">If this element is used, it must contain one or more child elements.</span></span>
  
<span data-ttu-id="e0e82-124">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e0e82-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e0e82-125">Несмотря на то что в схеме допустимы дополнительные дочерние элементы, элемент [календаритем](calendaritem.md) является единственным дочерним элементом, который веб-службы Exchange (EWS) будут возвращать в элементе **конфликтингмитингс** .</span><span class="sxs-lookup"><span data-stu-id="e0e82-125">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **ConflictingMeetings** element.</span></span> <span data-ttu-id="e0e82-126">В этой статье не перечислены дочерние элементы, допустимые для схемы, но не возвращенные службой EWS.</span><span class="sxs-lookup"><span data-stu-id="e0e82-126">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e0e82-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e0e82-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0e82-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e0e82-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0e82-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e0e82-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e0e82-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e0e82-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0e82-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e0e82-131">Validation File</span></span>  <br/> |<span data-ttu-id="e0e82-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e0e82-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0e82-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e0e82-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0e82-134">False</span><span class="sxs-lookup"><span data-stu-id="e0e82-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0e82-135">См. также</span><span class="sxs-lookup"><span data-stu-id="e0e82-135">See also</span></span>



- [<span data-ttu-id="e0e82-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e0e82-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

