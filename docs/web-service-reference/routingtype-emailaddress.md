---
title: RoutingType (EmailAddress)
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
description: Элемент RoutingType представляет протокол маршрутизации для получателя.
ms.openlocfilehash: a0a6cf312bcb1d4b4818a82bc8d8d3e3f33ad6f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835255"
---
# <a name="routingtype-emailaddress"></a><span data-ttu-id="a352c-103">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a352c-103">RoutingType (EmailAddress)</span></span>

<span data-ttu-id="a352c-104">Элемент **RoutingType** представляет протокол маршрутизации для получателя.</span><span class="sxs-lookup"><span data-stu-id="a352c-104">The **RoutingType** element represents the routing protocol for the recipient.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="a352c-105">**string**</span><span class="sxs-lookup"><span data-stu-id="a352c-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a352c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a352c-106">Attributes and elements</span></span>

<span data-ttu-id="a352c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a352c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a352c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a352c-108">Attributes</span></span>

<span data-ttu-id="a352c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a352c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a352c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a352c-110">Child elements</span></span>

<span data-ttu-id="a352c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a352c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a352c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a352c-112">Parent elements</span></span>

|<span data-ttu-id="a352c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a352c-113">**Element**</span></span>|<span data-ttu-id="a352c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a352c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a352c-115">Электронной почты (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a352c-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="a352c-116">Указывает адрес электронной почты объекта MailboxData.</span><span class="sxs-lookup"><span data-stu-id="a352c-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="a352c-117">Данный элемент используется в [операции GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a352c-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/><br/> <span data-ttu-id="a352c-118">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="a352c-118">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="a352c-119">Почтовый ящик (доступность)</span><span class="sxs-lookup"><span data-stu-id="a352c-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="a352c-120">Представляет пользователя почтового ящика для SetUserOofSettings или GetUserOofSettings запроса.</span><span class="sxs-lookup"><span data-stu-id="a352c-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="a352c-121">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a352c-121">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a352c-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a352c-122">Text value</span></span>

<span data-ttu-id="a352c-123">Текстовое значение является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a352c-123">A text value is optional.</span></span> <span data-ttu-id="a352c-124">Допустимые значения — SMTP.</span><span class="sxs-lookup"><span data-stu-id="a352c-124">The only valid value is SMTP.</span></span> <span data-ttu-id="a352c-125">Если значение не указано, используется значение по умолчанию SMTP.</span><span class="sxs-lookup"><span data-stu-id="a352c-125">If no value is provided, the default value of SMTP is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a352c-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="a352c-126">Remarks</span></span>

<span data-ttu-id="a352c-127">Этот элемент может возникнуть только один раз в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="a352c-127">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="a352c-128">Этот элемент не требуется.</span><span class="sxs-lookup"><span data-stu-id="a352c-128">This element is not required.</span></span> <span data-ttu-id="a352c-129">Этот элемент существует для включения новых протоколов.</span><span class="sxs-lookup"><span data-stu-id="a352c-129">This element exists for the inclusion of future protocols.</span></span> <span data-ttu-id="a352c-130">Другой элемент **RoutingType** используется для доступа к элементам в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a352c-130">Another **RoutingType** element is used for accessing items in a user's mailbox.</span></span> 
  
<span data-ttu-id="a352c-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a352c-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a352c-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a352c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a352c-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a352c-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a352c-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a352c-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a352c-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a352c-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a352c-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a352c-136">Validation File</span></span>  <br/> |<span data-ttu-id="a352c-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a352c-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a352c-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a352c-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a352c-139">False</span><span class="sxs-lookup"><span data-stu-id="a352c-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a352c-140">См. также</span><span class="sxs-lookup"><span data-stu-id="a352c-140">See also</span></span>

- [<span data-ttu-id="a352c-141">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a352c-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="a352c-142">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="a352c-142">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="a352c-143">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="a352c-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

