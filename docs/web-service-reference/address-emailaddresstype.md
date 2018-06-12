---
title: Адрес (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: 518641c8-7f6f-496c-86f9-341e7c1bb44c
description: Элемент адрес — адрес электронной почты полностью разрешенной.
ms.openlocfilehash: 2a2d409edcc3a04bf82c6da0080183becfc9b25b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761423"
---
# <a name="address-emailaddresstype"></a><span data-ttu-id="85b9a-103">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="85b9a-103">Address (EmailAddressType)</span></span>

<span data-ttu-id="85b9a-104">Элемент **адрес** — адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="85b9a-104">The **Address** element represents a fully resolved e-mail address.</span></span> 
  
```XML
<Address>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Address >
```

 <span data-ttu-id="85b9a-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="85b9a-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85b9a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="85b9a-106">Attributes and elements</span></span>

<span data-ttu-id="85b9a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="85b9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85b9a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="85b9a-108">Attributes</span></span>

<span data-ttu-id="85b9a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="85b9a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85b9a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="85b9a-110">Child elements</span></span>

|<span data-ttu-id="85b9a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="85b9a-111">**Element**</span></span>|<span data-ttu-id="85b9a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="85b9a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85b9a-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="85b9a-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="85b9a-114">Определяет имя почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="85b9a-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="85b9a-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="85b9a-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="85b9a-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="85b9a-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="85b9a-117">Определяет адрес Simple Mail Transfer Protocol (SMTP) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="85b9a-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="85b9a-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="85b9a-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="85b9a-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="85b9a-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="85b9a-120">Определяет маршрутизации, используемый для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="85b9a-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="85b9a-121">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="85b9a-121">The default is SMTP.</span></span> <span data-ttu-id="85b9a-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="85b9a-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="85b9a-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="85b9a-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="85b9a-124">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="85b9a-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="85b9a-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="85b9a-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="85b9a-126">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="85b9a-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="85b9a-127">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="85b9a-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="85b9a-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="85b9a-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85b9a-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="85b9a-129">Parent elements</span></span>

|<span data-ttu-id="85b9a-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="85b9a-130">**Element**</span></span>|<span data-ttu-id="85b9a-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="85b9a-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85b9a-132">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="85b9a-132">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="85b9a-133">Содержит коллекцию адресов электронной почты, которые представляют исходные получатели отслеживаемых сообщения.</span><span class="sxs-lookup"><span data-stu-id="85b9a-133">Contains a collection of e-mail addresses that represent the original recipients of a tracked message.</span></span>  <br/> |
|[<span data-ttu-id="85b9a-134">RoomLists</span><span class="sxs-lookup"><span data-stu-id="85b9a-134">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="85b9a-135">Содержит список конференц-залы в организации.</span><span class="sxs-lookup"><span data-stu-id="85b9a-135">Contains a list of meeting rooms in an organization.</span></span>  <br/> |
|[<span data-ttu-id="85b9a-136">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="85b9a-136">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="85b9a-137">Содержит список адресов электронной почты, которые должны входящих сообщений, отправленных в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="85b9a-137">Contains a list of e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85b9a-138">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="85b9a-138">Text value</span></span>

<span data-ttu-id="85b9a-139">Нет.</span><span class="sxs-lookup"><span data-stu-id="85b9a-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85b9a-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="85b9a-140">Remarks</span></span>

<span data-ttu-id="85b9a-141">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="85b9a-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85b9a-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="85b9a-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85b9a-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="85b9a-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85b9a-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="85b9a-144">Schema Name</span></span>  <br/> |<span data-ttu-id="85b9a-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="85b9a-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="85b9a-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="85b9a-146">Validation File</span></span>  <br/> |<span data-ttu-id="85b9a-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="85b9a-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85b9a-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="85b9a-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="85b9a-149">False</span><span class="sxs-lookup"><span data-stu-id="85b9a-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85b9a-150">См. также</span><span class="sxs-lookup"><span data-stu-id="85b9a-150">See also</span></span>

- [<span data-ttu-id="85b9a-151">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="85b9a-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md) 
- [<span data-ttu-id="85b9a-152">Операция GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="85b9a-152">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="85b9a-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="85b9a-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
