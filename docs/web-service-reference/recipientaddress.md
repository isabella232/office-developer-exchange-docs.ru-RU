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
ms.openlocfilehash: f4b6edd034dd91471e6496f6b0cca65bd3ffb69a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465851"
---
# <a name="recipientaddress"></a><span data-ttu-id="3c1f3-103">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="3c1f3-103">RecipientAddress</span></span>

<span data-ttu-id="3c1f3-104">Элемент **получательимеет адрес** представляет почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-104">The **RecipientAddress** element represents the mailbox of the recipient.</span></span> 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
```

 <span data-ttu-id="3c1f3-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="3c1f3-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c1f3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3c1f3-106">Attributes and elements</span></span>

<span data-ttu-id="3c1f3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c1f3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3c1f3-108">Attributes</span></span>

<span data-ttu-id="3c1f3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c1f3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3c1f3-110">Child elements</span></span>

|<span data-ttu-id="3c1f3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3c1f3-111">**Element**</span></span>|<span data-ttu-id="3c1f3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3c1f3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c1f3-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="3c1f3-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="3c1f3-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="3c1f3-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3c1f3-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="3c1f3-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="3c1f3-117">Определяет SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="3c1f3-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3c1f3-119">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="3c1f3-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="3c1f3-120">Представляет протокол маршрутизации для получателя.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="3c1f3-121">По умолчанию используется протокол SMTP.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-121">The default is SMTP.</span></span> <span data-ttu-id="3c1f3-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="3c1f3-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="3c1f3-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="3c1f3-124">Представляет тип почтового ящика, представленного адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-124">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="3c1f3-125">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3c1f3-125">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3c1f3-126">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-126">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="3c1f3-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-127">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c1f3-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3c1f3-128">Parent elements</span></span>

|<span data-ttu-id="3c1f3-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3c1f3-129">**Element**</span></span>|<span data-ttu-id="3c1f3-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3c1f3-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c1f3-131">Подсказки</span><span class="sxs-lookup"><span data-stu-id="3c1f3-131">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="3c1f3-132">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-132">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3c1f3-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="3c1f3-133">Remarks</span></span>

<span data-ttu-id="3c1f3-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c1f3-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c1f3-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3c1f3-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c1f3-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3c1f3-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c1f3-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3c1f3-137">Schema Name</span></span>  <br/> |<span data-ttu-id="3c1f3-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3c1f3-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c1f3-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3c1f3-139">Validation File</span></span>  <br/> |<span data-ttu-id="3c1f3-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3c1f3-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c1f3-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3c1f3-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c1f3-142">False</span><span class="sxs-lookup"><span data-stu-id="3c1f3-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c1f3-143">См. также</span><span class="sxs-lookup"><span data-stu-id="3c1f3-143">See also</span></span>



- [<span data-ttu-id="3c1f3-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3c1f3-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

