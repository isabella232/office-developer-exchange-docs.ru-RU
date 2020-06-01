---
title: Раутингтипе (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: Элемент Раутингтипе представляет протокол маршрутизации для получателя.
ms.openlocfilehash: 2193e72c38c687669f6e052b4d2526029aa89d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459036"
---
# <a name="routingtype-emailaddress"></a><span data-ttu-id="4ac7c-103">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="4ac7c-103">RoutingType (EmailAddress)</span></span>

<span data-ttu-id="4ac7c-104">Элемент **раутингтипе** представляет протокол маршрутизации для получателя.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-104">The **RoutingType** element represents the routing protocol for the recipient.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="4ac7c-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="4ac7c-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ac7c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4ac7c-106">Attributes and elements</span></span>

<span data-ttu-id="4ac7c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ac7c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4ac7c-108">Attributes</span></span>

<span data-ttu-id="4ac7c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ac7c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4ac7c-110">Child elements</span></span>

<span data-ttu-id="4ac7c-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ac7c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4ac7c-112">Parent elements</span></span>

|<span data-ttu-id="4ac7c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4ac7c-113">**Element**</span></span>|<span data-ttu-id="4ac7c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ac7c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ac7c-115">Электронная почта (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4ac7c-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="4ac7c-116">Задает адрес электронной почты объекта MailboxData.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="4ac7c-117">Этот элемент используется в [операции GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4ac7c-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/><br/> <span data-ttu-id="4ac7c-118">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="4ac7c-118">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="4ac7c-119">Mailbox (доступность)</span><span class="sxs-lookup"><span data-stu-id="4ac7c-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="4ac7c-120">Представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="4ac7c-121">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-121">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ac7c-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4ac7c-122">Text value</span></span>

<span data-ttu-id="4ac7c-123">Текстовое значение является необязательным.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-123">A text value is optional.</span></span> <span data-ttu-id="4ac7c-124">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-124">The following are the possible values:</span></span>

* <span data-ttu-id="4ac7c-125">SMTP</span><span class="sxs-lookup"><span data-stu-id="4ac7c-125">SMTP</span></span>
* <span data-ttu-id="4ac7c-126">Пример</span><span class="sxs-lookup"><span data-stu-id="4ac7c-126">EX</span></span>

<span data-ttu-id="4ac7c-127">Если значение не указано, используется значение по умолчанию (SMTP).</span><span class="sxs-lookup"><span data-stu-id="4ac7c-127">If no value is provided, the default value of SMTP is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ac7c-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="4ac7c-128">Remarks</span></span>

<span data-ttu-id="4ac7c-129">Этот элемент может встречаться в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) не чаще, чем один раз.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-129">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="4ac7c-130">Этот элемент не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-130">This element is not required.</span></span> <span data-ttu-id="4ac7c-131">Этот элемент существует для включения будущих протоколов.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-131">This element exists for the inclusion of future protocols.</span></span> <span data-ttu-id="4ac7c-132">Другой элемент **раутингтипе** используется для доступа к элементам в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-132">Another **RoutingType** element is used for accessing items in a user's mailbox.</span></span> 
  
<span data-ttu-id="4ac7c-133">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ac7c-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ac7c-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4ac7c-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ac7c-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4ac7c-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ac7c-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4ac7c-136">Schema Name</span></span>  <br/> |<span data-ttu-id="4ac7c-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4ac7c-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ac7c-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4ac7c-138">Validation File</span></span>  <br/> |<span data-ttu-id="4ac7c-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4ac7c-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ac7c-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4ac7c-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ac7c-141">False</span><span class="sxs-lookup"><span data-stu-id="4ac7c-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ac7c-142">См. также</span><span class="sxs-lookup"><span data-stu-id="4ac7c-142">See also</span></span>

- [<span data-ttu-id="4ac7c-143">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4ac7c-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="4ac7c-144">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="4ac7c-144">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="4ac7c-145">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="4ac7c-145">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

