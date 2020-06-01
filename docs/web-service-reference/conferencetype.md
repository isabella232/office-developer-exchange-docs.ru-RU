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
ms.openlocfilehash: 482fc09d709e2b151b255107af59cb98de236aec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463932"
---
# <a name="conferencetype"></a><span data-ttu-id="8b6bc-103">конференцетипе</span><span class="sxs-lookup"><span data-stu-id="8b6bc-103">ConferenceType</span></span>

<span data-ttu-id="8b6bc-104">Элемент **конференцетипе** описывает тип конференций, который выполняется с элементом календаря.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-104">The **ConferenceType** element describes the type of conferencing that is performed with a calendar item.</span></span> 
  
```xml
<ConferenceType/>
```

 <span data-ttu-id="8b6bc-105">**int**</span><span class="sxs-lookup"><span data-stu-id="8b6bc-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b6bc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8b6bc-106">Attributes and elements</span></span>

<span data-ttu-id="8b6bc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b6bc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8b6bc-108">Attributes</span></span>

<span data-ttu-id="8b6bc-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b6bc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8b6bc-110">Child elements</span></span>

<span data-ttu-id="8b6bc-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b6bc-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8b6bc-112">Parent elements</span></span>

|<span data-ttu-id="8b6bc-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b6bc-113">**Element**</span></span>|<span data-ttu-id="8b6bc-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b6bc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b6bc-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="8b6bc-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8b6bc-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8b6bc-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="8b6bc-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8b6bc-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8b6bc-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8b6bc-119">Text value</span></span>

<span data-ttu-id="8b6bc-120">При использовании этого элемента необходимо указать текстовое значение, представляющее целое значение.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-120">A text value that represents an integer value is required if this element is used.</span></span> <span data-ttu-id="8b6bc-121">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="8b6bc-122">0 = NetMeeting</span><span class="sxs-lookup"><span data-stu-id="8b6bc-122">0 = NetMeeting</span></span>
    
- <span data-ttu-id="8b6bc-123">1 = NetShow</span><span class="sxs-lookup"><span data-stu-id="8b6bc-123">1 = NetShow</span></span>
    
- <span data-ttu-id="8b6bc-124">2 = чат</span><span class="sxs-lookup"><span data-stu-id="8b6bc-124">2 = Chat</span></span>
    
## <a name="remarks"></a><span data-ttu-id="8b6bc-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="8b6bc-125">Remarks</span></span>

<span data-ttu-id="8b6bc-126">Свойство **митингворкспацеурл** доступно для записи в элементе календаря организатора.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-126">The **MeetingWorkspaceUrl** property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="8b6bc-127">Он доступен только для чтения для приглашений на собрания и элементов календаря участника.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-127">It is read-only for meeting requests and for attendee's calendar items.</span></span> 
  
<span data-ttu-id="8b6bc-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8b6bc-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8b6bc-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8b6bc-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b6bc-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8b6bc-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b6bc-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8b6bc-131">Schema Name</span></span>  <br/> |<span data-ttu-id="8b6bc-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8b6bc-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b6bc-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8b6bc-133">Validation File</span></span>  <br/> |<span data-ttu-id="8b6bc-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8b6bc-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b6bc-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8b6bc-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b6bc-136">False</span><span class="sxs-lookup"><span data-stu-id="8b6bc-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b6bc-137">См. также</span><span class="sxs-lookup"><span data-stu-id="8b6bc-137">See also</span></span>



- [<span data-ttu-id="8b6bc-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8b6bc-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

