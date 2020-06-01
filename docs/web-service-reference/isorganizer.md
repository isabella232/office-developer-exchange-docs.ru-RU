---
title: Подорганизатор
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a31ac268-5061-4272-a433-ffaea2fbcfa9
description: Элемент, который указывает, является ли этот пользователь организатором собрания.
ms.openlocfilehash: 45b7a66068dc00f6e60b7380240bea6836282fd4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466565"
---
# <a name="isorganizer"></a><span data-ttu-id="25646-103">Подорганизатор</span><span class="sxs-lookup"><span data-stu-id="25646-103">IsOrganizer</span></span>

<span data-ttu-id="25646-104">Элемент **, который указывает** , является ли этот пользователь организатором собрания.</span><span class="sxs-lookup"><span data-stu-id="25646-104">The **IsOrganizer** element specifies a Boolean value that indicates whether this person is the organizer of the meeting.</span></span> 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
```

 <span data-ttu-id="25646-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="25646-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25646-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="25646-106">Attributes and elements</span></span>

<span data-ttu-id="25646-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="25646-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25646-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="25646-108">Attributes</span></span>

<span data-ttu-id="25646-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="25646-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25646-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="25646-110">Child elements</span></span>

<span data-ttu-id="25646-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="25646-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25646-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="25646-112">Parent elements</span></span>

|<span data-ttu-id="25646-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25646-113">**Element**</span></span>|<span data-ttu-id="25646-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25646-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25646-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="25646-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="25646-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="25646-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="25646-117">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="25646-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="25646-118">Представляет сообщение о собрании.</span><span class="sxs-lookup"><span data-stu-id="25646-118">Represents a meeting message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25646-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="25646-119">Text value</span></span>

<span data-ttu-id="25646-120">Текстовое значение **true** для **элемента "," указывает** на то, что пользователь создал элемент календаря или сообщение о собрании.</span><span class="sxs-lookup"><span data-stu-id="25646-120">A text value of **true** for the **IsOrganizer** element indicates that the calendar item or meeting message was created by the user.</span></span> <span data-ttu-id="25646-121">Значение **false** указывает, что элемент календаря или сообщение о собрании не были созданы БВ пользователем.</span><span class="sxs-lookup"><span data-stu-id="25646-121">A value of **false** indicates that the calendar item or meeting message was not created bv the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="25646-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="25646-122">Remarks</span></span>

<span data-ttu-id="25646-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="25646-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="25646-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="25646-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25646-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="25646-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25646-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="25646-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25646-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="25646-127">Schema Name</span></span>  <br/> |<span data-ttu-id="25646-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="25646-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="25646-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="25646-129">Validation File</span></span>  <br/> |<span data-ttu-id="25646-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="25646-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="25646-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="25646-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="25646-132">См. также</span><span class="sxs-lookup"><span data-stu-id="25646-132">See also</span></span>



- [<span data-ttu-id="25646-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="25646-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

