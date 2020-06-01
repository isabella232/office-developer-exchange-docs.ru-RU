---
title: Запись (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: b028c5c7-3494-4ecd-96d1-78783daa660f
description: Элемент entry представляет один адрес электронной почты контакта.
ms.openlocfilehash: 766d67cda10b02c07a7677e541fddfc38a4285cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459646"
---
# <a name="entry-emailaddress"></a><span data-ttu-id="b279f-103">Запись (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="b279f-103">Entry (EmailAddress)</span></span>

<span data-ttu-id="b279f-104">Элемент **entry** представляет один адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="b279f-104">The **Entry** element represents a single e-mail address for a contact.</span></span> 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

<span data-ttu-id="b279f-105">**емаиладдрессдиктионарентритипе**</span><span class="sxs-lookup"><span data-stu-id="b279f-105">**EmailAddressDictionaryEntryType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b279f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b279f-106">Attributes and elements</span></span>

<span data-ttu-id="b279f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b279f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b279f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b279f-108">Attributes</span></span>

|<span data-ttu-id="b279f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b279f-109">**Attribute**</span></span>|<span data-ttu-id="b279f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b279f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b279f-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="b279f-111">**Key**</span></span> <br/> | <span data-ttu-id="b279f-112">Определяет адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b279f-112">Identifies the e-mail address.</span></span><br/><br/><span data-ttu-id="b279f-113">Ниже приведены возможные значения для этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="b279f-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="b279f-114">- EmailAddress1</span><span class="sxs-lookup"><span data-stu-id="b279f-114">-  EmailAddress1</span></span>  <br/><span data-ttu-id="b279f-115">- EmailAddress2</span><span class="sxs-lookup"><span data-stu-id="b279f-115">-  EmailAddress2</span></span>  <br/><span data-ttu-id="b279f-116">- EmailAddress3</span><span class="sxs-lookup"><span data-stu-id="b279f-116">-  EmailAddress3</span></span> <br/><br/>  <span data-ttu-id="b279f-117">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="b279f-117">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="b279f-118">**имя**</span><span class="sxs-lookup"><span data-stu-id="b279f-118">**Name**</span></span> <br/> |<span data-ttu-id="b279f-119">Определяет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b279f-119">Defines the name of the mailbox user.</span></span> <span data-ttu-id="b279f-120">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b279f-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="b279f-121">**раутингтипе**</span><span class="sxs-lookup"><span data-stu-id="b279f-121">**RoutingType**</span></span> <br/> |<span data-ttu-id="b279f-122">Определяет маршрутизацию, используемую для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b279f-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="b279f-123">По умолчанию используется протокол SMTP.</span><span class="sxs-lookup"><span data-stu-id="b279f-123">The default is SMTP.</span></span> <span data-ttu-id="b279f-124">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b279f-124">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="b279f-125">**MailboxType**</span><span class="sxs-lookup"><span data-stu-id="b279f-125">**MailboxType**</span></span> <br/> |<span data-ttu-id="b279f-126">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b279f-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="b279f-127">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b279f-127">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b279f-128">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b279f-128">Child elements</span></span>

<span data-ttu-id="b279f-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b279f-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b279f-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b279f-130">Parent elements</span></span>

|<span data-ttu-id="b279f-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b279f-131">**Element**</span></span>|<span data-ttu-id="b279f-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b279f-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b279f-133">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="b279f-133">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="b279f-134">Представляет коллекцию адресов электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="b279f-134">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b279f-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="b279f-135">Remarks</span></span>

<span data-ttu-id="b279f-136">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b279f-136">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b279f-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b279f-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b279f-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b279f-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b279f-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b279f-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b279f-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b279f-140">Schema name</span></span>  <br/> |<span data-ttu-id="b279f-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b279f-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="b279f-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b279f-142">Validation file</span></span>  <br/> |<span data-ttu-id="b279f-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b279f-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b279f-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b279f-144">Can be empty</span></span>  <br/> |<span data-ttu-id="b279f-145">False</span><span class="sxs-lookup"><span data-stu-id="b279f-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b279f-146">См. также</span><span class="sxs-lookup"><span data-stu-id="b279f-146">See also</span></span>

- [<span data-ttu-id="b279f-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b279f-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

