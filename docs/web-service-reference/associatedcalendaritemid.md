---
title: ассоЦиатедкалендаритемид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssociatedCalendarItemId
api_type:
- schema
ms.assetid: 5b29898c-ea59-4e6a-914c-c011ec754032
description: Элемент АссоЦиатедкалендаритемид представляет элемент календаря, связанный с Митингмессаже, свойство meetingrequest, Митингреспонсе, Митингканцеллатион или Реминдермессажедата.
ms.openlocfilehash: 816372c38243ba0fe5a7606c264dd1c5107350f2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460885"
---
# <a name="associatedcalendaritemid"></a><span data-ttu-id="c6ec4-103">ассоЦиатедкалендаритемид</span><span class="sxs-lookup"><span data-stu-id="c6ec4-103">AssociatedCalendarItemId</span></span>

<span data-ttu-id="c6ec4-104">Элемент **ассоЦиатедкалендаритемид** представляет элемент календаря, связанный с [митингмессаже](meetingmessage.md), [свойство meetingrequest](meetingrequest.md), [митингреспонсе](meetingresponse.md), [митингканцеллатион](meetingcancellation.md)или [реминдермессажедата](remindermessagedata.md).</span><span class="sxs-lookup"><span data-stu-id="c6ec4-104">The **AssociatedCalendarItemId** element represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md), or [ReminderMessageData](remindermessagedata.md).</span></span>
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="c6ec4-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="c6ec4-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6ec4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c6ec4-106">Attributes and elements</span></span>

<span data-ttu-id="c6ec4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c6ec4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6ec4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c6ec4-108">Attributes</span></span>

|<span data-ttu-id="c6ec4-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="c6ec4-109">**Attribute**</span></span>|<span data-ttu-id="c6ec4-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c6ec4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c6ec4-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="c6ec4-111">**Id**</span></span> <br/> |<span data-ttu-id="c6ec4-112">Определяет элемент календаря, связанный с собранием.</span><span class="sxs-lookup"><span data-stu-id="c6ec4-112">Identifies the calendar item that is associated with meeting.</span></span>  <br/> |
|<span data-ttu-id="c6ec4-113">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="c6ec4-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="c6ec4-114">Определяет конкретную версию элемента календаря, связанную с собранием.</span><span class="sxs-lookup"><span data-stu-id="c6ec4-114">Identifies a specific version of the calendar item that is associated with a meeting.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c6ec4-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c6ec4-115">Child elements</span></span>

<span data-ttu-id="c6ec4-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c6ec4-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c6ec4-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c6ec4-117">Parent elements</span></span>

<span data-ttu-id="c6ec4-118">[Митингмессаже](meetingmessage.md)  |  [Свойство meetingrequest](meetingrequest.md)  |  [Митингреспонсе](meetingresponse.md)  |  [Митингканцеллатион](meetingcancellation.md)  |  [Реминдермессажедата](remindermessagedata.md)</span><span class="sxs-lookup"><span data-stu-id="c6ec4-118">[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c6ec4-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="c6ec4-119">Remarks</span></span>

<span data-ttu-id="c6ec4-120">Версии Exchange, начинающиеся с номера сборки 15.00.0913.09, могут включать элемент **ассоЦиатедкалендаритемид** в качестве дочернего элемента элемента **реминдермессажедата** .</span><span class="sxs-lookup"><span data-stu-id="c6ec4-120">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
<span data-ttu-id="c6ec4-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6ec4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6ec4-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c6ec4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6ec4-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c6ec4-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c6ec4-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c6ec4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c6ec4-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c6ec4-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c6ec4-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c6ec4-126">Validation File</span></span>  <br/> |<span data-ttu-id="c6ec4-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c6ec4-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c6ec4-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c6ec4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6ec4-129">False</span><span class="sxs-lookup"><span data-stu-id="c6ec4-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6ec4-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c6ec4-130">See also</span></span>

- [<span data-ttu-id="c6ec4-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c6ec4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

