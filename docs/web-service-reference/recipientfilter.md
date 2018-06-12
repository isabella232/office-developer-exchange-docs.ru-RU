---
title: RecipientFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientFilter
api_type:
- schema
ms.assetid: 956c287a-a38a-49a7-a877-6d2088dfbc06
description: Элемент RecipientFilter представляет адрес получателя для использования с заданным сообщением отслеживания отчета.
ms.openlocfilehash: c31ed469132b110a690416b112d5e4e96e44c501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834972"
---
# <a name="recipientfilter"></a><span data-ttu-id="877d5-103">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="877d5-103">RecipientFilter</span></span>

<span data-ttu-id="877d5-104">Элемент **RecipientFilter** представляет адрес получателя для использования с заданным сообщением отслеживания отчета.</span><span class="sxs-lookup"><span data-stu-id="877d5-104">The **RecipientFilter** element represents a recipient address to use with the specified message tracking report.</span></span> 
  
```XML
 <RecipientFilter>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientFilter>
```

 <span data-ttu-id="877d5-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="877d5-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="877d5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="877d5-106">Attributes and elements</span></span>

<span data-ttu-id="877d5-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="877d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="877d5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="877d5-108">Attributes</span></span>

<span data-ttu-id="877d5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="877d5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="877d5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="877d5-110">Child elements</span></span>

|<span data-ttu-id="877d5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="877d5-111">**Element**</span></span>|<span data-ttu-id="877d5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="877d5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="877d5-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="877d5-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="877d5-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="877d5-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="877d5-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="877d5-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="877d5-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="877d5-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="877d5-117">Определяет основной адрес Simple Mail Transfer Protocol (SMTP) пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="877d5-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="877d5-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="877d5-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="877d5-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="877d5-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="877d5-120">Представляет протокол маршрутизации для данного получателя.</span><span class="sxs-lookup"><span data-stu-id="877d5-120">Represents the routing protocol for this recipient.</span></span> <span data-ttu-id="877d5-121">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="877d5-121">The default value is SMTP.</span></span> <span data-ttu-id="877d5-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="877d5-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="877d5-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="877d5-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="877d5-124">Представляет тип почтового ящика, который соответствует адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="877d5-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="877d5-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="877d5-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="877d5-126">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="877d5-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="877d5-127">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="877d5-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="877d5-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="877d5-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="877d5-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="877d5-129">Parent elements</span></span>

|<span data-ttu-id="877d5-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="877d5-130">**Element**</span></span>|<span data-ttu-id="877d5-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="877d5-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="877d5-132">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="877d5-132">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="877d5-133">Содержит запроса для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного сообщения, отслеживания отчетов для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="877d5-133">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="877d5-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="877d5-134">Text value</span></span>

<span data-ttu-id="877d5-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="877d5-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="877d5-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="877d5-136">Remarks</span></span>

<span data-ttu-id="877d5-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="877d5-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="877d5-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="877d5-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="877d5-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="877d5-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="877d5-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="877d5-140">Schema Name</span></span>  <br/> |<span data-ttu-id="877d5-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="877d5-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="877d5-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="877d5-142">Validation File</span></span>  <br/> |<span data-ttu-id="877d5-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="877d5-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="877d5-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="877d5-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="877d5-145">False</span><span class="sxs-lookup"><span data-stu-id="877d5-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="877d5-146">См. также</span><span class="sxs-lookup"><span data-stu-id="877d5-146">See also</span></span>



[<span data-ttu-id="877d5-147">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="877d5-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="877d5-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="877d5-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

