---
title: митингтимезоне
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTimeZone
api_type:
- schema
ms.assetid: 413b47d9-8126-462c-9a4f-4e771a5e8889
description: Элемент Митингтимезоне представляет часовой пояс для расположения, в котором размещается собрание.
ms.openlocfilehash: aef4ac4e7571ded6920cbaf90e2895d421068f55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465473"
---
# <a name="meetingtimezone"></a><span data-ttu-id="fec36-103">митингтимезоне</span><span class="sxs-lookup"><span data-stu-id="fec36-103">MeetingTimeZone</span></span>

<span data-ttu-id="fec36-104">Элемент **митингтимезоне** представляет часовой пояс для расположения, в котором размещается собрание.</span><span class="sxs-lookup"><span data-stu-id="fec36-104">The **MeetingTimeZone** element represents the time zone of the location where the meeting is hosted.</span></span> 
  
```xml
<MeetingTimeZone>
   <BaseOffset/>
   <Standard/>
   <Daylight/>
</MeetingTimeZone>
```

 <span data-ttu-id="fec36-105">**тимезонетипе**</span><span class="sxs-lookup"><span data-stu-id="fec36-105">**TimeZoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fec36-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fec36-106">Attributes and elements</span></span>

<span data-ttu-id="fec36-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fec36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fec36-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fec36-108">Attributes</span></span>

|<span data-ttu-id="fec36-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="fec36-109">**Attribute**</span></span>|<span data-ttu-id="fec36-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fec36-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fec36-111">**тимезоненаме**</span><span class="sxs-lookup"><span data-stu-id="fec36-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="fec36-112">Описывает имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="fec36-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fec36-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fec36-113">Child elements</span></span>

|<span data-ttu-id="fec36-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fec36-114">**Element**</span></span>|<span data-ttu-id="fec36-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fec36-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fec36-116">басеоффсет</span><span class="sxs-lookup"><span data-stu-id="fec36-116">BaseOffset</span></span>](baseoffset.md) <br/> |<span data-ttu-id="fec36-117">Представляет почасовое смещение от времени в формате UTC для текущего часового пояса.</span><span class="sxs-lookup"><span data-stu-id="fec36-117">Represents the hourly offset from UTC for the current time zone.</span></span>  <br/> |
|[<span data-ttu-id="fec36-118">Standard</span><span class="sxs-lookup"><span data-stu-id="fec36-118">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="fec36-119">Представляет дату и время изменения времени с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="fec36-119">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="fec36-120">Переход</span><span class="sxs-lookup"><span data-stu-id="fec36-120">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="fec36-121">Представляет дату и время изменения времени со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="fec36-121">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fec36-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fec36-122">Parent elements</span></span>

|<span data-ttu-id="fec36-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fec36-123">**Element**</span></span>|<span data-ttu-id="fec36-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fec36-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fec36-125">календаритем</span><span class="sxs-lookup"><span data-stu-id="fec36-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="fec36-126">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="fec36-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="fec36-127">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="fec36-127">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="fec36-128">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fec36-128">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fec36-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="fec36-129">Remarks</span></span>

<span data-ttu-id="fec36-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fec36-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fec36-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fec36-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fec36-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fec36-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fec36-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fec36-133">Schema Name</span></span>  <br/> |<span data-ttu-id="fec36-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fec36-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="fec36-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fec36-135">Validation File</span></span>  <br/> |<span data-ttu-id="fec36-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fec36-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fec36-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fec36-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="fec36-138">False</span><span class="sxs-lookup"><span data-stu-id="fec36-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fec36-139">См. также</span><span class="sxs-lookup"><span data-stu-id="fec36-139">See also</span></span>



- [<span data-ttu-id="fec36-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fec36-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

