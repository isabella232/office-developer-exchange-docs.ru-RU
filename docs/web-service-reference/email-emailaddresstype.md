---
title: Электронной почты (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Email
api_type:
- schema
ms.assetid: dfffa1d5-2c3c-4f56-af63-5853df462e58
description: Элемент Email представляет пользователя почтового ящика для запроса GetUserAvailability.
ms.openlocfilehash: 0e7848d7c4f5001ed86b06d11af1d7623b4bf1f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762269"
---
# <a name="email-emailaddresstype"></a><span data-ttu-id="2ecf8-103">Электронной почты (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2ecf8-103">Email (EmailAddressType)</span></span>

<span data-ttu-id="2ecf8-104">Элемент **Email** представляет пользователя почтового ящика для запроса GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-104">The **Email** element represents the mailbox user for a GetUserAvailability query.</span></span> 
  
- [<span data-ttu-id="2ecf8-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="2ecf8-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)  
- [<span data-ttu-id="2ecf8-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="2ecf8-106">MailboxDataArray</span></span>](mailboxdataarray.md) 
- [<span data-ttu-id="2ecf8-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="2ecf8-107">MailboxData</span></span>](mailboxdata.md) 
- [<span data-ttu-id="2ecf8-108">Электронной почты (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2ecf8-108">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 <span data-ttu-id="2ecf8-109">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="2ecf8-109">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ecf8-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2ecf8-110">Attributes and elements</span></span>

<span data-ttu-id="2ecf8-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ecf8-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2ecf8-112">Attributes</span></span>

<span data-ttu-id="2ecf8-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ecf8-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2ecf8-114">Child elements</span></span>

|<span data-ttu-id="2ecf8-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2ecf8-115">**Element**</span></span>|<span data-ttu-id="2ecf8-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2ecf8-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ecf8-117">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2ecf8-117">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="2ecf8-118">Представляет отображаемое имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-118">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="2ecf8-119">Адрес (строка)</span><span class="sxs-lookup"><span data-stu-id="2ecf8-119">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="2ecf8-120">Представляет адрес электронной почты пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-120">Represents the e-mail address of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="2ecf8-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2ecf8-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="2ecf8-122">Представляет протокол маршрутизации для сообщения.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-122">Represents the routing protocol for the message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2ecf8-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2ecf8-123">Parent elements</span></span>

|<span data-ttu-id="2ecf8-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2ecf8-124">**Element**</span></span>|<span data-ttu-id="2ecf8-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2ecf8-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ecf8-126">MailboxData</span><span class="sxs-lookup"><span data-stu-id="2ecf8-126">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="2ecf8-127">Представляет отдельного пользователя почтового ящика и параметры возвращаемого типа данных об этом пользователе.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-127">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="2ecf8-128">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="2ecf8-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2ecf8-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="2ecf8-129">Remarks</span></span>

<span data-ttu-id="2ecf8-130">Схема с описанием этого элемента находится в каталоге /EWS/ на компьютере, на котором запущено приложение MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-130">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ecf8-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2ecf8-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ecf8-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2ecf8-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ecf8-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2ecf8-133">Schema Name</span></span>  <br/> |<span data-ttu-id="2ecf8-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2ecf8-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ecf8-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2ecf8-135">Validation File</span></span>  <br/> |<span data-ttu-id="2ecf8-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2ecf8-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ecf8-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2ecf8-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ecf8-138">False</span><span class="sxs-lookup"><span data-stu-id="2ecf8-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ecf8-139">См. также</span><span class="sxs-lookup"><span data-stu-id="2ecf8-139">See also</span></span>

- [<span data-ttu-id="2ecf8-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2ecf8-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="2ecf8-141">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="2ecf8-141">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="2ecf8-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="2ecf8-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

