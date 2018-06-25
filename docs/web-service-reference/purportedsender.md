---
title: PurportedSender
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PurportedSender
api_type:
- schema
ms.assetid: eb7a54ec-2e48-4030-bbcf-50a31609691b
description: Элемент PurportedSender содержит контактные данные для утверждения отправителя сообщения электронной почты.
ms.openlocfilehash: 1e5b74d60d824c06834cf988557ef64fb84d70c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834937"
---
# <a name="purportedsender"></a><span data-ttu-id="060c0-103">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="060c0-103">PurportedSender</span></span>

<span data-ttu-id="060c0-104">Элемент **PurportedSender** содержит контактные данные для утверждения отправителя сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="060c0-104">The **PurportedSender** element contains contact information for the alleged sender of an e-mail message.</span></span> 
  
```XML
<PurportedSender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</PurportedSender>
```

 <span data-ttu-id="060c0-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="060c0-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="060c0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="060c0-106">Attributes and elements</span></span>

<span data-ttu-id="060c0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="060c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="060c0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="060c0-108">Attributes</span></span>

<span data-ttu-id="060c0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="060c0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="060c0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="060c0-110">Child elements</span></span>

|<span data-ttu-id="060c0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="060c0-111">**Element**</span></span>|<span data-ttu-id="060c0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="060c0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="060c0-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="060c0-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="060c0-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="060c0-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="060c0-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="060c0-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="060c0-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="060c0-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="060c0-117">Определяет адрес Simple Mail Transfer Protocol (SMTP) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="060c0-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="060c0-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="060c0-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="060c0-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="060c0-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="060c0-120">Представляет протокол маршрутизации для получателя.</span><span class="sxs-lookup"><span data-stu-id="060c0-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="060c0-121">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="060c0-121">The default value is SMTP.</span></span> <span data-ttu-id="060c0-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="060c0-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="060c0-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="060c0-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="060c0-124">Представляет тип почтового ящика, который соответствует адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="060c0-124">Represents the type of mailbox that is represented by the e-mail address..</span></span> <span data-ttu-id="060c0-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="060c0-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="060c0-126">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="060c0-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="060c0-127">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="060c0-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="060c0-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="060c0-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="060c0-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="060c0-129">Parent elements</span></span>

|<span data-ttu-id="060c0-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="060c0-130">**Element**</span></span>|<span data-ttu-id="060c0-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="060c0-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="060c0-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="060c0-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="060c0-133">Задает условия типам сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="060c0-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="060c0-134">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="060c0-134">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="060c0-135">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="060c0-135">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="060c0-136">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="060c0-136">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="060c0-137">Содержит результат одного сообщения для элемента [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="060c0-137">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="060c0-138">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="060c0-138">Text value</span></span>

<span data-ttu-id="060c0-139">Нет.</span><span class="sxs-lookup"><span data-stu-id="060c0-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="060c0-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="060c0-140">Remarks</span></span>

<span data-ttu-id="060c0-141">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="060c0-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="060c0-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="060c0-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="060c0-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="060c0-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="060c0-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="060c0-144">Schema Name</span></span>  <br/> |<span data-ttu-id="060c0-145">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="060c0-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="060c0-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="060c0-146">Validation File</span></span>  <br/> |<span data-ttu-id="060c0-147">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="060c0-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="060c0-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="060c0-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="060c0-149">False</span><span class="sxs-lookup"><span data-stu-id="060c0-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="060c0-150">См. также</span><span class="sxs-lookup"><span data-stu-id="060c0-150">See also</span></span>



[<span data-ttu-id="060c0-151">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="060c0-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="060c0-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="060c0-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

