---
title: FederatedDeliveryMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FederatedDeliveryMailbox
api_type:
- schema
ms.assetid: cd56bcc0-d24a-4e8b-87bd-999bf69234b7
description: Элемент FederatedDeliveryMailbox представляет почтовых ящиков, в которой было отправлено сообщение кросс сервер.
ms.openlocfilehash: 4a9250455f8de3ede25f2b5ba9433690137ca1d3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762525"
---
# <a name="federateddeliverymailbox"></a><span data-ttu-id="7334d-103">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="7334d-103">FederatedDeliveryMailbox</span></span>

<span data-ttu-id="7334d-104">Элемент **FederatedDeliveryMailbox** представляет почтовых ящиков, в которой было отправлено сообщение кросс сервер.</span><span class="sxs-lookup"><span data-stu-id="7334d-104">The **FederatedDeliveryMailbox** element represents the mailbox to which a cross-premise message was sent.</span></span> 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 <span data-ttu-id="7334d-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="7334d-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7334d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7334d-106">Attributes and elements</span></span>

<span data-ttu-id="7334d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7334d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7334d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7334d-108">Attributes</span></span>

<span data-ttu-id="7334d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7334d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7334d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7334d-110">Child elements</span></span>

|<span data-ttu-id="7334d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7334d-111">**Element**</span></span>|<span data-ttu-id="7334d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7334d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7334d-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7334d-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="7334d-114">Определяет имя почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="7334d-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="7334d-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7334d-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7334d-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="7334d-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="7334d-117">Определяет адрес Simple Mail Transfer Protocol (SMTP) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="7334d-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="7334d-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7334d-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7334d-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="7334d-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="7334d-120">Определяет маршрутизации, используемый для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7334d-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="7334d-121">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="7334d-121">The default is SMTP.</span></span> <span data-ttu-id="7334d-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7334d-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7334d-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="7334d-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="7334d-124">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7334d-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="7334d-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7334d-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7334d-126">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="7334d-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7334d-127">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="7334d-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="7334d-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7334d-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7334d-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7334d-129">Parent elements</span></span>

|<span data-ttu-id="7334d-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7334d-130">**Element**</span></span>|<span data-ttu-id="7334d-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7334d-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7334d-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7334d-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="7334d-133">Содержит критерии для типов сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="7334d-133">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7334d-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7334d-134">Text value</span></span>

<span data-ttu-id="7334d-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="7334d-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7334d-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="7334d-136">Remarks</span></span>

<span data-ttu-id="7334d-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7334d-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7334d-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7334d-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7334d-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7334d-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7334d-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7334d-140">Schema Name</span></span>  <br/> |<span data-ttu-id="7334d-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7334d-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7334d-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7334d-142">Validation File</span></span>  <br/> |<span data-ttu-id="7334d-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7334d-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7334d-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7334d-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="7334d-145">False</span><span class="sxs-lookup"><span data-stu-id="7334d-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7334d-146">См. также</span><span class="sxs-lookup"><span data-stu-id="7334d-146">See also</span></span>



- [<span data-ttu-id="7334d-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7334d-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

