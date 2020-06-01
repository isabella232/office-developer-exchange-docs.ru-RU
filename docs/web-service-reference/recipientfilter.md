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
description: Элемент RecipientFilter представляет адрес получателя, который будет использоваться с указанным отчетом об отслеживании сообщений.
ms.openlocfilehash: 945adf9155434e0690debfccc7caf70ba0cb94ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465809"
---
# <a name="recipientfilter"></a><span data-ttu-id="3b92d-103">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="3b92d-103">RecipientFilter</span></span>

<span data-ttu-id="3b92d-104">Элемент **RecipientFilter** представляет адрес получателя, который будет использоваться с указанным отчетом об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="3b92d-104">The **RecipientFilter** element represents a recipient address to use with the specified message tracking report.</span></span> 
  
```XML
 <RecipientFilter>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientFilter>
```

 <span data-ttu-id="3b92d-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="3b92d-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b92d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3b92d-106">Attributes and elements</span></span>

<span data-ttu-id="3b92d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3b92d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b92d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3b92d-108">Attributes</span></span>

<span data-ttu-id="3b92d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3b92d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b92d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3b92d-110">Child elements</span></span>

|<span data-ttu-id="3b92d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3b92d-111">**Element**</span></span>|<span data-ttu-id="3b92d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3b92d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b92d-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="3b92d-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="3b92d-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3b92d-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="3b92d-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3b92d-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3b92d-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="3b92d-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="3b92d-117">Определяет основной SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3b92d-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="3b92d-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3b92d-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3b92d-119">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="3b92d-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="3b92d-120">Представляет протокол маршрутизации для этого получателя.</span><span class="sxs-lookup"><span data-stu-id="3b92d-120">Represents the routing protocol for this recipient.</span></span> <span data-ttu-id="3b92d-121">По умолчанию используется значение SMTP.</span><span class="sxs-lookup"><span data-stu-id="3b92d-121">The default value is SMTP.</span></span> <span data-ttu-id="3b92d-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3b92d-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3b92d-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="3b92d-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="3b92d-124">Представляет тип почтового ящика, представленного адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3b92d-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="3b92d-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3b92d-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3b92d-126">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3b92d-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3b92d-127">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="3b92d-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="3b92d-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3b92d-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b92d-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3b92d-129">Parent elements</span></span>

|<span data-ttu-id="3b92d-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3b92d-130">**Element**</span></span>|<span data-ttu-id="3b92d-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3b92d-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b92d-132">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3b92d-132">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="3b92d-133">Содержит запрос для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="3b92d-133">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3b92d-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3b92d-134">Text value</span></span>

<span data-ttu-id="3b92d-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b92d-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3b92d-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="3b92d-136">Remarks</span></span>

<span data-ttu-id="3b92d-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b92d-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b92d-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3b92d-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b92d-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3b92d-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3b92d-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3b92d-140">Schema Name</span></span>  <br/> |<span data-ttu-id="3b92d-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3b92d-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3b92d-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3b92d-142">Validation File</span></span>  <br/> |<span data-ttu-id="3b92d-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3b92d-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3b92d-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3b92d-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b92d-145">False</span><span class="sxs-lookup"><span data-stu-id="3b92d-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b92d-146">См. также</span><span class="sxs-lookup"><span data-stu-id="3b92d-146">See also</span></span>



[<span data-ttu-id="3b92d-147">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3b92d-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="3b92d-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3b92d-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

