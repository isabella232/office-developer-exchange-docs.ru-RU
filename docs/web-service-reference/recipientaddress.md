---
title: RecipientAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientAddress
api_type:
- schema
ms.assetid: 9ae6351a-2c60-4715-a489-5681a13641f9
description: Элемент RecipientAddress представляет почтовый ящик получателя.
ms.openlocfilehash: 10928ac206227cfc21bd83ab5bfa9a55aad354e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834974"
---
# <a name="recipientaddress"></a><span data-ttu-id="b3b9b-103">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="b3b9b-103">RecipientAddress</span></span>

<span data-ttu-id="b3b9b-104">Элемент **RecipientAddress** представляет почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-104">The **RecipientAddress** element represents the mailbox of the recipient.</span></span> 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
```

 <span data-ttu-id="b3b9b-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="b3b9b-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3b9b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b3b9b-106">Attributes and elements</span></span>

<span data-ttu-id="b3b9b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3b9b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b3b9b-108">Attributes</span></span>

<span data-ttu-id="b3b9b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3b9b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b3b9b-110">Child elements</span></span>

|<span data-ttu-id="b3b9b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b3b9b-111">**Element**</span></span>|<span data-ttu-id="b3b9b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b3b9b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3b9b-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="b3b9b-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="b3b9b-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="b3b9b-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b3b9b-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="b3b9b-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="b3b9b-117">Определяет адрес Simple Mail Transfer Protocol (SMTP) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="b3b9b-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b3b9b-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="b3b9b-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="b3b9b-120">Представляет протокол маршрутизации для получателя.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="b3b9b-121">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-121">The default is SMTP.</span></span> <span data-ttu-id="b3b9b-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b3b9b-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="b3b9b-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="b3b9b-124">Представляет тип почтового ящика, который соответствует адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-124">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="b3b9b-125">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="b3b9b-125">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b3b9b-126">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-126">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="b3b9b-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-127">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b3b9b-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b3b9b-128">Parent elements</span></span>

|<span data-ttu-id="b3b9b-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b3b9b-129">**Element**</span></span>|<span data-ttu-id="b3b9b-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b3b9b-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3b9b-131">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="b3b9b-131">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="b3b9b-132">Представляет значения для различных типов почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-132">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b3b9b-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="b3b9b-133">Remarks</span></span>

<span data-ttu-id="b3b9b-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3b9b-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3b9b-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b3b9b-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3b9b-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b3b9b-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b3b9b-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b3b9b-137">Schema Name</span></span>  <br/> |<span data-ttu-id="b3b9b-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b3b9b-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="b3b9b-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b3b9b-139">Validation File</span></span>  <br/> |<span data-ttu-id="b3b9b-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b3b9b-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b3b9b-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b3b9b-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="b3b9b-142">False</span><span class="sxs-lookup"><span data-stu-id="b3b9b-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3b9b-143">См. также</span><span class="sxs-lookup"><span data-stu-id="b3b9b-143">See also</span></span>



- [<span data-ttu-id="b3b9b-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b3b9b-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

