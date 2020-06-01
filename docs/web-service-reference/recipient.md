---
title: Recipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipient
api_type:
- schema
ms.assetid: 52adbb30-3bfd-48aa-9ea8-9f7d3b4bee44
description: Элемент Recipient представляет получателя, для которого возникло событие.
ms.openlocfilehash: eb7e85acf3c2b898b3f0bff4b63168d344e1daa8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465858"
---
# <a name="recipient"></a><span data-ttu-id="1d4aa-103">Recipient</span><span class="sxs-lookup"><span data-stu-id="1d4aa-103">Recipient</span></span>

<span data-ttu-id="1d4aa-104">Элемент **Recipient** представляет получателя, для которого возникло событие.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-104">The **Recipient** element represents the recipient for whom the event occurred.</span></span> 
  
```XML
<Recipient>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Recipient>
```

 <span data-ttu-id="1d4aa-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="1d4aa-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d4aa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1d4aa-106">Attributes and elements</span></span>

<span data-ttu-id="1d4aa-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d4aa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1d4aa-108">Attributes</span></span>

<span data-ttu-id="1d4aa-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d4aa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1d4aa-110">Child elements</span></span>

|<span data-ttu-id="1d4aa-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1d4aa-111">**Element**</span></span>|<span data-ttu-id="1d4aa-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1d4aa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d4aa-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1d4aa-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="1d4aa-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="1d4aa-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1d4aa-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="1d4aa-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="1d4aa-117">Определяет основной SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="1d4aa-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1d4aa-119">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="1d4aa-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="1d4aa-120">Определяет маршрутизацию, используемую для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="1d4aa-121">По умолчанию используется значение SMTP.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-121">The default value is SMTP.</span></span> <span data-ttu-id="1d4aa-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1d4aa-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="1d4aa-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="1d4aa-124">Представляет тип почтового ящика, представленного адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="1d4aa-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1d4aa-126">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="1d4aa-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1d4aa-127">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="1d4aa-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d4aa-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1d4aa-129">Parent elements</span></span>

|<span data-ttu-id="1d4aa-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1d4aa-130">**Element**</span></span>|<span data-ttu-id="1d4aa-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1d4aa-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d4aa-132">реЦипиенттраккинжевент</span><span class="sxs-lookup"><span data-stu-id="1d4aa-132">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="1d4aa-133">Содержит сведения об отдельном событии получателя.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-133">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="1d4aa-134">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="1d4aa-134">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="1d4aa-135">Задает условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-135">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1d4aa-136">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1d4aa-136">Text value</span></span>

<span data-ttu-id="1d4aa-137">Нет.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1d4aa-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="1d4aa-138">Remarks</span></span>

<span data-ttu-id="1d4aa-139">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1d4aa-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d4aa-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1d4aa-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d4aa-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1d4aa-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1d4aa-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1d4aa-142">Schema Name</span></span>  <br/> |<span data-ttu-id="1d4aa-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1d4aa-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="1d4aa-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1d4aa-144">Validation File</span></span>  <br/> |<span data-ttu-id="1d4aa-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1d4aa-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1d4aa-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1d4aa-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d4aa-147">False</span><span class="sxs-lookup"><span data-stu-id="1d4aa-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d4aa-148">См. также</span><span class="sxs-lookup"><span data-stu-id="1d4aa-148">See also</span></span>



- [<span data-ttu-id="1d4aa-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1d4aa-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

