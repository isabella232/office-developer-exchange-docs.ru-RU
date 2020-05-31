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
description: Элемент Получательимеет адрес представляет почтовый ящик получателя.
ms.openlocfilehash: 10928ac206227cfc21bd83ab5bfa9a55aad354e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834974"
---
# <a name="recipientaddress"></a><span data-ttu-id="3fed7-103">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="3fed7-103">RecipientAddress</span></span>

<span data-ttu-id="3fed7-104">Элемент **получательимеет адрес** представляет почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="3fed7-104">The **RecipientAddress** element represents the mailbox of the recipient.</span></span> 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
```

 <span data-ttu-id="3fed7-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="3fed7-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3fed7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3fed7-106">Attributes and elements</span></span>

<span data-ttu-id="3fed7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3fed7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3fed7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3fed7-108">Attributes</span></span>

<span data-ttu-id="3fed7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3fed7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3fed7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3fed7-110">Child elements</span></span>

|<span data-ttu-id="3fed7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3fed7-111">**Element**</span></span>|<span data-ttu-id="3fed7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3fed7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fed7-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="3fed7-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="3fed7-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3fed7-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="3fed7-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3fed7-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3fed7-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="3fed7-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="3fed7-117">Определяет SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3fed7-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="3fed7-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3fed7-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3fed7-119">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="3fed7-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="3fed7-120">Представляет протокол маршрутизации для получателя.</span><span class="sxs-lookup"><span data-stu-id="3fed7-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="3fed7-121">По умолчанию используется протокол SMTP.</span><span class="sxs-lookup"><span data-stu-id="3fed7-121">The default is SMTP.</span></span> <span data-ttu-id="3fed7-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3fed7-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3fed7-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="3fed7-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="3fed7-124">Представляет тип почтового ящика, представленного адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3fed7-124">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="3fed7-125">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3fed7-125">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3fed7-126">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="3fed7-126">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="3fed7-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3fed7-127">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3fed7-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3fed7-128">Parent elements</span></span>

|<span data-ttu-id="3fed7-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3fed7-129">**Element**</span></span>|<span data-ttu-id="3fed7-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3fed7-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fed7-131">Подсказки</span><span class="sxs-lookup"><span data-stu-id="3fed7-131">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="3fed7-132">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3fed7-132">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3fed7-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="3fed7-133">Remarks</span></span>

<span data-ttu-id="3fed7-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3fed7-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3fed7-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3fed7-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3fed7-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3fed7-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3fed7-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3fed7-137">Schema Name</span></span>  <br/> |<span data-ttu-id="3fed7-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3fed7-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="3fed7-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3fed7-139">Validation File</span></span>  <br/> |<span data-ttu-id="3fed7-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3fed7-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3fed7-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3fed7-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="3fed7-142">False</span><span class="sxs-lookup"><span data-stu-id="3fed7-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3fed7-143">См. также</span><span class="sxs-lookup"><span data-stu-id="3fed7-143">See also</span></span>



- [<span data-ttu-id="3fed7-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3fed7-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

