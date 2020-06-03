---
title: Standard
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: Стандартный элемент представляет дату и время изменения времени с летнего на стандартное время.
ms.openlocfilehash: 1214a1debb53c9a31ca7c92a0c9e5c0722960d75
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467566"
---
# <a name="standard"></a><span data-ttu-id="20a85-103">Standard</span><span class="sxs-lookup"><span data-stu-id="20a85-103">Standard</span></span>

<span data-ttu-id="20a85-104">**Стандартный** элемент представляет дату и время изменения времени с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="20a85-104">The **Standard** element represents the date and time when the time changes from daylight saving time to standard time.</span></span> 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

```xml
<Standard TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Standard>
```

<span data-ttu-id="20a85-105">**тимечанжетипе**</span><span class="sxs-lookup"><span data-stu-id="20a85-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="20a85-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="20a85-106">Attributes and elements</span></span>

<span data-ttu-id="20a85-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="20a85-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20a85-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="20a85-108">Attributes</span></span>

|<span data-ttu-id="20a85-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="20a85-109">**Attribute**</span></span>|<span data-ttu-id="20a85-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="20a85-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="20a85-111">**тимезоненаме**</span><span class="sxs-lookup"><span data-stu-id="20a85-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="20a85-112">Описывает имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="20a85-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="20a85-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="20a85-113">Child elements</span></span>

|<span data-ttu-id="20a85-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="20a85-114">**Element**</span></span>|<span data-ttu-id="20a85-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="20a85-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20a85-116">Offset</span><span class="sxs-lookup"><span data-stu-id="20a85-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="20a85-117">Описывает смещение от [басеоффсет](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="20a85-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="20a85-118">В сочетании с элементом **басеоффсет** элемент **offset** определяет, является ли время стандартным или летним.</span><span class="sxs-lookup"><span data-stu-id="20a85-118">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="20a85-119">релативэйеарлирекурренце</span><span class="sxs-lookup"><span data-stu-id="20a85-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="20a85-120">Описывает относительный ежегодный шаблон повторения для даты смены часового пояса.</span><span class="sxs-lookup"><span data-stu-id="20a85-120">Describes a relative yearly recurrence pattern for a time zone transition date.</span></span>  <br/> |
|[<span data-ttu-id="20a85-121">абсолутедате</span><span class="sxs-lookup"><span data-stu-id="20a85-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="20a85-122">Представляет дату, когда время изменяется со стандартного или летнего времени.</span><span class="sxs-lookup"><span data-stu-id="20a85-122">Represents the date when the time changes from standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="20a85-123">Время (Тимечанжетипе)</span><span class="sxs-lookup"><span data-stu-id="20a85-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="20a85-124">Описывает время, по истечении которого время меняется со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="20a85-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20a85-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="20a85-125">Parent elements</span></span>

|<span data-ttu-id="20a85-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="20a85-126">**Element**</span></span>|<span data-ttu-id="20a85-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="20a85-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20a85-128">митингтимезоне</span><span class="sxs-lookup"><span data-stu-id="20a85-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="20a85-129">Представляет часовой пояс для расположения, в котором размещается собрание.</span><span class="sxs-lookup"><span data-stu-id="20a85-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="20a85-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="20a85-130">Remarks</span></span>

<span data-ttu-id="20a85-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="20a85-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20a85-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="20a85-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20a85-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="20a85-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="20a85-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="20a85-134">Schema Name</span></span>  <br/> |<span data-ttu-id="20a85-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="20a85-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="20a85-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="20a85-136">Validation File</span></span>  <br/> |<span data-ttu-id="20a85-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="20a85-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="20a85-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="20a85-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="20a85-139">False</span><span class="sxs-lookup"><span data-stu-id="20a85-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20a85-140">См. также</span><span class="sxs-lookup"><span data-stu-id="20a85-140">See also</span></span>

- [<span data-ttu-id="20a85-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="20a85-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

