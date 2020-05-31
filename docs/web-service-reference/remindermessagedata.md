---
title: реминдермессажедата
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04dd4987-baaf-4ebe-ae58-ad962c2f8fa1
description: Элемент Реминдермессажедата указывает данные в сообщении с напоминанием.
ms.openlocfilehash: a1d01dd24030b047bd8ad025f3e1cebed0da8e29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835067"
---
# <a name="remindermessagedata"></a><span data-ttu-id="fd6d0-103">реминдермессажедата</span><span class="sxs-lookup"><span data-stu-id="fd6d0-103">ReminderMessageData</span></span>

<span data-ttu-id="fd6d0-104">Элемент **реминдермессажедата** указывает данные в сообщении с напоминанием.</span><span class="sxs-lookup"><span data-stu-id="fd6d0-104">The **ReminderMessageData** element specifies the data in a reminder message.</span></span> 
  
```XML
<ReminderMessageData>
   <ReminderText></ReminderText>
   <Location></Location>
   <StartTime></StartTime>
   <EndTime></EndTime>
   <AssociatedCalendarItemId></AssociatedCalendarItemId>
</ReminderMessageData>

```

 <span data-ttu-id="fd6d0-105">**реминдермессажедататипе**</span><span class="sxs-lookup"><span data-stu-id="fd6d0-105">**ReminderMessageDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd6d0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fd6d0-106">Attributes and elements</span></span>

<span data-ttu-id="fd6d0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fd6d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd6d0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fd6d0-108">Attributes</span></span>

<span data-ttu-id="fd6d0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fd6d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd6d0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fd6d0-110">Child elements</span></span>

<span data-ttu-id="fd6d0-111">[Реминдертекст](remindertext.md) | [Location](location.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md) [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md)(реминдермессажедататипе) время окончания (реминдермессажедататипе) ассоЦиатедкалендаритемид | </span><span class="sxs-lookup"><span data-stu-id="fd6d0-111">[ReminderText](remindertext.md) | [Location](location.md) | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [AssociatedCalendarItemId](associatedcalendaritemid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd6d0-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fd6d0-112">Parent elements</span></span>

[<span data-ttu-id="fd6d0-113">Сообщение</span><span class="sxs-lookup"><span data-stu-id="fd6d0-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="fd6d0-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="fd6d0-114">Remarks</span></span>

<span data-ttu-id="fd6d0-115">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="fd6d0-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="fd6d0-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd6d0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="fd6d0-117">Версии Exchange, начинающиеся с номера сборки 15.00.0913.09, могут включать элемент **ассоЦиатедкалендаритемид** в качестве дочернего элемента элемента **реминдермессажедата** .</span><span class="sxs-lookup"><span data-stu-id="fd6d0-117">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="fd6d0-118">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fd6d0-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd6d0-119">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fd6d0-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd6d0-120">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fd6d0-120">Schema Name</span></span>  <br/> |<span data-ttu-id="fd6d0-121">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fd6d0-121">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd6d0-122">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fd6d0-122">Validation File</span></span>  <br/> |<span data-ttu-id="fd6d0-123">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fd6d0-123">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd6d0-124">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fd6d0-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd6d0-125">True</span><span class="sxs-lookup"><span data-stu-id="fd6d0-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd6d0-126">См. также</span><span class="sxs-lookup"><span data-stu-id="fd6d0-126">See also</span></span>



[<span data-ttu-id="fd6d0-127">Сообщение</span><span class="sxs-lookup"><span data-stu-id="fd6d0-127">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="fd6d0-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fd6d0-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

