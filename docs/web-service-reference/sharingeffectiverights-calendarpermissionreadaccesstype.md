---
title: Шаринжеффективеригхтс (Календарпермиссионреадакцесстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: b519f642-a9ef-4300-92e6-ed8202855fde
description: Элемент Шаринжеффективеригхтс указывает разрешения, которые есть у пользователя для данных календаря, к которым предоставлен доступ.
ms.openlocfilehash: 5581e9cc001608a124ae94e69eba836f6fd98520
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458581"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a><span data-ttu-id="75bd3-103">Шаринжеффективеригхтс (Календарпермиссионреадакцесстипе)</span><span class="sxs-lookup"><span data-stu-id="75bd3-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>

<span data-ttu-id="75bd3-104">Элемент **шаринжеффективеригхтс** указывает разрешения, которые есть у пользователя для данных календаря, к которым предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="75bd3-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the calendar data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 <span data-ttu-id="75bd3-105">**календарпермиссионреадакцесстипе**</span><span class="sxs-lookup"><span data-stu-id="75bd3-105">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75bd3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="75bd3-106">Attributes and elements</span></span>

<span data-ttu-id="75bd3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="75bd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75bd3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="75bd3-108">Attributes</span></span>

<span data-ttu-id="75bd3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="75bd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75bd3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="75bd3-110">Child elements</span></span>

<span data-ttu-id="75bd3-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="75bd3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75bd3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="75bd3-112">Parent elements</span></span>

|<span data-ttu-id="75bd3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="75bd3-113">**Element**</span></span>|<span data-ttu-id="75bd3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="75bd3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75bd3-115">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="75bd3-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="75bd3-116">Представляет папку, в которой в основном содержатся элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="75bd3-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75bd3-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="75bd3-117">Text value</span></span>

<span data-ttu-id="75bd3-118">В следующей таблице приведены возможные значения для элемента **шаринжеффективеригхтс** .</span><span class="sxs-lookup"><span data-stu-id="75bd3-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
|<span data-ttu-id="75bd3-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="75bd3-119">**Value**</span></span>|<span data-ttu-id="75bd3-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="75bd3-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="75bd3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="75bd3-121">None</span></span>  <br/> |<span data-ttu-id="75bd3-122">Указывает, что у пользователя нет разрешения на просмотр элементов в календаре.</span><span class="sxs-lookup"><span data-stu-id="75bd3-122">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="75bd3-123">тимеонли</span><span class="sxs-lookup"><span data-stu-id="75bd3-123">TimeOnly</span></span>  <br/> |<span data-ttu-id="75bd3-124">Указывает, что у пользователя есть разрешение на просмотр сведений о занятости в календаре.</span><span class="sxs-lookup"><span data-stu-id="75bd3-124">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="75bd3-125">тимеандсубжектандлокатион</span><span class="sxs-lookup"><span data-stu-id="75bd3-125">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="75bd3-126">Указывает, что пользователь имеет разрешение на просмотр сведений о занятости в календаре и теме и местоположении встреч.</span><span class="sxs-lookup"><span data-stu-id="75bd3-126">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="75bd3-127">фуллдетаилс</span><span class="sxs-lookup"><span data-stu-id="75bd3-127">FullDetails</span></span>  <br/> |<span data-ttu-id="75bd3-128">Указывает, что у пользователя есть разрешение на просмотр всех элементов календаря, в том числе сведения о занятости, теме, местоположении и сведения о встречах.</span><span class="sxs-lookup"><span data-stu-id="75bd3-128">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="75bd3-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="75bd3-129">Remarks</span></span>

<span data-ttu-id="75bd3-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="75bd3-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75bd3-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="75bd3-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75bd3-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="75bd3-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75bd3-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="75bd3-133">Schema Name</span></span>  <br/> |<span data-ttu-id="75bd3-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="75bd3-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="75bd3-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="75bd3-135">Validation File</span></span>  <br/> |<span data-ttu-id="75bd3-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="75bd3-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="75bd3-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="75bd3-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="75bd3-138">False</span><span class="sxs-lookup"><span data-stu-id="75bd3-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75bd3-139">См. также</span><span class="sxs-lookup"><span data-stu-id="75bd3-139">See also</span></span>



- [<span data-ttu-id="75bd3-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="75bd3-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

