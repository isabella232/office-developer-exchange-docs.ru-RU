---
title: EndTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTimeZone
api_type:
- schema
ms.assetid: 6c53c337-be60-4d22-9e9e-a0c140c5e913
description: Элемент EndTimeZone определяет часовой пояс для времени окончания Календаритем или свойство meetingrequest.
ms.openlocfilehash: 65eeedcc7c4d0e616ae54d4e2545fd310e9ad905
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762357"
---
# <a name="endtimezone"></a><span data-ttu-id="22eb0-103">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="22eb0-103">EndTimeZone</span></span>

<span data-ttu-id="22eb0-104">Элемент **EndTimeZone** определяет часовой пояс для времени окончания [календаритем](calendaritem.md) или [свойство meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="22eb0-104">The **EndTimeZone** element defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<EndTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</EndTimeZone>
```

 <span data-ttu-id="22eb0-105">**тимезонедефинитионтипе**</span><span class="sxs-lookup"><span data-stu-id="22eb0-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22eb0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="22eb0-106">Attributes and elements</span></span>

<span data-ttu-id="22eb0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="22eb0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22eb0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="22eb0-108">Attributes</span></span>

|<span data-ttu-id="22eb0-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="22eb0-109">**Attribute**</span></span>|<span data-ttu-id="22eb0-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22eb0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="22eb0-111">Id</span><span class="sxs-lookup"><span data-stu-id="22eb0-111">Id</span></span>  <br/> |<span data-ttu-id="22eb0-112">Представляет уникальный идентификатор определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="22eb0-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="22eb0-113">Имя</span><span class="sxs-lookup"><span data-stu-id="22eb0-113">Name</span></span>  <br/> |<span data-ttu-id="22eb0-114">Представляет описательное имя определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="22eb0-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="22eb0-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="22eb0-115">Child elements</span></span>

|<span data-ttu-id="22eb0-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="22eb0-116">**Element**</span></span>|<span data-ttu-id="22eb0-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22eb0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22eb0-118">Periods</span><span class="sxs-lookup"><span data-stu-id="22eb0-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="22eb0-119">Представляет массив элементов [period](period.md) , определяющий смещение времени на разных стадиях часового пояса.</span><span class="sxs-lookup"><span data-stu-id="22eb0-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="22eb0-120">транситионсграупс</span><span class="sxs-lookup"><span data-stu-id="22eb0-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="22eb0-121">Представляет массив элементов [транситионсграуп](transitionsgroup.md) , определяющих переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="22eb0-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="22eb0-122">Выполняет</span><span class="sxs-lookup"><span data-stu-id="22eb0-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="22eb0-123">Представляет массив переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="22eb0-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22eb0-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="22eb0-124">Parent elements</span></span>

|<span data-ttu-id="22eb0-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="22eb0-125">**Element**</span></span>|<span data-ttu-id="22eb0-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22eb0-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22eb0-127">календаритем</span><span class="sxs-lookup"><span data-stu-id="22eb0-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="22eb0-128">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="22eb0-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="22eb0-129">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="22eb0-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="22eb0-130">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="22eb0-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="22eb0-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="22eb0-131">Remarks</span></span>

<span data-ttu-id="22eb0-132">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="22eb0-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22eb0-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="22eb0-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22eb0-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="22eb0-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22eb0-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="22eb0-135">Schema Name</span></span>  <br/> |<span data-ttu-id="22eb0-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="22eb0-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="22eb0-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="22eb0-137">Validation File</span></span>  <br/> |<span data-ttu-id="22eb0-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="22eb0-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="22eb0-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="22eb0-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="22eb0-140">False</span><span class="sxs-lookup"><span data-stu-id="22eb0-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22eb0-141">См. также</span><span class="sxs-lookup"><span data-stu-id="22eb0-141">See also</span></span>



- [<span data-ttu-id="22eb0-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="22eb0-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

