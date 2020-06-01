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
description: Элемент Address представляет полностью разрешенный адрес электронной почты.
ms.openlocfilehash: 591bc675165ec80f69407bd8ee19d16c9ddff15a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464905"
---
# <a name="address-emailaddresstype"></a><span data-ttu-id="0dc0a-103">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="0dc0a-103">Address (EmailAddressType)</span></span>

<span data-ttu-id="0dc0a-104">Элемент **Address** представляет полностью разрешенный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-104">The **Address** element represents a fully resolved e-mail address.</span></span> 
  
```XML
<Address>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Address >
```

 <span data-ttu-id="0dc0a-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="0dc0a-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0dc0a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0dc0a-106">Attributes and elements</span></span>

<span data-ttu-id="0dc0a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0dc0a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0dc0a-108">Attributes</span></span>

<span data-ttu-id="0dc0a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0dc0a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0dc0a-110">Child elements</span></span>

|<span data-ttu-id="0dc0a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0dc0a-111">**Element**</span></span>|<span data-ttu-id="0dc0a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0dc0a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0dc0a-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="0dc0a-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="0dc0a-114">Определяет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="0dc0a-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0dc0a-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="0dc0a-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="0dc0a-117">Определяет SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="0dc0a-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0dc0a-119">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="0dc0a-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="0dc0a-120">Определяет маршрутизацию, используемую для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="0dc0a-121">По умолчанию используется протокол SMTP.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-121">The default is SMTP.</span></span> <span data-ttu-id="0dc0a-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0dc0a-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="0dc0a-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="0dc0a-124">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="0dc0a-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0dc0a-126">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="0dc0a-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0dc0a-127">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="0dc0a-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0dc0a-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0dc0a-129">Parent elements</span></span>

|<span data-ttu-id="0dc0a-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0dc0a-130">**Element**</span></span>|<span data-ttu-id="0dc0a-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0dc0a-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0dc0a-132">оригиналреЦипиентс</span><span class="sxs-lookup"><span data-stu-id="0dc0a-132">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="0dc0a-133">Содержит набор адресов электронной почты, которые представляют исходных получателей отслеживаемого сообщения.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-133">Contains a collection of e-mail addresses that represent the original recipients of a tracked message.</span></span>  <br/> |
|[<span data-ttu-id="0dc0a-134">румлистс</span><span class="sxs-lookup"><span data-stu-id="0dc0a-134">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="0dc0a-135">Содержит список комнат для собраний в Организации.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-135">Contains a list of meeting rooms in an organization.</span></span>  <br/> |
|[<span data-ttu-id="0dc0a-136">сенттоаддрессес</span><span class="sxs-lookup"><span data-stu-id="0dc0a-136">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="0dc0a-137">Содержит список адресов электронной почты, на которые должны быть отправлены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-137">Contains a list of e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0dc0a-138">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0dc0a-138">Text value</span></span>

<span data-ttu-id="0dc0a-139">Нет.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0dc0a-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="0dc0a-140">Remarks</span></span>

<span data-ttu-id="0dc0a-141">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dc0a-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0dc0a-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0dc0a-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0dc0a-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0dc0a-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0dc0a-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0dc0a-144">Schema Name</span></span>  <br/> |<span data-ttu-id="0dc0a-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0dc0a-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="0dc0a-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0dc0a-146">Validation File</span></span>  <br/> |<span data-ttu-id="0dc0a-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0dc0a-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0dc0a-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0dc0a-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="0dc0a-149">False</span><span class="sxs-lookup"><span data-stu-id="0dc0a-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0dc0a-150">См. также</span><span class="sxs-lookup"><span data-stu-id="0dc0a-150">See also</span></span>

- [<span data-ttu-id="0dc0a-151">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="0dc0a-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md) 
- [<span data-ttu-id="0dc0a-152">Операция GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="0dc0a-152">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="0dc0a-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0dc0a-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

