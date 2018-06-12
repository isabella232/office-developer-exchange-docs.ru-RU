---
title: SendingAs
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
description: Элемент SendingAs представляет адрес электронной почты, который пользователь пытается отправить как.
ms.openlocfilehash: a5468ddb8facf99038d319252f7e1c780a888ca1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835338"
---
# <a name="sendingas"></a><span data-ttu-id="a5fcb-103">SendingAs</span><span class="sxs-lookup"><span data-stu-id="a5fcb-103">SendingAs</span></span>

<span data-ttu-id="a5fcb-104">Элемент **SendingAs** представляет адрес электронной почты, который пользователь пытается отправить как.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-104">The **SendingAs** element represents an e-mail address that a user is trying to send as.</span></span> 
  
```XML
<SendingAs>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</SendingAs>
```

 <span data-ttu-id="a5fcb-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="a5fcb-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5fcb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a5fcb-106">Attributes and elements</span></span>

<span data-ttu-id="a5fcb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5fcb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a5fcb-108">Attributes</span></span>

<span data-ttu-id="a5fcb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5fcb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a5fcb-110">Child elements</span></span>

|<span data-ttu-id="a5fcb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5fcb-111">**Element**</span></span>|<span data-ttu-id="a5fcb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5fcb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5fcb-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a5fcb-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="a5fcb-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="a5fcb-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a5fcb-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="a5fcb-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="a5fcb-117">Определяет основной адрес Simple Mail Transfer Protocol (SMTP) пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="a5fcb-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a5fcb-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a5fcb-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="a5fcb-120">Определяет тип адреса для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-120">Defines the address type for the mailbox.</span></span> <span data-ttu-id="a5fcb-121">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-121">The default is SMTP.</span></span> <span data-ttu-id="a5fcb-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a5fcb-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="a5fcb-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="a5fcb-124">Представляет тип почтового ящика, представленного для электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-124">Represents the type of mailbox that is represented by an e-mail user.</span></span> <span data-ttu-id="a5fcb-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a5fcb-126">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="a5fcb-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="a5fcb-127">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="a5fcb-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a5fcb-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a5fcb-129">Parent elements</span></span>

|<span data-ttu-id="a5fcb-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5fcb-130">**Element**</span></span>|<span data-ttu-id="a5fcb-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5fcb-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5fcb-132">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="a5fcb-132">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="a5fcb-133">Содержит получателей и типы почтовые подсказки для извлечения.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-133">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a5fcb-134">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a5fcb-134">Text value</span></span>

<span data-ttu-id="a5fcb-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a5fcb-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="a5fcb-136">Remarks</span></span>

<span data-ttu-id="a5fcb-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5fcb-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a5fcb-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5fcb-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a5fcb-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a5fcb-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a5fcb-140">Schema Name</span></span>  <br/> |<span data-ttu-id="a5fcb-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a5fcb-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a5fcb-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a5fcb-142">Validation File</span></span>  <br/> |<span data-ttu-id="a5fcb-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a5fcb-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a5fcb-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a5fcb-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5fcb-145">False</span><span class="sxs-lookup"><span data-stu-id="a5fcb-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5fcb-146">См. также</span><span class="sxs-lookup"><span data-stu-id="a5fcb-146">See also</span></span>



- [<span data-ttu-id="a5fcb-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a5fcb-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

