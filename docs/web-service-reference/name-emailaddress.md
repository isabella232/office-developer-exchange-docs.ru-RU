---
title: Имя (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: c719c55f-d625-4e64-846f-50ac91881443
description: Элемент Name представляет отображаемое имя пользователя почтового ящика.
ms.openlocfilehash: 6d30f06c3bfd77d2715798349ab084cdf81f21a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834505"
---
# <a name="name-emailaddress"></a><span data-ttu-id="858d7-103">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="858d7-103">Name (EmailAddress)</span></span>

<span data-ttu-id="858d7-104">Элемент **Name** представляет отображаемое имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="858d7-104">The **Name** element represents the display name of the mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="858d7-105">**Строка**</span><span class="sxs-lookup"><span data-stu-id="858d7-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="858d7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="858d7-106">Attributes and elements</span></span>

<span data-ttu-id="858d7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="858d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="858d7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="858d7-108">Attributes</span></span>

<span data-ttu-id="858d7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="858d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="858d7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="858d7-110">Child elements</span></span>

<span data-ttu-id="858d7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="858d7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="858d7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="858d7-112">Parent elements</span></span>

|<span data-ttu-id="858d7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="858d7-113">**Element**</span></span>|<span data-ttu-id="858d7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="858d7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="858d7-115">Электронной почты (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="858d7-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="858d7-116">Представляет пользователя почтового ящика для запроса GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="858d7-116">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> <br/><span data-ttu-id="858d7-117">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="858d7-117">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="858d7-118">Почтовый ящик (доступность)</span><span class="sxs-lookup"><span data-stu-id="858d7-118">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="858d7-119">Представляет пользователя почтового ящика для SetUserOofSettings или GetUserOofSettings запроса.</span><span class="sxs-lookup"><span data-stu-id="858d7-119">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="858d7-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="858d7-120">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="858d7-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="858d7-121">Text value</span></span>

<span data-ttu-id="858d7-122">Текстовое значение является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="858d7-122">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="858d7-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="858d7-123">Remarks</span></span>

<span data-ttu-id="858d7-124">Этот элемент может возникнуть только один раз в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="858d7-124">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="858d7-125">Этот элемент не требуется.</span><span class="sxs-lookup"><span data-stu-id="858d7-125">This element is not required.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="858d7-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="858d7-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="858d7-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="858d7-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="858d7-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="858d7-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="858d7-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="858d7-129">Schema Name</span></span>  <br/> |<span data-ttu-id="858d7-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="858d7-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="858d7-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="858d7-131">Validation File</span></span>  <br/> |<span data-ttu-id="858d7-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="858d7-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="858d7-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="858d7-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="858d7-134">False</span><span class="sxs-lookup"><span data-stu-id="858d7-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="858d7-135">См. также</span><span class="sxs-lookup"><span data-stu-id="858d7-135">See also</span></span>

- [<span data-ttu-id="858d7-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="858d7-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="858d7-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="858d7-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="858d7-138">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="858d7-138">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

