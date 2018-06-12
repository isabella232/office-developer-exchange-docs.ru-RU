---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: Элемент EmailAddress указывает полностью разрешенной SMTP-адрес для почтового ящика сайта или связанного пользователя.
ms.openlocfilehash: c31a37fc0dbdcc2b501b82346a17a0a3b4775556
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762274"
---
# <a name="emailaddress-emailaddresstype"></a><span data-ttu-id="93927-103">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="93927-103">EmailAddress (EmailAddressType)</span></span>

<span data-ttu-id="93927-104">Элемент **EmailAddress** указывает полностью разрешенной SMTP-адрес для почтового ящика сайта или связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="93927-104">The **EmailAddress** element specifies the fully resolved SMTP address for the site mailbox or the associated persona.</span></span> 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 <span data-ttu-id="93927-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="93927-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93927-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93927-106">Attributes and elements</span></span>

<span data-ttu-id="93927-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="93927-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93927-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93927-108">Attributes</span></span>

<span data-ttu-id="93927-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="93927-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93927-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93927-110">Child elements</span></span>

|<span data-ttu-id="93927-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93927-111">**Element**</span></span>|<span data-ttu-id="93927-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93927-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93927-113">Имя (строка)</span><span class="sxs-lookup"><span data-stu-id="93927-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="93927-114">Указывает имя уточнения поиска или ключ или имя электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="93927-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="93927-115">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="93927-115">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="93927-116">Определяет основной SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="93927-116">Defines the primary SMTP address of a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="93927-117">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="93927-117">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md) <br/> |<span data-ttu-id="93927-118">Указывает тип маршрутизации адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="93927-118">Specifies the routing type of an email address.</span></span>  <br/> |
|[<span data-ttu-id="93927-119">MailboxType</span><span class="sxs-lookup"><span data-stu-id="93927-119">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="93927-120">Представляет тип почтового ящика, который соответствует адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="93927-120">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="93927-121">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="93927-121">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="93927-122">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="93927-122">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93927-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93927-123">Parent elements</span></span>

|<span data-ttu-id="93927-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93927-124">**Element**</span></span>|<span data-ttu-id="93927-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93927-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93927-126">Пользователь</span><span class="sxs-lookup"><span data-stu-id="93927-126">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="93927-127">Задает набор пользователя данные, возвращаемые запросом **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="93927-127">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93927-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="93927-128">Text value</span></span>

<span data-ttu-id="93927-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="93927-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93927-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="93927-130">Remarks</span></span>

<span data-ttu-id="93927-131">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="93927-131">This element is optional.</span></span>
  
<span data-ttu-id="93927-132">Элемент **EmailAddress** используется для клиентов, относящихся к Exchange Online и версий Microsoft Exchange Server, начиная с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="93927-132">The **EmailAddress** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="93927-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93927-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93927-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93927-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93927-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93927-135">Schema Name</span></span>  <br/> |<span data-ttu-id="93927-136">Схема типа</span><span class="sxs-lookup"><span data-stu-id="93927-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="93927-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93927-137">Validation File</span></span>  <br/> |<span data-ttu-id="93927-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="93927-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="93927-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93927-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="93927-140">См. также</span><span class="sxs-lookup"><span data-stu-id="93927-140">See also</span></span>

- [<span data-ttu-id="93927-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="93927-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

