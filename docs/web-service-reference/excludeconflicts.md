---
title: ексклудеконфликтс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExcludeConflicts
api_type:
- schema
ms.assetid: ec33ef23-8537-41eb-8d89-7eb906a1fad7
description: Элемент Ексклудеконфликтс указывает, следует ли возвращать предлагаемые моменты времени для конфликтов между участниками.
ms.openlocfilehash: d20c594ae600abf110681ea678b2d95a23bf7809
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456978"
---
# <a name="excludeconflicts"></a><span data-ttu-id="d3d21-103">ексклудеконфликтс</span><span class="sxs-lookup"><span data-stu-id="d3d21-103">ExcludeConflicts</span></span>

<span data-ttu-id="d3d21-104">Элемент **ексклудеконфликтс** указывает, следует ли возвращать предлагаемые моменты времени для конфликтов между участниками.</span><span class="sxs-lookup"><span data-stu-id="d3d21-104">The **ExcludeConflicts** element specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span> 
  
[<span data-ttu-id="d3d21-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="d3d21-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="d3d21-106">маилбоксдатааррай</span><span class="sxs-lookup"><span data-stu-id="d3d21-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
[<span data-ttu-id="d3d21-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="d3d21-107">MailboxData</span></span>](mailboxdata.md)
  
[<span data-ttu-id="d3d21-108">ексклудеконфликтс</span><span class="sxs-lookup"><span data-stu-id="d3d21-108">ExcludeConflicts</span></span>](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
```

 <span data-ttu-id="d3d21-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d3d21-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3d21-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d3d21-110">Attributes and elements</span></span>

<span data-ttu-id="d3d21-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d3d21-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3d21-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d3d21-112">Attributes</span></span>

<span data-ttu-id="d3d21-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d3d21-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3d21-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d3d21-114">Child elements</span></span>

<span data-ttu-id="d3d21-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d3d21-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d3d21-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d3d21-116">Parent elements</span></span>

|<span data-ttu-id="d3d21-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3d21-117">**Element**</span></span>|<span data-ttu-id="d3d21-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3d21-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3d21-119">MailboxData</span><span class="sxs-lookup"><span data-stu-id="d3d21-119">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="d3d21-120">Представляет отдельного пользователя почтового ящика и параметры возвращаемого типа данных об этом пользователе.</span><span class="sxs-lookup"><span data-stu-id="d3d21-120">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="d3d21-121">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="d3d21-121">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3d21-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d3d21-122">Text value</span></span>

<span data-ttu-id="d3d21-123">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="d3d21-123">A text value is required.</span></span> <span data-ttu-id="d3d21-124">Возможные значения: Boolean **true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="d3d21-124">The possible values are a Boolean **true** or **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d3d21-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="d3d21-125">Remarks</span></span>

<span data-ttu-id="d3d21-126">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3d21-126">This element is required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="d3d21-127">Схема с описанием этого элемента находится в каталоге /EWS/ на компьютере, на котором запущено приложение MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d3d21-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d3d21-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d3d21-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3d21-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d3d21-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3d21-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d3d21-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d3d21-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d3d21-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3d21-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d3d21-132">Validation File</span></span>  <br/> |<span data-ttu-id="d3d21-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d3d21-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3d21-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d3d21-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3d21-135">False</span><span class="sxs-lookup"><span data-stu-id="d3d21-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3d21-136">См. также</span><span class="sxs-lookup"><span data-stu-id="d3d21-136">See also</span></span>



[<span data-ttu-id="d3d21-137">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d3d21-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d3d21-138">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="d3d21-138">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="d3d21-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="d3d21-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

