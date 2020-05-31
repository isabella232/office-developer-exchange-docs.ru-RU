---
title: исонлинемитинг
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOnlineMeeting
api_type:
- schema
ms.assetid: c29df676-0f3a-4694-a42f-522c6d16872f
description: Элемент Исонлинемитинг указывает, находится ли собрание в сети.
ms.openlocfilehash: 5a56b0b9828d6f6bec83fc0ad0f8f9579b471a72
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834061"
---
# <a name="isonlinemeeting"></a><span data-ttu-id="5a86f-103">исонлинемитинг</span><span class="sxs-lookup"><span data-stu-id="5a86f-103">IsOnlineMeeting</span></span>

<span data-ttu-id="5a86f-104">Элемент **исонлинемитинг** указывает, находится ли собрание в сети.</span><span class="sxs-lookup"><span data-stu-id="5a86f-104">The **IsOnlineMeeting** element indicates whether the meeting is online.</span></span> 
  
```xml
<IsOnlineMeeting/>
```

 <span data-ttu-id="5a86f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5a86f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a86f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5a86f-106">Attributes and elements</span></span>

<span data-ttu-id="5a86f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5a86f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a86f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5a86f-108">Attributes</span></span>

<span data-ttu-id="5a86f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5a86f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a86f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5a86f-110">Child elements</span></span>

<span data-ttu-id="5a86f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5a86f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a86f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5a86f-112">Parent elements</span></span>

|<span data-ttu-id="5a86f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5a86f-113">**Element**</span></span>|<span data-ttu-id="5a86f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5a86f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a86f-115">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="5a86f-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5a86f-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a86f-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5a86f-117">календаритем</span><span class="sxs-lookup"><span data-stu-id="5a86f-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5a86f-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a86f-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a86f-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5a86f-119">Text value</span></span>

<span data-ttu-id="5a86f-120">При использовании этого элемента необходимо указать текстовое значение, представляющее логическое значение.</span><span class="sxs-lookup"><span data-stu-id="5a86f-120">A text value that represents a Boolean value is required if this element is used.</span></span> <span data-ttu-id="5a86f-121">Значение **true** указывает, что собрание находится в сети.</span><span class="sxs-lookup"><span data-stu-id="5a86f-121">A value of **true** indicates that the meeting is online.</span></span> <span data-ttu-id="5a86f-122">Значение **false** указывает, что собрание находится не в сети.</span><span class="sxs-lookup"><span data-stu-id="5a86f-122">A value of **false** indicates that the meeting is not online.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5a86f-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="5a86f-123">Remarks</span></span>

<span data-ttu-id="5a86f-124">Свойство Исонлинемитинг доступно для записи в элементе календаря организатора.</span><span class="sxs-lookup"><span data-stu-id="5a86f-124">The IsOnlineMeeting property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="5a86f-125">Он доступен только для чтения для приглашений на собрания и элементов календаря участников.</span><span class="sxs-lookup"><span data-stu-id="5a86f-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="5a86f-126">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Майкрософт Exchange 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5a86f-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a86f-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5a86f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a86f-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5a86f-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a86f-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5a86f-129">Schema name</span></span>  <br/> |<span data-ttu-id="5a86f-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5a86f-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a86f-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5a86f-131">Validation file</span></span>  <br/> |<span data-ttu-id="5a86f-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5a86f-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a86f-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5a86f-133">Can be empty</span></span>  <br/> |<span data-ttu-id="5a86f-134">False</span><span class="sxs-lookup"><span data-stu-id="5a86f-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a86f-135">См. также</span><span class="sxs-lookup"><span data-stu-id="5a86f-135">See also</span></span>



- [<span data-ttu-id="5a86f-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5a86f-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

