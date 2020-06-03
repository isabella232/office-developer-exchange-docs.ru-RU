---
title: федератедделиверимаилбокс
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
description: Элемент Федератедделиверимаилбокс представляет почтовый ящик, в который было отправлено сообщение с перекрестным локальным сообщением.
ms.openlocfilehash: d493ed81e82237b7257e8c469f4552d931b73aa6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461949"
---
# <a name="federateddeliverymailbox"></a><span data-ttu-id="c6262-103">федератедделиверимаилбокс</span><span class="sxs-lookup"><span data-stu-id="c6262-103">FederatedDeliveryMailbox</span></span>

<span data-ttu-id="c6262-104">Элемент **федератедделиверимаилбокс** представляет почтовый ящик, в который было отправлено сообщение с перекрестным локальным сообщением.</span><span class="sxs-lookup"><span data-stu-id="c6262-104">The **FederatedDeliveryMailbox** element represents the mailbox to which a cross-premise message was sent.</span></span> 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 <span data-ttu-id="c6262-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="c6262-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6262-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c6262-106">Attributes and elements</span></span>

<span data-ttu-id="c6262-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c6262-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6262-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c6262-108">Attributes</span></span>

<span data-ttu-id="c6262-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c6262-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6262-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c6262-110">Child elements</span></span>

|<span data-ttu-id="c6262-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c6262-111">**Element**</span></span>|<span data-ttu-id="c6262-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c6262-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6262-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="c6262-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="c6262-114">Определяет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c6262-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="c6262-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="c6262-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c6262-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="c6262-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="c6262-117">Определяет SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c6262-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="c6262-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="c6262-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c6262-119">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="c6262-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="c6262-120">Определяет маршрутизацию, используемую для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c6262-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="c6262-121">По умолчанию используется протокол SMTP.</span><span class="sxs-lookup"><span data-stu-id="c6262-121">The default is SMTP.</span></span> <span data-ttu-id="c6262-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="c6262-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c6262-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="c6262-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="c6262-124">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c6262-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="c6262-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="c6262-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c6262-126">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="c6262-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="c6262-127">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6262-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="c6262-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="c6262-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c6262-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c6262-129">Parent elements</span></span>

|<span data-ttu-id="c6262-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c6262-130">**Element**</span></span>|<span data-ttu-id="c6262-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c6262-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6262-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c6262-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="c6262-133">Содержит условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="c6262-133">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c6262-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c6262-134">Text value</span></span>

<span data-ttu-id="c6262-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="c6262-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c6262-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="c6262-136">Remarks</span></span>

<span data-ttu-id="c6262-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6262-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6262-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c6262-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6262-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c6262-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c6262-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c6262-140">Schema Name</span></span>  <br/> |<span data-ttu-id="c6262-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c6262-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c6262-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c6262-142">Validation File</span></span>  <br/> |<span data-ttu-id="c6262-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c6262-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c6262-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c6262-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6262-145">False</span><span class="sxs-lookup"><span data-stu-id="c6262-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6262-146">См. также</span><span class="sxs-lookup"><span data-stu-id="c6262-146">See also</span></span>



- [<span data-ttu-id="c6262-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c6262-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

