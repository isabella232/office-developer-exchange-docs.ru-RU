---
title: AssociatedCalendarItemId
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
description: Элемент AssociatedCalendarItemId представляет элемента календаря, который связан с MeetingMessage, MeetingRequest, MeetingResponse, MeetingCancellation или ReminderMessageData.
ms.openlocfilehash: 4445da88d6fec42c1e02cd8de4d2e423485a4472
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761506"
---
# <a name="associatedcalendaritemid"></a><span data-ttu-id="7eaf3-103">AssociatedCalendarItemId</span><span class="sxs-lookup"><span data-stu-id="7eaf3-103">AssociatedCalendarItemId</span></span>

<span data-ttu-id="7eaf3-104">Элемент **AssociatedCalendarItemId** представляет элемента календаря, который связан с [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md)или [ReminderMessageData](remindermessagedata.md).</span><span class="sxs-lookup"><span data-stu-id="7eaf3-104">The **AssociatedCalendarItemId** element represents the calendar item that is associated with a [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md), or [ReminderMessageData](remindermessagedata.md).</span></span>
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="7eaf3-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="7eaf3-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7eaf3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7eaf3-106">Attributes and elements</span></span>

<span data-ttu-id="7eaf3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7eaf3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7eaf3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7eaf3-108">Attributes</span></span>

|<span data-ttu-id="7eaf3-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7eaf3-109">**Attribute**</span></span>|<span data-ttu-id="7eaf3-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7eaf3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7eaf3-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="7eaf3-111">**Id**</span></span> <br/> |<span data-ttu-id="7eaf3-112">Определяет элемент календаря, который связан с собрания.</span><span class="sxs-lookup"><span data-stu-id="7eaf3-112">Identifies the calendar item that is associated with meeting.</span></span>  <br/> |
|<span data-ttu-id="7eaf3-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="7eaf3-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="7eaf3-114">Идентифицирует определенной версии элемента календаря, который связан с собрания.</span><span class="sxs-lookup"><span data-stu-id="7eaf3-114">Identifies a specific version of the calendar item that is associated with a meeting.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7eaf3-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7eaf3-115">Child elements</span></span>

<span data-ttu-id="7eaf3-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="7eaf3-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7eaf3-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7eaf3-117">Parent elements</span></span>

<span data-ttu-id="7eaf3-118">[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)</span><span class="sxs-lookup"><span data-stu-id="7eaf3-118">[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7eaf3-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="7eaf3-119">Remarks</span></span>

<span data-ttu-id="7eaf3-120">Версии Exchange, начиная с номер сборки 15.00.0913.09 может включать элемент **AssociatedCalendarItemId** как дочерний элемент элемента **ReminderMessageData** .</span><span class="sxs-lookup"><span data-stu-id="7eaf3-120">Versions of Exchange starting with build number 15.00.0913.09 can include the **AssociatedCalendarItemId** element as a child element of the **ReminderMessageData** element.</span></span> 
  
<span data-ttu-id="7eaf3-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7eaf3-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7eaf3-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7eaf3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7eaf3-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7eaf3-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7eaf3-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7eaf3-124">Schema Name</span></span>  <br/> |<span data-ttu-id="7eaf3-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7eaf3-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7eaf3-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7eaf3-126">Validation File</span></span>  <br/> |<span data-ttu-id="7eaf3-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7eaf3-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7eaf3-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7eaf3-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="7eaf3-129">False</span><span class="sxs-lookup"><span data-stu-id="7eaf3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7eaf3-130">См. также</span><span class="sxs-lookup"><span data-stu-id="7eaf3-130">See also</span></span>

- [<span data-ttu-id="7eaf3-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7eaf3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

