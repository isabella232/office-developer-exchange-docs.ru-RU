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
description: Элемент представляет адрес электронной почты контакта.
ms.openlocfilehash: 1852584e507c38da030815c37f85f7c4af4e2ba4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762366"
---
# <a name="entry-emailaddress"></a><span data-ttu-id="532b7-103">Запись (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="532b7-103">Entry (EmailAddress)</span></span>

<span data-ttu-id="532b7-104">**Элемент** представляет адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="532b7-104">The **Entry** element represents a single e-mail address for a contact.</span></span> 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

<span data-ttu-id="532b7-105">**EmailAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="532b7-105">**EmailAddressDictionaryEntryType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="532b7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="532b7-106">Attributes and elements</span></span>

<span data-ttu-id="532b7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="532b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="532b7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="532b7-108">Attributes</span></span>

|<span data-ttu-id="532b7-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="532b7-109">**Attribute**</span></span>|<span data-ttu-id="532b7-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="532b7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="532b7-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="532b7-111">**Key**</span></span> <br/> | <span data-ttu-id="532b7-112">Указывает адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="532b7-112">Identifies the e-mail address.</span></span><br/><br/><span data-ttu-id="532b7-113">Ниже приведены возможные значения этого атрибута.</span><span class="sxs-lookup"><span data-stu-id="532b7-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="532b7-114">-EmailAddress1</span><span class="sxs-lookup"><span data-stu-id="532b7-114">-  EmailAddress1</span></span>  <br/><span data-ttu-id="532b7-115">-EmailAddress2</span><span class="sxs-lookup"><span data-stu-id="532b7-115">-  EmailAddress2</span></span>  <br/><span data-ttu-id="532b7-116">-EmailAddress3</span><span class="sxs-lookup"><span data-stu-id="532b7-116">-  EmailAddress3</span></span> <br/><br/>  <span data-ttu-id="532b7-117">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="532b7-117">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="532b7-118">**Имя**</span><span class="sxs-lookup"><span data-stu-id="532b7-118">**Name**</span></span> <br/> |<span data-ttu-id="532b7-119">Определяет имя почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="532b7-119">Defines the name of the mailbox user.</span></span> <span data-ttu-id="532b7-120">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="532b7-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="532b7-121">**RoutingType**</span><span class="sxs-lookup"><span data-stu-id="532b7-121">**RoutingType**</span></span> <br/> |<span data-ttu-id="532b7-122">Определяет маршрутизации, используемый для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="532b7-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="532b7-123">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="532b7-123">The default is SMTP.</span></span> <span data-ttu-id="532b7-124">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="532b7-124">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="532b7-125">**MailboxType**</span><span class="sxs-lookup"><span data-stu-id="532b7-125">**MailboxType**</span></span> <br/> |<span data-ttu-id="532b7-126">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="532b7-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="532b7-127">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="532b7-127">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="532b7-128">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="532b7-128">Child elements</span></span>

<span data-ttu-id="532b7-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="532b7-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="532b7-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="532b7-130">Parent elements</span></span>

|<span data-ttu-id="532b7-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="532b7-131">**Element**</span></span>|<span data-ttu-id="532b7-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="532b7-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="532b7-133">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="532b7-133">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="532b7-134">Представляет коллекцию адреса электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="532b7-134">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="532b7-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="532b7-135">Remarks</span></span>

<span data-ttu-id="532b7-136">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="532b7-136">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="532b7-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="532b7-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="532b7-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="532b7-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="532b7-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="532b7-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="532b7-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="532b7-140">Schema name</span></span>  <br/> |<span data-ttu-id="532b7-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="532b7-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="532b7-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="532b7-142">Validation file</span></span>  <br/> |<span data-ttu-id="532b7-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="532b7-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="532b7-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="532b7-144">Can be empty</span></span>  <br/> |<span data-ttu-id="532b7-145">False</span><span class="sxs-lookup"><span data-stu-id="532b7-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="532b7-146">См. также</span><span class="sxs-lookup"><span data-stu-id="532b7-146">See also</span></span>

- [<span data-ttu-id="532b7-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="532b7-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

