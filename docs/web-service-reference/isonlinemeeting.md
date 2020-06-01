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
ms.openlocfilehash: d2d60c8a51ad7e03c33b57709d9173e79d162268
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460402"
---
# <a name="isonlinemeeting"></a><span data-ttu-id="a8af8-103">исонлинемитинг</span><span class="sxs-lookup"><span data-stu-id="a8af8-103">IsOnlineMeeting</span></span>

<span data-ttu-id="a8af8-104">Элемент **исонлинемитинг** указывает, находится ли собрание в сети.</span><span class="sxs-lookup"><span data-stu-id="a8af8-104">The **IsOnlineMeeting** element indicates whether the meeting is online.</span></span> 
  
```xml
<IsOnlineMeeting/>
```

 <span data-ttu-id="a8af8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a8af8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8af8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a8af8-106">Attributes and elements</span></span>

<span data-ttu-id="a8af8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a8af8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8af8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a8af8-108">Attributes</span></span>

<span data-ttu-id="a8af8-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a8af8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8af8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a8af8-110">Child elements</span></span>

<span data-ttu-id="a8af8-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a8af8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8af8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a8af8-112">Parent elements</span></span>

|<span data-ttu-id="a8af8-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a8af8-113">**Element**</span></span>|<span data-ttu-id="a8af8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a8af8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8af8-115">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="a8af8-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a8af8-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8af8-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a8af8-117">календаритем</span><span class="sxs-lookup"><span data-stu-id="a8af8-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a8af8-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8af8-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8af8-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a8af8-119">Text value</span></span>

<span data-ttu-id="a8af8-120">При использовании этого элемента необходимо указать текстовое значение, представляющее логическое значение.</span><span class="sxs-lookup"><span data-stu-id="a8af8-120">A text value that represents a Boolean value is required if this element is used.</span></span> <span data-ttu-id="a8af8-121">Значение **true** указывает, что собрание находится в сети.</span><span class="sxs-lookup"><span data-stu-id="a8af8-121">A value of **true** indicates that the meeting is online.</span></span> <span data-ttu-id="a8af8-122">Значение **false** указывает, что собрание находится не в сети.</span><span class="sxs-lookup"><span data-stu-id="a8af8-122">A value of **false** indicates that the meeting is not online.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a8af8-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="a8af8-123">Remarks</span></span>

<span data-ttu-id="a8af8-124">Свойство Исонлинемитинг доступно для записи в элементе календаря организатора.</span><span class="sxs-lookup"><span data-stu-id="a8af8-124">The IsOnlineMeeting property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="a8af8-125">Он доступен только для чтения для приглашений на собрания и элементов календаря участников.</span><span class="sxs-lookup"><span data-stu-id="a8af8-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="a8af8-126">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Майкрософт Exchange 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a8af8-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8af8-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a8af8-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8af8-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a8af8-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8af8-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a8af8-129">Schema name</span></span>  <br/> |<span data-ttu-id="a8af8-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a8af8-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8af8-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a8af8-131">Validation file</span></span>  <br/> |<span data-ttu-id="a8af8-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a8af8-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8af8-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a8af8-133">Can be empty</span></span>  <br/> |<span data-ttu-id="a8af8-134">False</span><span class="sxs-lookup"><span data-stu-id="a8af8-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8af8-135">См. также</span><span class="sxs-lookup"><span data-stu-id="a8af8-135">See also</span></span>



- [<span data-ttu-id="a8af8-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a8af8-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

