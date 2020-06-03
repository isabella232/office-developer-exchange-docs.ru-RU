---
title: сендингас
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendingAs
api_type:
- schema
ms.assetid: b43ce19f-9ab0-4946-acb2-c5aafead9d35
description: Элемент Сендингас представляет адрес электронной почты, который пользователь пытается отправить как.
ms.openlocfilehash: cd11bd60cbbe3434fcc1b0b9a1cfe0de9f0b1e21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462138"
---
# <a name="sendingas"></a><span data-ttu-id="e98cc-103">сендингас</span><span class="sxs-lookup"><span data-stu-id="e98cc-103">SendingAs</span></span>

<span data-ttu-id="e98cc-104">Элемент **сендингас** представляет адрес электронной почты, который пользователь пытается отправить как.</span><span class="sxs-lookup"><span data-stu-id="e98cc-104">The **SendingAs** element represents an e-mail address that a user is trying to send as.</span></span> 
  
```XML
<SendingAs>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</SendingAs>
```

 <span data-ttu-id="e98cc-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="e98cc-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e98cc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e98cc-106">Attributes and elements</span></span>

<span data-ttu-id="e98cc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e98cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e98cc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e98cc-108">Attributes</span></span>

<span data-ttu-id="e98cc-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e98cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e98cc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e98cc-110">Child elements</span></span>

|<span data-ttu-id="e98cc-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e98cc-111">**Element**</span></span>|<span data-ttu-id="e98cc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e98cc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e98cc-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e98cc-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="e98cc-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e98cc-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="e98cc-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e98cc-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e98cc-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="e98cc-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="e98cc-117">Определяет основной SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e98cc-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="e98cc-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e98cc-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e98cc-119">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="e98cc-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="e98cc-120">Определяет тип адреса для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e98cc-120">Defines the address type for the mailbox.</span></span> <span data-ttu-id="e98cc-121">По умолчанию используется протокол SMTP.</span><span class="sxs-lookup"><span data-stu-id="e98cc-121">The default is SMTP.</span></span> <span data-ttu-id="e98cc-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e98cc-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e98cc-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="e98cc-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="e98cc-124">Представляет тип почтового ящика, представленного пользователем электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e98cc-124">Represents the type of mailbox that is represented by an e-mail user.</span></span> <span data-ttu-id="e98cc-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e98cc-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e98cc-126">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="e98cc-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e98cc-127">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="e98cc-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="e98cc-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e98cc-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e98cc-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e98cc-129">Parent elements</span></span>

|<span data-ttu-id="e98cc-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e98cc-130">**Element**</span></span>|<span data-ttu-id="e98cc-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e98cc-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e98cc-132">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="e98cc-132">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="e98cc-133">Содержит получателей и типы советов по работе с почтой, которые необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="e98cc-133">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e98cc-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e98cc-134">Text value</span></span>

<span data-ttu-id="e98cc-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="e98cc-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e98cc-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="e98cc-136">Remarks</span></span>

<span data-ttu-id="e98cc-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e98cc-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e98cc-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e98cc-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e98cc-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e98cc-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e98cc-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e98cc-140">Schema Name</span></span>  <br/> |<span data-ttu-id="e98cc-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e98cc-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e98cc-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e98cc-142">Validation File</span></span>  <br/> |<span data-ttu-id="e98cc-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e98cc-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e98cc-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e98cc-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="e98cc-145">False</span><span class="sxs-lookup"><span data-stu-id="e98cc-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e98cc-146">См. также</span><span class="sxs-lookup"><span data-stu-id="e98cc-146">See also</span></span>



- [<span data-ttu-id="e98cc-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e98cc-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

