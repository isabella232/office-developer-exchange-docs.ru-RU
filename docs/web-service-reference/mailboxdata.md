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
description: Элемент MailboxData представляет отдельного пользователя почтового ящика и параметры для типа возвращаемых данных о пользователе почтового ящика.
ms.openlocfilehash: df60294e7d83b1459e5cca7d75c2b6b4bb9d931d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834281"
---
# <a name="mailboxdata"></a><span data-ttu-id="0e27f-103">MailboxData</span><span class="sxs-lookup"><span data-stu-id="0e27f-103">MailboxData</span></span>

<span data-ttu-id="0e27f-104">Элемент **MailboxData** представляет отдельного пользователя почтового ящика и параметры для типа возвращаемых данных о пользователе почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="0e27f-104">The **MailboxData** element represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span> 
  
- [<span data-ttu-id="0e27f-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="0e27f-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="0e27f-106">маилбоксдатааррай</span><span class="sxs-lookup"><span data-stu-id="0e27f-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="0e27f-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="0e27f-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

<span data-ttu-id="0e27f-108">**MailboxData**</span><span class="sxs-lookup"><span data-stu-id="0e27f-108">**MailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0e27f-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0e27f-109">Attributes and elements</span></span>

<span data-ttu-id="0e27f-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0e27f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e27f-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0e27f-111">Attributes</span></span>

<span data-ttu-id="0e27f-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="0e27f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e27f-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0e27f-113">Child elements</span></span>

|<span data-ttu-id="0e27f-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0e27f-114">**Element**</span></span>|<span data-ttu-id="0e27f-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0e27f-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e27f-116">Электронная почта (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="0e27f-116">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="0e27f-117">Представляет пользователя почтового ящика для запроса GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="0e27f-117">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> |
|[<span data-ttu-id="0e27f-118">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="0e27f-118">AttendeeType</span></span>](attendeetype.md) <br/> |<span data-ttu-id="0e27f-119">Представляет тип участника, идентифицированного в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="0e27f-119">Represents the type of attendee identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="0e27f-120">Используется в запросах предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="0e27f-120">This is used in requests for meeting suggestions.</span></span>  <br/> |
|[<span data-ttu-id="0e27f-121">ексклудеконфликтс</span><span class="sxs-lookup"><span data-stu-id="0e27f-121">ExcludeConflicts</span></span>](excludeconflicts.md) <br/> |<span data-ttu-id="0e27f-122">Указывает, следует ли возвращать предлагаемые времена для календарных ситуаций, в которых возникает конфликт между участниками.</span><span class="sxs-lookup"><span data-stu-id="0e27f-122">Specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0e27f-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0e27f-123">Parent elements</span></span>

|<span data-ttu-id="0e27f-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0e27f-124">**Element**</span></span>|<span data-ttu-id="0e27f-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0e27f-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e27f-126">маилбоксдатааррай</span><span class="sxs-lookup"><span data-stu-id="0e27f-126">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="0e27f-127">Содержит список почтовых ящиков, в которых запрашиваются сведения о доступности.</span><span class="sxs-lookup"><span data-stu-id="0e27f-127">Contains a list of mailboxes to query for availability information.</span></span>  <br/> <span data-ttu-id="0e27f-128">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="0e27f-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0e27f-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="0e27f-129">Remarks</span></span>

<span data-ttu-id="0e27f-130">Клиентское приложение может определять один или несколько элементов **MailboxData** .</span><span class="sxs-lookup"><span data-stu-id="0e27f-130">A client application can define one to many **MailboxData** elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0e27f-131">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server 2007 с ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0e27f-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="0e27f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0e27f-132">Example</span></span>

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

## <a name="element-information"></a><span data-ttu-id="0e27f-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0e27f-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e27f-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0e27f-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e27f-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0e27f-135">Schema Name</span></span>  <br/> |<span data-ttu-id="0e27f-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0e27f-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e27f-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0e27f-137">Validation File</span></span>  <br/> |<span data-ttu-id="0e27f-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0e27f-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e27f-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0e27f-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e27f-140">False</span><span class="sxs-lookup"><span data-stu-id="0e27f-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e27f-141">См. также</span><span class="sxs-lookup"><span data-stu-id="0e27f-141">See also</span></span>

- [<span data-ttu-id="0e27f-142">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0e27f-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="0e27f-143">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="0e27f-143">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="0e27f-144">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="0e27f-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

