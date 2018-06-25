---
title: AdjacentMeetings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdjacentMeetings
api_type:
- schema
ms.assetid: 50a9c381-9166-476e-8421-29e51b94499b
description: Элемент AdjacentMeetings определяет все элементы календаря, расположенных на время собрания.
ms.openlocfilehash: 9ab818f4f67c32c01101cc595ccb92424a872ef0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761360"
---
# <a name="adjacentmeetings"></a><span data-ttu-id="3c961-103">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="3c961-103">AdjacentMeetings</span></span>

<span data-ttu-id="3c961-104">Элемент **AdjacentMeetings** определяет все элементы календаря, расположенных на время собрания.</span><span class="sxs-lookup"><span data-stu-id="3c961-104">The **AdjacentMeetings** element identifies all calendar items that are adjacent to a meeting time.</span></span> 
  
```xml
<AdjacentMeetings>
   <CalendarItem/>
</AdjacentMeetings>
```

 <span data-ttu-id="3c961-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="3c961-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c961-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3c961-106">Attributes and elements</span></span>

<span data-ttu-id="3c961-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3c961-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c961-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3c961-108">Attributes</span></span>

<span data-ttu-id="3c961-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3c961-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c961-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3c961-110">Child elements</span></span>

|<span data-ttu-id="3c961-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3c961-111">**Element**</span></span>|<span data-ttu-id="3c961-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3c961-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c961-113">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="3c961-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3c961-114">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c961-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c961-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3c961-115">Parent elements</span></span>

|<span data-ttu-id="3c961-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3c961-116">**Element**</span></span>|<span data-ttu-id="3c961-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3c961-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c961-118">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="3c961-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3c961-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c961-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3c961-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3c961-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3c961-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c961-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3c961-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="3c961-122">Remarks</span></span>

<span data-ttu-id="3c961-123">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3c961-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="3c961-124">Несмотря на то, что дополнительные дочерние элементы являются допустимыми в схеме, [элемента календаря, имеющего](calendaritem.md) элемент является единственным дочерний элемент, который возвращает веб-служб Exchange (EWS) в элементе **AdjacentMeetings** .</span><span class="sxs-lookup"><span data-stu-id="3c961-124">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **AdjacentMeetings** element.</span></span> <span data-ttu-id="3c961-125">В этом разделе не позволяет отобразить список дочерних элементов, которые являются допустимыми в схеме, но не будут получены с веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c961-125">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="3c961-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3c961-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c961-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3c961-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c961-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3c961-128">Schema Name</span></span>  <br/> |<span data-ttu-id="3c961-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3c961-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c961-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3c961-130">Validation File</span></span>  <br/> |<span data-ttu-id="3c961-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3c961-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c961-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3c961-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c961-133">False</span><span class="sxs-lookup"><span data-stu-id="3c961-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c961-134">См. также</span><span class="sxs-lookup"><span data-stu-id="3c961-134">See also</span></span>

- [<span data-ttu-id="3c961-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3c961-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

