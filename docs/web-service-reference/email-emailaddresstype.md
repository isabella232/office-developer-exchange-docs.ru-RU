---
title: Электронная почта (EmailAddressType)
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
description: Элемент email представляет пользователя почтового ящика для запроса GetUserAvailability.
ms.openlocfilehash: 2ed8de9c011a385ec6c4ebd2f8d1d47304343a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459232"
---
# <a name="email-emailaddresstype"></a><span data-ttu-id="a352e-103">Электронная почта (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a352e-103">Email (EmailAddressType)</span></span>

<span data-ttu-id="a352e-104">Элемент **Email** представляет пользователя почтового ящика для запроса GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="a352e-104">The **Email** element represents the mailbox user for a GetUserAvailability query.</span></span> 
  
- [<span data-ttu-id="a352e-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="a352e-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)  
- [<span data-ttu-id="a352e-106">маилбоксдатааррай</span><span class="sxs-lookup"><span data-stu-id="a352e-106">MailboxDataArray</span></span>](mailboxdataarray.md) 
- [<span data-ttu-id="a352e-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="a352e-107">MailboxData</span></span>](mailboxdata.md) 
- [<span data-ttu-id="a352e-108">Электронная почта (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a352e-108">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 <span data-ttu-id="a352e-109">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="a352e-109">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a352e-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a352e-110">Attributes and elements</span></span>

<span data-ttu-id="a352e-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a352e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a352e-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a352e-112">Attributes</span></span>

<span data-ttu-id="a352e-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a352e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a352e-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a352e-114">Child elements</span></span>

|<span data-ttu-id="a352e-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a352e-115">**Element**</span></span>|<span data-ttu-id="a352e-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a352e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a352e-117">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a352e-117">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="a352e-118">Представляет отображаемое имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a352e-118">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="a352e-119">Address (строка)</span><span class="sxs-lookup"><span data-stu-id="a352e-119">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="a352e-120">Представляет адрес электронной почты пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a352e-120">Represents the e-mail address of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="a352e-121">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a352e-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="a352e-122">Представляет протокол маршрутизации для сообщения.</span><span class="sxs-lookup"><span data-stu-id="a352e-122">Represents the routing protocol for the message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a352e-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a352e-123">Parent elements</span></span>

|<span data-ttu-id="a352e-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a352e-124">**Element**</span></span>|<span data-ttu-id="a352e-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a352e-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a352e-126">MailboxData</span><span class="sxs-lookup"><span data-stu-id="a352e-126">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="a352e-127">Представляет отдельного пользователя почтового ящика и параметры возвращаемого типа данных об этом пользователе.</span><span class="sxs-lookup"><span data-stu-id="a352e-127">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="a352e-128">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="a352e-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a352e-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="a352e-129">Remarks</span></span>

<span data-ttu-id="a352e-130">Схема с описанием этого элемента находится в каталоге /EWS/ на компьютере, на котором запущено приложение MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a352e-130">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a352e-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a352e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a352e-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a352e-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a352e-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a352e-133">Schema Name</span></span>  <br/> |<span data-ttu-id="a352e-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a352e-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="a352e-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a352e-135">Validation File</span></span>  <br/> |<span data-ttu-id="a352e-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a352e-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a352e-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a352e-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="a352e-138">False</span><span class="sxs-lookup"><span data-stu-id="a352e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a352e-139">См. также</span><span class="sxs-lookup"><span data-stu-id="a352e-139">See also</span></span>

- [<span data-ttu-id="a352e-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a352e-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="a352e-141">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="a352e-141">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="a352e-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="a352e-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

