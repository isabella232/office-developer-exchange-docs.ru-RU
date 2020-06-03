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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465809"
---
# <a name="recipientfilter"></a><span data-ttu-id="219e4-103">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="219e4-103">RecipientFilter</span></span>

<span data-ttu-id="219e4-104">Элемент **RecipientFilter** представляет адрес получателя, который будет использоваться с указанным отчетом об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="219e4-104">The **RecipientFilter** element represents a recipient address to use with the specified message tracking report.</span></span> 
  
```XML
 <RecipientFilter>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientFilter>
```

 <span data-ttu-id="219e4-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="219e4-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="219e4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="219e4-106">Attributes and elements</span></span>

<span data-ttu-id="219e4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="219e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="219e4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="219e4-108">Attributes</span></span>

<span data-ttu-id="219e4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="219e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="219e4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="219e4-110">Child elements</span></span>

|<span data-ttu-id="219e4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="219e4-111">**Element**</span></span>|<span data-ttu-id="219e4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="219e4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="219e4-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="219e4-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="219e4-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="219e4-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="219e4-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="219e4-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="219e4-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="219e4-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="219e4-117">Определяет основной SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="219e4-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="219e4-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="219e4-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="219e4-119">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="219e4-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="219e4-120">Представляет протокол маршрутизации для этого получателя.</span><span class="sxs-lookup"><span data-stu-id="219e4-120">Represents the routing protocol for this recipient.</span></span> <span data-ttu-id="219e4-121">По умолчанию используется значение SMTP.</span><span class="sxs-lookup"><span data-stu-id="219e4-121">The default value is SMTP.</span></span> <span data-ttu-id="219e4-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="219e4-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="219e4-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="219e4-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="219e4-124">Представляет тип почтового ящика, представленного адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="219e4-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="219e4-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="219e4-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="219e4-126">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="219e4-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="219e4-127">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="219e4-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="219e4-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="219e4-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="219e4-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="219e4-129">Parent elements</span></span>

|<span data-ttu-id="219e4-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="219e4-130">**Element**</span></span>|<span data-ttu-id="219e4-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="219e4-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="219e4-132">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="219e4-132">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="219e4-133">Содержит запрос для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="219e4-133">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="219e4-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="219e4-134">Text value</span></span>

<span data-ttu-id="219e4-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="219e4-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="219e4-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="219e4-136">Remarks</span></span>

<span data-ttu-id="219e4-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="219e4-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="219e4-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="219e4-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="219e4-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="219e4-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="219e4-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="219e4-140">Schema Name</span></span>  <br/> |<span data-ttu-id="219e4-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="219e4-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="219e4-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="219e4-142">Validation File</span></span>  <br/> |<span data-ttu-id="219e4-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="219e4-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="219e4-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="219e4-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="219e4-145">False</span><span class="sxs-lookup"><span data-stu-id="219e4-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="219e4-146">См. также</span><span class="sxs-lookup"><span data-stu-id="219e4-146">See also</span></span>



[<span data-ttu-id="219e4-147">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="219e4-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="219e4-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="219e4-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

