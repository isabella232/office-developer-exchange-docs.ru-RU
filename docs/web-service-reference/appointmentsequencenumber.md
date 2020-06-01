---
title: аппоинтментсекуенценумбер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentSequenceNumber
api_type:
- schema
ms.assetid: eb4c48bd-f905-48dc-ae16-53a080b9b025
description: Элемент Аппоинтментсекуенценумбер указывает порядковый номер версии встречи.
ms.openlocfilehash: daeea7a656c59923bcb6f2850539c7869d6eb181
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461662"
---
# <a name="appointmentsequencenumber"></a><span data-ttu-id="e2bc8-103">аппоинтментсекуенценумбер</span><span class="sxs-lookup"><span data-stu-id="e2bc8-103">AppointmentSequenceNumber</span></span>

<span data-ttu-id="e2bc8-104">Элемент **аппоинтментсекуенценумбер** указывает порядковый номер версии встречи.</span><span class="sxs-lookup"><span data-stu-id="e2bc8-104">The **AppointmentSequenceNumber** element specifies the sequence number of a version of an appointment.</span></span> 
  
```xml
<AppointmentSequenceNumber/>
```

 <span data-ttu-id="e2bc8-105">**int**</span><span class="sxs-lookup"><span data-stu-id="e2bc8-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2bc8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e2bc8-106">Attributes and elements</span></span>

<span data-ttu-id="e2bc8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e2bc8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2bc8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e2bc8-108">Attributes</span></span>

<span data-ttu-id="e2bc8-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e2bc8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2bc8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e2bc8-110">Child elements</span></span>

<span data-ttu-id="e2bc8-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e2bc8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e2bc8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e2bc8-112">Parent elements</span></span>

|<span data-ttu-id="e2bc8-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e2bc8-113">**Element**</span></span>|<span data-ttu-id="e2bc8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e2bc8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2bc8-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="e2bc8-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e2bc8-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2bc8-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e2bc8-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="e2bc8-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e2bc8-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2bc8-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e2bc8-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e2bc8-119">Text value</span></span>

<span data-ttu-id="e2bc8-120">Текстовое значение представляет номер версии.</span><span class="sxs-lookup"><span data-stu-id="e2bc8-120">The text value represents a version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2bc8-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="e2bc8-121">Remarks</span></span>

<span data-ttu-id="e2bc8-122">Это значение обновляется при обновлении встречи с новыми сведениями.</span><span class="sxs-lookup"><span data-stu-id="e2bc8-122">This value is updated when the appointment is updated with new information.</span></span> 
  
<span data-ttu-id="e2bc8-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e2bc8-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2bc8-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e2bc8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2bc8-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e2bc8-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2bc8-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e2bc8-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e2bc8-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e2bc8-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2bc8-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e2bc8-128">Validation File</span></span>  <br/> |<span data-ttu-id="e2bc8-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e2bc8-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2bc8-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e2bc8-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2bc8-131">False</span><span class="sxs-lookup"><span data-stu-id="e2bc8-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2bc8-132">См. также</span><span class="sxs-lookup"><span data-stu-id="e2bc8-132">See also</span></span>

- [<span data-ttu-id="e2bc8-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e2bc8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

