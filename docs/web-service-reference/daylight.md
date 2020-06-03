---
title: Переход
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: Элемент "лето" представляет дату и время изменения времени со стандартного времени на летнее.
ms.openlocfilehash: bf2041cb4677f837ddb5b399041f1c19a7b5f577
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457461"
---
# <a name="daylight"></a><span data-ttu-id="a7db7-103">Переход</span><span class="sxs-lookup"><span data-stu-id="a7db7-103">Daylight</span></span>

<span data-ttu-id="a7db7-104">Элемент " **лето** " представляет дату и время изменения времени со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="a7db7-104">The **Daylight** element represents the date and time when the time changes from standard time to daylight saving time.</span></span> 
  
```xml
<Daylight TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Daylight>
```

```xml
<Daylight TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Daylight>
```

<span data-ttu-id="a7db7-105">**тимечанжетипе**</span><span class="sxs-lookup"><span data-stu-id="a7db7-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a7db7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a7db7-106">Attributes and elements</span></span>

<span data-ttu-id="a7db7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a7db7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7db7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a7db7-108">Attributes</span></span>

|<span data-ttu-id="a7db7-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a7db7-109">**Attribute**</span></span>|<span data-ttu-id="a7db7-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7db7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7db7-111">**тимезоненаме**</span><span class="sxs-lookup"><span data-stu-id="a7db7-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="a7db7-112">Описывает имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a7db7-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a7db7-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a7db7-113">Child elements</span></span>

|<span data-ttu-id="a7db7-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a7db7-114">**Element**</span></span>|<span data-ttu-id="a7db7-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7db7-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7db7-116">Offset</span><span class="sxs-lookup"><span data-stu-id="a7db7-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="a7db7-117">Описывает смещение от [басеоффсет](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="a7db7-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="a7db7-118">Основное смещение в дополнение к этому смещению определяет время в зависимости от того, является ли оно стандартным или летним.</span><span class="sxs-lookup"><span data-stu-id="a7db7-118">The base offset in addition to this offset identifies the time according to whether it is standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="a7db7-119">релативэйеарлирекурренце</span><span class="sxs-lookup"><span data-stu-id="a7db7-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="a7db7-120">Описывает относительный ежегодный шаблон повторения для шаблона даты перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a7db7-120">Describes a relative yearly recurrence pattern for a time zone transition date pattern.</span></span>  <br/> |
|[<span data-ttu-id="a7db7-121">абсолутедате</span><span class="sxs-lookup"><span data-stu-id="a7db7-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="a7db7-122">Представляет дату, когда время изменяется со стандартного или летнего времени.</span><span class="sxs-lookup"><span data-stu-id="a7db7-122">Represents the date when the time changes from standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="a7db7-123">Время (Тимечанжетипе)</span><span class="sxs-lookup"><span data-stu-id="a7db7-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="a7db7-124">Описывает время, по истечении которого время меняется со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="a7db7-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a7db7-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a7db7-125">Parent elements</span></span>

|<span data-ttu-id="a7db7-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a7db7-126">**Element**</span></span>|<span data-ttu-id="a7db7-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7db7-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7db7-128">митингтимезоне</span><span class="sxs-lookup"><span data-stu-id="a7db7-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="a7db7-129">Представляет часовой пояс для расположения, в котором размещается собрание.</span><span class="sxs-lookup"><span data-stu-id="a7db7-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a7db7-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="a7db7-130">Remarks</span></span>

<span data-ttu-id="a7db7-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a7db7-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7db7-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a7db7-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7db7-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a7db7-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7db7-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a7db7-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a7db7-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a7db7-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7db7-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a7db7-136">Validation File</span></span>  <br/> |<span data-ttu-id="a7db7-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a7db7-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7db7-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a7db7-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7db7-139">False</span><span class="sxs-lookup"><span data-stu-id="a7db7-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7db7-140">См. также</span><span class="sxs-lookup"><span data-stu-id="a7db7-140">See also</span></span>

- [<span data-ttu-id="a7db7-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a7db7-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

