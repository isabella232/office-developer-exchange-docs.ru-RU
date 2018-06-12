---
title: Отправитель (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Sender
api_type:
- schema
ms.assetid: 717eb6d0-d167-4b20-92e2-5d08b96186c4
description: Элемент отправителя представляет адрес электронной почты отправителя сообщения.
ms.openlocfilehash: bac62412caf1044c13015f1d9d7ef63552747c1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835320"
---
# <a name="sender-emailaddresstype"></a><span data-ttu-id="1f37b-103">Отправитель (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1f37b-103">Sender (EmailAddressType)</span></span>

<span data-ttu-id="1f37b-104">Элемент **отправителя** представляет адрес электронной почты отправителя сообщения.</span><span class="sxs-lookup"><span data-stu-id="1f37b-104">The **Sender** element represents the e-mail address for the sender of the message.</span></span> 
  
```XML
<Sender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Sender>
```

 <span data-ttu-id="1f37b-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="1f37b-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f37b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1f37b-106">Attributes and elements</span></span>

<span data-ttu-id="1f37b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1f37b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f37b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1f37b-108">Attributes</span></span>

<span data-ttu-id="1f37b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1f37b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f37b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1f37b-110">Child elements</span></span>

|<span data-ttu-id="1f37b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1f37b-111">**Element**</span></span>|<span data-ttu-id="1f37b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1f37b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f37b-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1f37b-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="1f37b-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1f37b-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="1f37b-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1f37b-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1f37b-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="1f37b-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="1f37b-117">Определяет основной адрес Simple Mail Transfer Protocol (SMTP) пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1f37b-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="1f37b-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1f37b-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1f37b-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="1f37b-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="1f37b-120">Представляет протокол маршрутизации для получателя.</span><span class="sxs-lookup"><span data-stu-id="1f37b-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="1f37b-121">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="1f37b-121">The default value is SMTP.</span></span> <span data-ttu-id="1f37b-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1f37b-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1f37b-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="1f37b-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="1f37b-124">Представляет тип почтового ящика, который соответствует адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1f37b-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="1f37b-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1f37b-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1f37b-126">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="1f37b-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1f37b-127">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="1f37b-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="1f37b-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1f37b-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f37b-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1f37b-129">Parent elements</span></span>

|<span data-ttu-id="1f37b-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1f37b-130">**Element**</span></span>|<span data-ttu-id="1f37b-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1f37b-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f37b-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="1f37b-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="1f37b-133">Задает условия типам сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="1f37b-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="1f37b-134">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="1f37b-134">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="1f37b-135">Содержит результат одного сообщения для элемента [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="1f37b-135">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
|[<span data-ttu-id="1f37b-136">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="1f37b-136">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="1f37b-137">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1f37b-137">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f37b-138">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1f37b-138">Text value</span></span>

<span data-ttu-id="1f37b-139">Нет.</span><span class="sxs-lookup"><span data-stu-id="1f37b-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1f37b-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="1f37b-140">Remarks</span></span>

<span data-ttu-id="1f37b-141">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f37b-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f37b-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1f37b-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f37b-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1f37b-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f37b-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1f37b-144">Schema Name</span></span>  <br/> |<span data-ttu-id="1f37b-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1f37b-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="1f37b-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1f37b-146">Validation File</span></span>  <br/> |<span data-ttu-id="1f37b-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1f37b-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f37b-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1f37b-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f37b-149">False</span><span class="sxs-lookup"><span data-stu-id="1f37b-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f37b-150">См. также</span><span class="sxs-lookup"><span data-stu-id="1f37b-150">See also</span></span>



[<span data-ttu-id="1f37b-151">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="1f37b-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="1f37b-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1f37b-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

