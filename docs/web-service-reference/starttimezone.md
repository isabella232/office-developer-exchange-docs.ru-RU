---
title: StartTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeZone
api_type:
- schema
ms.assetid: d38c4dc1-4ecb-42a1-8d57-a451b16a2de2
description: Элемент StartTimeZone определяет часовой пояс для времени начала Календаритем или свойство meetingrequest.
ms.openlocfilehash: fa88f676c0f6a7a2e934f51274942ed3bccbc789
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458525"
---
# <a name="starttimezone"></a><span data-ttu-id="a17d1-103">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="a17d1-103">StartTimeZone</span></span>

<span data-ttu-id="a17d1-104">Элемент **StartTimeZone** определяет часовой пояс для времени начала [календаритем](calendaritem.md) или [свойство meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="a17d1-104">The **StartTimeZone** element defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<StartTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</StartTimeZone>
```

<span data-ttu-id="a17d1-105">**тимезонедефинитионтипе**</span><span class="sxs-lookup"><span data-stu-id="a17d1-105">**TimeZoneDefinitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a17d1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a17d1-106">Attributes and elements</span></span>

<span data-ttu-id="a17d1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a17d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a17d1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a17d1-108">Attributes</span></span>

|<span data-ttu-id="a17d1-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a17d1-109">**Attribute**</span></span>|<span data-ttu-id="a17d1-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a17d1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a17d1-111">Id</span><span class="sxs-lookup"><span data-stu-id="a17d1-111">Id</span></span>  <br/> |<span data-ttu-id="a17d1-112">Представляет уникальный идентификатор определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a17d1-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="a17d1-113">Имя</span><span class="sxs-lookup"><span data-stu-id="a17d1-113">Name</span></span>  <br/> |<span data-ttu-id="a17d1-114">Представляет описательное имя определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a17d1-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a17d1-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a17d1-115">Child elements</span></span>

|<span data-ttu-id="a17d1-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a17d1-116">**Element**</span></span>|<span data-ttu-id="a17d1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a17d1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a17d1-118">Periods</span><span class="sxs-lookup"><span data-stu-id="a17d1-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="a17d1-119">Представляет массив элементов [period](period.md) , определяющий смещение времени на разных стадиях часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a17d1-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="a17d1-120">транситионсграупс</span><span class="sxs-lookup"><span data-stu-id="a17d1-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="a17d1-121">Представляет массив элементов [транситионсграуп](transitionsgroup.md) , определяющих переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a17d1-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="a17d1-122">Выполняет</span><span class="sxs-lookup"><span data-stu-id="a17d1-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="a17d1-123">Представляет массив переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a17d1-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a17d1-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a17d1-124">Parent elements</span></span>

|<span data-ttu-id="a17d1-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a17d1-125">**Element**</span></span>|<span data-ttu-id="a17d1-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a17d1-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a17d1-127">календаритем</span><span class="sxs-lookup"><span data-stu-id="a17d1-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a17d1-128">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="a17d1-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a17d1-129">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="a17d1-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a17d1-130">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a17d1-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a17d1-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="a17d1-131">Remarks</span></span>

<span data-ttu-id="a17d1-132">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a17d1-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a17d1-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a17d1-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a17d1-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a17d1-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a17d1-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a17d1-135">Schema Name</span></span>  <br/> |<span data-ttu-id="a17d1-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a17d1-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="a17d1-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a17d1-137">Validation File</span></span>  <br/> |<span data-ttu-id="a17d1-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a17d1-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a17d1-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a17d1-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="a17d1-140">False</span><span class="sxs-lookup"><span data-stu-id="a17d1-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a17d1-141">См. также</span><span class="sxs-lookup"><span data-stu-id="a17d1-141">See also</span></span>

- [<span data-ttu-id="a17d1-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a17d1-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

