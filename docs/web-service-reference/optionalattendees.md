---
title: OptionalAttendees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OptionalAttendees
api_type:
- schema
ms.assetid: e7c80c4d-3794-45e9-986f-6a8a687df0a4
description: Элемент OptionalAttendees представляет участников, которые не являются обязательными для участия в собрании.
ms.openlocfilehash: 9eeff7151042f26fe5b00b43ec16a27946680a9f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468175"
---
# <a name="optionalattendees"></a><span data-ttu-id="18a50-103">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="18a50-103">OptionalAttendees</span></span>

<span data-ttu-id="18a50-104">Элемент **OptionalAttendees** представляет участников, которые не являются обязательными для участия в собрании.</span><span class="sxs-lookup"><span data-stu-id="18a50-104">The **OptionalAttendees** element represents attendees who are not required to attend a meeting.</span></span> 
  
```xml
<OptionalAttendees>
   <Attendee/>
</OptionalAttendees>
```

 <span data-ttu-id="18a50-105">**нонемптяррайофаттендистипе**</span><span class="sxs-lookup"><span data-stu-id="18a50-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18a50-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="18a50-106">Attributes and elements</span></span>

<span data-ttu-id="18a50-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="18a50-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18a50-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="18a50-108">Attributes</span></span>

<span data-ttu-id="18a50-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="18a50-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18a50-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="18a50-110">Child elements</span></span>

|<span data-ttu-id="18a50-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="18a50-111">**Element**</span></span>|<span data-ttu-id="18a50-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="18a50-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18a50-113">Участник</span><span class="sxs-lookup"><span data-stu-id="18a50-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="18a50-114">Представляет участников и ресурсы собрания.</span><span class="sxs-lookup"><span data-stu-id="18a50-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18a50-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="18a50-115">Parent elements</span></span>

|<span data-ttu-id="18a50-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="18a50-116">**Element**</span></span>|<span data-ttu-id="18a50-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="18a50-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18a50-118">календаритем</span><span class="sxs-lookup"><span data-stu-id="18a50-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="18a50-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="18a50-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="18a50-120">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="18a50-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="18a50-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="18a50-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="18a50-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="18a50-122">Remarks</span></span>

<span data-ttu-id="18a50-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="18a50-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18a50-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="18a50-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18a50-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="18a50-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18a50-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="18a50-126">Schema name</span></span>  <br/> |<span data-ttu-id="18a50-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="18a50-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="18a50-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="18a50-128">Validation file</span></span>  <br/> |<span data-ttu-id="18a50-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="18a50-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18a50-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="18a50-130">Can be empty</span></span>  <br/> |<span data-ttu-id="18a50-131">False</span><span class="sxs-lookup"><span data-stu-id="18a50-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18a50-132">См. также</span><span class="sxs-lookup"><span data-stu-id="18a50-132">See also</span></span>



- [<span data-ttu-id="18a50-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="18a50-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

