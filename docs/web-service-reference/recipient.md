---
title: Область записи
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
description: Элемент получателя представляет получателя, для которого произошло событие.
ms.openlocfilehash: e8e8f9d6031d27c7441017c85eb26a143258b183
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834971"
---
# <a name="recipient"></a><span data-ttu-id="8fb92-103">Область записи</span><span class="sxs-lookup"><span data-stu-id="8fb92-103">Recipient</span></span>

<span data-ttu-id="8fb92-104">Элемент **получателя** представляет получателя, для которого произошло событие.</span><span class="sxs-lookup"><span data-stu-id="8fb92-104">The **Recipient** element represents the recipient for whom the event occurred.</span></span> 
  
```XML
<Recipient>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Recipient>
```

 <span data-ttu-id="8fb92-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="8fb92-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8fb92-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8fb92-106">Attributes and elements</span></span>

<span data-ttu-id="8fb92-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8fb92-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fb92-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8fb92-108">Attributes</span></span>

<span data-ttu-id="8fb92-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8fb92-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8fb92-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8fb92-110">Child elements</span></span>

|<span data-ttu-id="8fb92-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8fb92-111">**Element**</span></span>|<span data-ttu-id="8fb92-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8fb92-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fb92-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8fb92-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="8fb92-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="8fb92-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="8fb92-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8fb92-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8fb92-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="8fb92-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="8fb92-117">Определяет основной адрес Simple Mail Transfer Protocol (SMTP) пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="8fb92-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="8fb92-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8fb92-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8fb92-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="8fb92-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="8fb92-120">Определяет маршрутизации, используемый для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="8fb92-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="8fb92-121">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="8fb92-121">The default value is SMTP.</span></span> <span data-ttu-id="8fb92-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8fb92-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8fb92-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="8fb92-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="8fb92-124">Представляет тип почтового ящика, который соответствует адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8fb92-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="8fb92-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8fb92-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8fb92-126">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="8fb92-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="8fb92-127">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="8fb92-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="8fb92-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8fb92-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8fb92-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8fb92-129">Parent elements</span></span>

|<span data-ttu-id="8fb92-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8fb92-130">**Element**</span></span>|<span data-ttu-id="8fb92-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8fb92-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fb92-132">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="8fb92-132">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="8fb92-133">Содержит сведения для одного события для получателя.</span><span class="sxs-lookup"><span data-stu-id="8fb92-133">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="8fb92-134">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="8fb92-134">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="8fb92-135">Задает условия типам сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="8fb92-135">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8fb92-136">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8fb92-136">Text value</span></span>

<span data-ttu-id="8fb92-137">Нет.</span><span class="sxs-lookup"><span data-stu-id="8fb92-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8fb92-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="8fb92-138">Remarks</span></span>

<span data-ttu-id="8fb92-139">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8fb92-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8fb92-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8fb92-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fb92-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8fb92-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8fb92-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8fb92-142">Schema Name</span></span>  <br/> |<span data-ttu-id="8fb92-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8fb92-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="8fb92-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8fb92-144">Validation File</span></span>  <br/> |<span data-ttu-id="8fb92-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8fb92-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8fb92-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8fb92-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="8fb92-147">False</span><span class="sxs-lookup"><span data-stu-id="8fb92-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8fb92-148">См. также</span><span class="sxs-lookup"><span data-stu-id="8fb92-148">See also</span></span>



- [<span data-ttu-id="8fb92-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8fb92-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

