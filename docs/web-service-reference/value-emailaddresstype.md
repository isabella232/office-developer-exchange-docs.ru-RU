---
title: Значение (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 24eaa473-0024-47e2-b7d2-051d5dd4f53c
description: Элемент value указывает значение EmailAddress, связанное с массивом сопоставлений.
ms.openlocfilehash: 45af2aaab7d2475ae46ae24ed13b1435f5b352c6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467601"
---
# <a name="value-emailaddresstype"></a><span data-ttu-id="18dc4-103">Значение (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="18dc4-103">Value (EmailAddressType)</span></span>

<span data-ttu-id="18dc4-104">Элемент **value** указывает значение **EmailAddress** , связанное с массивом сопоставлений.</span><span class="sxs-lookup"><span data-stu-id="18dc4-104">The **Value** element specifies the value of an **EmailAddress** associated with an attributions array.</span></span> 
  
```XML
<Value>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
   <OriginalDisplayName/>
</Value>
```

<span data-ttu-id="18dc4-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="18dc4-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="18dc4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="18dc4-106">Attributes and elements</span></span>

<span data-ttu-id="18dc4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="18dc4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18dc4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="18dc4-108">Attributes</span></span>

<span data-ttu-id="18dc4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="18dc4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18dc4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="18dc4-110">Child elements</span></span>

<span data-ttu-id="18dc4-111">[Имя (строка)](name-string.md)  |  [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md)  |  [Раутингтипе (EmailAddressType)](routingtype-emailaddresstype.md)  |  [MailboxType](mailboxtype.md)  |  [ItemId](itemid.md)  |  [Оригиналдисплайнаме](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="18dc4-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18dc4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="18dc4-112">Parent elements</span></span>

[<span data-ttu-id="18dc4-113">емаиладдрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="18dc4-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="18dc4-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="18dc4-114">Remarks</span></span>

<span data-ttu-id="18dc4-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="18dc4-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="18dc4-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="18dc4-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18dc4-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="18dc4-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18dc4-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="18dc4-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18dc4-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="18dc4-119">Schema name</span></span>  <br/> |<span data-ttu-id="18dc4-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="18dc4-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="18dc4-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="18dc4-121">Validation file</span></span>  <br/> |<span data-ttu-id="18dc4-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="18dc4-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18dc4-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="18dc4-123">Can be empty</span></span>  <br/> |<span data-ttu-id="18dc4-124">false</span><span class="sxs-lookup"><span data-stu-id="18dc4-124">false</span></span>  <br/> |
   

