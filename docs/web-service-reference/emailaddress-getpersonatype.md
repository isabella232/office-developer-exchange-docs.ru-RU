---
title: EmailAddress (Жетперсонатипе)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 052055b5-4630-40ed-9b24-9e7f4bf7ba1d
description: Элемент EmailAddress (Жетперсонатипе) указывает адрес электронной почты, связанный с персонажом.
ms.openlocfilehash: b58f61202cd94ff282b21138b47b40887b38752a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463456"
---
# <a name="emailaddress-getpersonatype"></a><span data-ttu-id="a4356-103">EmailAddress (Жетперсонатипе)</span><span class="sxs-lookup"><span data-stu-id="a4356-103">EmailAddress (GetPersonaType)</span></span>

<span data-ttu-id="a4356-104">Элемент **EmailAddress (жетперсонатипе)** указывает адрес электронной почты, связанный с персонажом.</span><span class="sxs-lookup"><span data-stu-id="a4356-104">The **EmailAddress (GetPersonaType)** element specifies the email address associated with the persona.</span></span> 
  
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

 <span data-ttu-id="a4356-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="a4356-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4356-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a4356-106">Attributes and elements</span></span>

<span data-ttu-id="a4356-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a4356-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4356-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a4356-108">Attributes</span></span>

<span data-ttu-id="a4356-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a4356-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4356-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a4356-110">Child elements</span></span>

<span data-ttu-id="a4356-111">[Имя (строка)](name-string.md)  |  [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md)  |  [Раутингтипе (EmailAddressType)](routingtype-emailaddresstype.md)  |  [MailboxType](mailboxtype.md)  |  [ItemId](itemid.md)  |  [Оригиналдисплайнаме](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="a4356-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4356-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a4356-112">Parent elements</span></span>

[<span data-ttu-id="a4356-113">GetPersona</span><span class="sxs-lookup"><span data-stu-id="a4356-113">GetPersona</span></span>](getpersona.md)
  
## <a name="remarks"></a><span data-ttu-id="a4356-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="a4356-114">Remarks</span></span>

<span data-ttu-id="a4356-115">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a4356-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="a4356-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a4356-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4356-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a4356-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4356-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a4356-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a4356-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a4356-119">Schema Name</span></span>  <br/> |<span data-ttu-id="a4356-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a4356-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a4356-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a4356-121">Validation File</span></span>  <br/> |<span data-ttu-id="a4356-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a4356-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a4356-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a4356-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="a4356-124">True</span><span class="sxs-lookup"><span data-stu-id="a4356-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4356-125">См. также</span><span class="sxs-lookup"><span data-stu-id="a4356-125">See also</span></span>

- [<span data-ttu-id="a4356-126">GetPersona</span><span class="sxs-lookup"><span data-stu-id="a4356-126">GetPersona</span></span>](getpersona.md)
- [<span data-ttu-id="a4356-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a4356-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

