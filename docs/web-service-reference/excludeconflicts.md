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
ms.openlocfilehash: 66b69d57246942e551de2f683949870823e2e4e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762418"
---
# <a name="excludeconflicts"></a><span data-ttu-id="58ae4-103">ексклудеконфликтс</span><span class="sxs-lookup"><span data-stu-id="58ae4-103">ExcludeConflicts</span></span>

<span data-ttu-id="58ae4-104">Элемент **ексклудеконфликтс** указывает, следует ли возвращать предлагаемые моменты времени для конфликтов между участниками.</span><span class="sxs-lookup"><span data-stu-id="58ae4-104">The **ExcludeConflicts** element specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span> 
  
[<span data-ttu-id="58ae4-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="58ae4-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="58ae4-106">маилбоксдатааррай</span><span class="sxs-lookup"><span data-stu-id="58ae4-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
[<span data-ttu-id="58ae4-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="58ae4-107">MailboxData</span></span>](mailboxdata.md)
  
[<span data-ttu-id="58ae4-108">ексклудеконфликтс</span><span class="sxs-lookup"><span data-stu-id="58ae4-108">ExcludeConflicts</span></span>](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
```

 <span data-ttu-id="58ae4-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="58ae4-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58ae4-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="58ae4-110">Attributes and elements</span></span>

<span data-ttu-id="58ae4-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="58ae4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58ae4-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="58ae4-112">Attributes</span></span>

<span data-ttu-id="58ae4-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="58ae4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58ae4-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="58ae4-114">Child elements</span></span>

<span data-ttu-id="58ae4-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="58ae4-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="58ae4-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="58ae4-116">Parent elements</span></span>

|<span data-ttu-id="58ae4-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="58ae4-117">**Element**</span></span>|<span data-ttu-id="58ae4-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="58ae4-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58ae4-119">MailboxData</span><span class="sxs-lookup"><span data-stu-id="58ae4-119">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="58ae4-120">Представляет отдельного пользователя почтового ящика и параметры возвращаемого типа данных об этом пользователе.</span><span class="sxs-lookup"><span data-stu-id="58ae4-120">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="58ae4-121">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="58ae4-121">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="58ae4-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="58ae4-122">Text value</span></span>

<span data-ttu-id="58ae4-123">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="58ae4-123">A text value is required.</span></span> <span data-ttu-id="58ae4-124">Возможные значения: Boolean **true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="58ae4-124">The possible values are a Boolean **true** or **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="58ae4-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="58ae4-125">Remarks</span></span>

<span data-ttu-id="58ae4-126">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="58ae4-126">This element is required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="58ae4-127">Схема с описанием этого элемента находится в каталоге /EWS/ на компьютере, на котором запущено приложение MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="58ae4-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="58ae4-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="58ae4-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58ae4-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="58ae4-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58ae4-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="58ae4-130">Schema Name</span></span>  <br/> |<span data-ttu-id="58ae4-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="58ae4-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="58ae4-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="58ae4-132">Validation File</span></span>  <br/> |<span data-ttu-id="58ae4-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="58ae4-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58ae4-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="58ae4-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="58ae4-135">False</span><span class="sxs-lookup"><span data-stu-id="58ae4-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58ae4-136">См. также</span><span class="sxs-lookup"><span data-stu-id="58ae4-136">See also</span></span>



[<span data-ttu-id="58ae4-137">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="58ae4-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="58ae4-138">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="58ae4-138">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="58ae4-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="58ae4-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

