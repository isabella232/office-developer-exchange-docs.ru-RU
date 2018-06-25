---
title: EmailAddress (GetPersonaType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 052055b5-4630-40ed-9b24-9e7f4bf7ba1d
description: Элемент EmailAddress (GetPersonaType) указывает адрес электронной почты, связанный с пользователя.
ms.openlocfilehash: a28a4a61a9719875fe99e1c950bcd3ec3af9ab13
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762275"
---
# <a name="emailaddress-getpersonatype"></a><span data-ttu-id="443ee-103">EmailAddress (GetPersonaType)</span><span class="sxs-lookup"><span data-stu-id="443ee-103">EmailAddress (GetPersonaType)</span></span>

<span data-ttu-id="443ee-104">Элемент **EmailAddress (GetPersonaType)** указывает адрес электронной почты, связанный с пользователя.</span><span class="sxs-lookup"><span data-stu-id="443ee-104">The **EmailAddress (GetPersonaType)** element specifies the email address associated with the persona.</span></span> 
  
```XML
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
    <OriginalDisplayName></OriginalDisplayName>
</EmailAddress>>
```

 <span data-ttu-id="443ee-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="443ee-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="443ee-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="443ee-106">Attributes and elements</span></span>

<span data-ttu-id="443ee-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="443ee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="443ee-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="443ee-108">Attributes</span></span>

<span data-ttu-id="443ee-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="443ee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="443ee-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="443ee-110">Child elements</span></span>

<span data-ttu-id="443ee-111">[Имя (строка)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="443ee-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="443ee-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="443ee-112">Parent elements</span></span>

[<span data-ttu-id="443ee-113">GetPersona</span><span class="sxs-lookup"><span data-stu-id="443ee-113">GetPersona</span></span>](getpersona.md)
  
## <a name="remarks"></a><span data-ttu-id="443ee-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="443ee-114">Remarks</span></span>

<span data-ttu-id="443ee-115">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="443ee-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="443ee-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="443ee-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="443ee-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="443ee-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="443ee-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="443ee-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="443ee-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="443ee-119">Schema Name</span></span>  <br/> |<span data-ttu-id="443ee-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="443ee-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="443ee-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="443ee-121">Validation File</span></span>  <br/> |<span data-ttu-id="443ee-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="443ee-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="443ee-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="443ee-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="443ee-124">True</span><span class="sxs-lookup"><span data-stu-id="443ee-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="443ee-125">См. также</span><span class="sxs-lookup"><span data-stu-id="443ee-125">See also</span></span>

- [<span data-ttu-id="443ee-126">GetPersona</span><span class="sxs-lookup"><span data-stu-id="443ee-126">GetPersona</span></span>](getpersona.md)
- [<span data-ttu-id="443ee-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="443ee-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

