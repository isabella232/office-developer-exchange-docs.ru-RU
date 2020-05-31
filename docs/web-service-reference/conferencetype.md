---
title: конференцетипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConferenceType
api_type:
- schema
ms.assetid: 6bcf6c18-2695-44b1-aabe-dadc52b2633a
description: Элемент Конференцетипе описывает тип конференций, который выполняется с элементом календаря.
ms.openlocfilehash: d312420606c5e1914fe321ae7c7c512f0833199c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761706"
---
# <a name="conferencetype"></a><span data-ttu-id="9d1d6-103">конференцетипе</span><span class="sxs-lookup"><span data-stu-id="9d1d6-103">ConferenceType</span></span>

<span data-ttu-id="9d1d6-104">Элемент **конференцетипе** описывает тип конференций, который выполняется с элементом календаря.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-104">The **ConferenceType** element describes the type of conferencing that is performed with a calendar item.</span></span> 
  
```xml
<ConferenceType/>
```

 <span data-ttu-id="9d1d6-105">**int**</span><span class="sxs-lookup"><span data-stu-id="9d1d6-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d1d6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9d1d6-106">Attributes and elements</span></span>

<span data-ttu-id="9d1d6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d1d6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9d1d6-108">Attributes</span></span>

<span data-ttu-id="9d1d6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d1d6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9d1d6-110">Child elements</span></span>

<span data-ttu-id="9d1d6-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d1d6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9d1d6-112">Parent elements</span></span>

|<span data-ttu-id="9d1d6-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9d1d6-113">**Element**</span></span>|<span data-ttu-id="9d1d6-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9d1d6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d1d6-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="9d1d6-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9d1d6-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9d1d6-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="9d1d6-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9d1d6-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d1d6-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9d1d6-119">Text value</span></span>

<span data-ttu-id="9d1d6-120">При использовании этого элемента необходимо указать текстовое значение, представляющее целое значение.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-120">A text value that represents an integer value is required if this element is used.</span></span> <span data-ttu-id="9d1d6-121">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="9d1d6-122">0 = NetMeeting</span><span class="sxs-lookup"><span data-stu-id="9d1d6-122">0 = NetMeeting</span></span>
    
- <span data-ttu-id="9d1d6-123">1 = NetShow</span><span class="sxs-lookup"><span data-stu-id="9d1d6-123">1 = NetShow</span></span>
    
- <span data-ttu-id="9d1d6-124">2 = чат</span><span class="sxs-lookup"><span data-stu-id="9d1d6-124">2 = Chat</span></span>
    
## <a name="remarks"></a><span data-ttu-id="9d1d6-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="9d1d6-125">Remarks</span></span>

<span data-ttu-id="9d1d6-126">Свойство **митингворкспацеурл** доступно для записи в элементе календаря организатора.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-126">The **MeetingWorkspaceUrl** property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="9d1d6-127">Он доступен только для чтения для приглашений на собрания и элементов календаря участника.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-127">It is read-only for meeting requests and for attendee's calendar items.</span></span> 
  
<span data-ttu-id="9d1d6-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9d1d6-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9d1d6-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9d1d6-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d1d6-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9d1d6-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d1d6-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9d1d6-131">Schema Name</span></span>  <br/> |<span data-ttu-id="9d1d6-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9d1d6-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d1d6-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9d1d6-133">Validation File</span></span>  <br/> |<span data-ttu-id="9d1d6-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9d1d6-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d1d6-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9d1d6-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d1d6-136">False</span><span class="sxs-lookup"><span data-stu-id="9d1d6-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d1d6-137">См. также</span><span class="sxs-lookup"><span data-stu-id="9d1d6-137">See also</span></span>



- [<span data-ttu-id="9d1d6-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9d1d6-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

