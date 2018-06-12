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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762525"
---
# <a name="federateddeliverymailbox"></a><span data-ttu-id="af345-103">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="af345-103">FederatedDeliveryMailbox</span></span>

<span data-ttu-id="af345-104">Элемент **FederatedDeliveryMailbox** представляет почтовых ящиков, в которой было отправлено сообщение кросс сервер.</span><span class="sxs-lookup"><span data-stu-id="af345-104">The **FederatedDeliveryMailbox** element represents the mailbox to which a cross-premise message was sent.</span></span> 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 <span data-ttu-id="af345-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="af345-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af345-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="af345-106">Attributes and elements</span></span>

<span data-ttu-id="af345-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="af345-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af345-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="af345-108">Attributes</span></span>

<span data-ttu-id="af345-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="af345-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af345-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="af345-110">Child elements</span></span>

|<span data-ttu-id="af345-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="af345-111">**Element**</span></span>|<span data-ttu-id="af345-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="af345-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af345-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="af345-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="af345-114">Определяет имя почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="af345-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="af345-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="af345-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="af345-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="af345-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="af345-117">Определяет адрес Simple Mail Transfer Protocol (SMTP) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="af345-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="af345-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="af345-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="af345-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="af345-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="af345-120">Определяет маршрутизации, используемый для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="af345-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="af345-121">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="af345-121">The default is SMTP.</span></span> <span data-ttu-id="af345-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="af345-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="af345-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="af345-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="af345-124">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="af345-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="af345-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="af345-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="af345-126">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="af345-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="af345-127">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="af345-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="af345-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="af345-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af345-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="af345-129">Parent elements</span></span>

|<span data-ttu-id="af345-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="af345-130">**Element**</span></span>|<span data-ttu-id="af345-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="af345-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af345-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="af345-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="af345-133">Содержит критерии для типов сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="af345-133">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="af345-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="af345-134">Text value</span></span>

<span data-ttu-id="af345-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="af345-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="af345-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="af345-136">Remarks</span></span>

<span data-ttu-id="af345-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="af345-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af345-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="af345-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af345-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="af345-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="af345-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="af345-140">Schema Name</span></span>  <br/> |<span data-ttu-id="af345-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="af345-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="af345-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="af345-142">Validation File</span></span>  <br/> |<span data-ttu-id="af345-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="af345-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="af345-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="af345-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="af345-145">False</span><span class="sxs-lookup"><span data-stu-id="af345-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af345-146">См. также</span><span class="sxs-lookup"><span data-stu-id="af345-146">See also</span></span>



- [<span data-ttu-id="af345-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="af345-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

