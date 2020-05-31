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
ms.openlocfilehash: bc186170ccca06669ea7d20cea06c542f9ce274a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761478"
---
# <a name="appointmentsequencenumber"></a><span data-ttu-id="2df1c-103">аппоинтментсекуенценумбер</span><span class="sxs-lookup"><span data-stu-id="2df1c-103">AppointmentSequenceNumber</span></span>

<span data-ttu-id="2df1c-104">Элемент **аппоинтментсекуенценумбер** указывает порядковый номер версии встречи.</span><span class="sxs-lookup"><span data-stu-id="2df1c-104">The **AppointmentSequenceNumber** element specifies the sequence number of a version of an appointment.</span></span> 
  
```xml
<AppointmentSequenceNumber/>
```

 <span data-ttu-id="2df1c-105">**int**</span><span class="sxs-lookup"><span data-stu-id="2df1c-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2df1c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2df1c-106">Attributes and elements</span></span>

<span data-ttu-id="2df1c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2df1c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2df1c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2df1c-108">Attributes</span></span>

<span data-ttu-id="2df1c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2df1c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2df1c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2df1c-110">Child elements</span></span>

<span data-ttu-id="2df1c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2df1c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2df1c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2df1c-112">Parent elements</span></span>

|<span data-ttu-id="2df1c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2df1c-113">**Element**</span></span>|<span data-ttu-id="2df1c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2df1c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2df1c-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="2df1c-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2df1c-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="2df1c-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2df1c-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="2df1c-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2df1c-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2df1c-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2df1c-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2df1c-119">Text value</span></span>

<span data-ttu-id="2df1c-120">Текстовое значение представляет номер версии.</span><span class="sxs-lookup"><span data-stu-id="2df1c-120">The text value represents a version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2df1c-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="2df1c-121">Remarks</span></span>

<span data-ttu-id="2df1c-122">Это значение обновляется при обновлении встречи с новыми сведениями.</span><span class="sxs-lookup"><span data-stu-id="2df1c-122">This value is updated when the appointment is updated with new information.</span></span> 
  
<span data-ttu-id="2df1c-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2df1c-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2df1c-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2df1c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2df1c-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2df1c-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2df1c-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2df1c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="2df1c-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2df1c-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="2df1c-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2df1c-128">Validation File</span></span>  <br/> |<span data-ttu-id="2df1c-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2df1c-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2df1c-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2df1c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="2df1c-131">False</span><span class="sxs-lookup"><span data-stu-id="2df1c-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2df1c-132">См. также</span><span class="sxs-lookup"><span data-stu-id="2df1c-132">See also</span></span>

- [<span data-ttu-id="2df1c-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2df1c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

