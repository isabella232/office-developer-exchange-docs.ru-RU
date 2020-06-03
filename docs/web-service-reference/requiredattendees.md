---
title: RequiredAttendees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequiredAttendees
api_type:
- schema
ms.assetid: 422f8d44-b0eb-49ca-af0f-0e22b54c78d2
description: Элемент RequiredAttendees представляет участников, которые необходимы для участия в собрании.
ms.openlocfilehash: a67800687f24dc323c3d80e4166ca9dd34dfc4fc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468294"
---
# <a name="requiredattendees"></a><span data-ttu-id="e64fe-103">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="e64fe-103">RequiredAttendees</span></span>

<span data-ttu-id="e64fe-104">Элемент **RequiredAttendees** представляет участников, которые необходимы для участия в собрании.</span><span class="sxs-lookup"><span data-stu-id="e64fe-104">The **RequiredAttendees** element represents attendees that are required to attend a meeting.</span></span> 
  
```xml
<RequiredAttendees>
   <Attendee/>
</RequiredAttendees>
```

 <span data-ttu-id="e64fe-105">**нонемптяррайофаттендистипе**</span><span class="sxs-lookup"><span data-stu-id="e64fe-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e64fe-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e64fe-106">Attributes and elements</span></span>

<span data-ttu-id="e64fe-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e64fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e64fe-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e64fe-108">Attributes</span></span>

<span data-ttu-id="e64fe-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e64fe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e64fe-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e64fe-110">Child elements</span></span>

|<span data-ttu-id="e64fe-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e64fe-111">**Element**</span></span>|<span data-ttu-id="e64fe-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e64fe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e64fe-113">Участник</span><span class="sxs-lookup"><span data-stu-id="e64fe-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="e64fe-114">Представляет участников и ресурсы собрания.</span><span class="sxs-lookup"><span data-stu-id="e64fe-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e64fe-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e64fe-115">Parent elements</span></span>

|<span data-ttu-id="e64fe-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e64fe-116">**Element**</span></span>|<span data-ttu-id="e64fe-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e64fe-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e64fe-118">календаритем</span><span class="sxs-lookup"><span data-stu-id="e64fe-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e64fe-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="e64fe-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e64fe-120">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="e64fe-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e64fe-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e64fe-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e64fe-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="e64fe-122">Remarks</span></span>

<span data-ttu-id="e64fe-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e64fe-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e64fe-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e64fe-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e64fe-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e64fe-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e64fe-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e64fe-126">Schema name</span></span>  <br/> |<span data-ttu-id="e64fe-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e64fe-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="e64fe-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e64fe-128">Validation file</span></span>  <br/> |<span data-ttu-id="e64fe-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e64fe-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e64fe-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e64fe-130">Can be empty</span></span>  <br/> |<span data-ttu-id="e64fe-131">False</span><span class="sxs-lookup"><span data-stu-id="e64fe-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e64fe-132">См. также</span><span class="sxs-lookup"><span data-stu-id="e64fe-132">See also</span></span>



- [<span data-ttu-id="e64fe-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e64fe-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

