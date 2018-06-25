---
title: MailboxData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxData
api_type:
- schema
ms.assetid: e9e3f50c-5a7b-49c7-a9ea-117959c08352
description: Элемент MailboxData представляет для отдельного почтового ящика пользователя и параметры для типа данных должно быть возвращено о пользователя почтового ящика.
ms.openlocfilehash: df60294e7d83b1459e5cca7d75c2b6b4bb9d931d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834281"
---
# <a name="mailboxdata"></a><span data-ttu-id="774f5-103">MailboxData</span><span class="sxs-lookup"><span data-stu-id="774f5-103">MailboxData</span></span>

<span data-ttu-id="774f5-104">Элемент **MailboxData** представляет для отдельного почтового ящика пользователя и параметры для типа данных должно быть возвращено о пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="774f5-104">The **MailboxData** element represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span> 
  
- [<span data-ttu-id="774f5-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="774f5-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="774f5-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="774f5-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="774f5-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="774f5-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

<span data-ttu-id="774f5-108">**MailboxData**</span><span class="sxs-lookup"><span data-stu-id="774f5-108">**MailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="774f5-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="774f5-109">Attributes and elements</span></span>

<span data-ttu-id="774f5-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="774f5-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="774f5-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="774f5-111">Attributes</span></span>

<span data-ttu-id="774f5-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="774f5-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="774f5-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="774f5-113">Child elements</span></span>

|<span data-ttu-id="774f5-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="774f5-114">**Element**</span></span>|<span data-ttu-id="774f5-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="774f5-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="774f5-116">Электронной почты (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="774f5-116">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="774f5-117">Представляет пользователя почтового ящика для запроса GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="774f5-117">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> |
|[<span data-ttu-id="774f5-118">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="774f5-118">AttendeeType</span></span>](attendeetype.md) <br/> |<span data-ttu-id="774f5-119">Представляет тип участника, обнаруженных в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="774f5-119">Represents the type of attendee identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="774f5-120">Используется в запросах для предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="774f5-120">This is used in requests for meeting suggestions.</span></span>  <br/> |
|[<span data-ttu-id="774f5-121">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="774f5-121">ExcludeConflicts</span></span>](excludeconflicts.md) <br/> |<span data-ttu-id="774f5-122">Указывает, нужно ли возвращать предложенного времени для время календаря, конфликтующие среди участников.</span><span class="sxs-lookup"><span data-stu-id="774f5-122">Specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="774f5-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="774f5-123">Parent elements</span></span>

|<span data-ttu-id="774f5-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="774f5-124">**Element**</span></span>|<span data-ttu-id="774f5-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="774f5-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="774f5-126">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="774f5-126">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="774f5-127">Содержит список почтовых ящиков для запроса сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="774f5-127">Contains a list of mailboxes to query for availability information.</span></span>  <br/> <span data-ttu-id="774f5-128">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="774f5-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="774f5-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="774f5-129">Remarks</span></span>

<span data-ttu-id="774f5-130">Клиентское приложение можно определить один ко многим элементам **MailboxData** .</span><span class="sxs-lookup"><span data-stu-id="774f5-130">A client application can define one to many **MailboxData** elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="774f5-131">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="774f5-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="774f5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="774f5-132">Example</span></span>

```xml
<MailboxDataArray>
  <MailboxData xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
    <Email>
      <Name></Name>
      <Address>someone@ExServer.example.com</Address>
      <RoutingType>SMTP</RoutingType>
    </Email>
    <AttendeeType>Organizer</AttendeeType>
    <ExcludeConflicts>false</ExcludeConflicts>
  </MailboxData>
</MailboxDataArray>
```

## <a name="element-information"></a><span data-ttu-id="774f5-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="774f5-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="774f5-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="774f5-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="774f5-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="774f5-135">Schema Name</span></span>  <br/> |<span data-ttu-id="774f5-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="774f5-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="774f5-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="774f5-137">Validation File</span></span>  <br/> |<span data-ttu-id="774f5-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="774f5-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="774f5-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="774f5-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="774f5-140">False</span><span class="sxs-lookup"><span data-stu-id="774f5-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="774f5-141">См. также</span><span class="sxs-lookup"><span data-stu-id="774f5-141">See also</span></span>

- [<span data-ttu-id="774f5-142">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="774f5-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="774f5-143">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="774f5-143">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="774f5-144">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="774f5-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

