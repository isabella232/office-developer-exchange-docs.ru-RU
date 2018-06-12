---
title: Адрес (строка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: a3cdfcbd-d0c5-46d6-8daa-52405fc63ff0
description: Элемент адрес — адрес электронной почты пользователя почтового ящика.
ms.openlocfilehash: 07c634d6166d88a8912bc66081a13671e600c801
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761357"
---
# <a name="address-string"></a><span data-ttu-id="fc40a-103">Адрес (строка)</span><span class="sxs-lookup"><span data-stu-id="fc40a-103">Address (string)</span></span>

<span data-ttu-id="fc40a-104">Элемент **адрес** — адрес электронной почты пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="fc40a-104">The **Address** element represents the e-mail address of the mailbox user.</span></span> 
  
```xml
<Address>...</Address>
```

 <span data-ttu-id="fc40a-105">**string**</span><span class="sxs-lookup"><span data-stu-id="fc40a-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc40a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fc40a-106">Attributes and elements</span></span>

<span data-ttu-id="fc40a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fc40a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc40a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fc40a-108">Attributes</span></span>

<span data-ttu-id="fc40a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc40a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc40a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fc40a-110">Child elements</span></span>

<span data-ttu-id="fc40a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc40a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc40a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fc40a-112">Parent elements</span></span>

|<span data-ttu-id="fc40a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc40a-113">**Element**</span></span>|<span data-ttu-id="fc40a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc40a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc40a-115">Электронной почты (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="fc40a-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="fc40a-116">Указывает адрес электронной почты объекта MailboxData.</span><span class="sxs-lookup"><span data-stu-id="fc40a-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="fc40a-117">Данный элемент используется в [операции GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="fc40a-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span><br/><br/> <span data-ttu-id="fc40a-118">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="fc40a-118">The following is the XPath to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="fc40a-119">Почтовый ящик (доступность)</span><span class="sxs-lookup"><span data-stu-id="fc40a-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="fc40a-120">Представляет пользователя почтового ящика для SetUserOofSettings или GetUserOofSettings запроса.</span><span class="sxs-lookup"><span data-stu-id="fc40a-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span><br/><br/>  <span data-ttu-id="fc40a-121">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="fc40a-121">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc40a-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fc40a-122">Text value</span></span>

<span data-ttu-id="fc40a-123">Текстовое значение является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="fc40a-123">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc40a-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="fc40a-124">Remarks</span></span>

<span data-ttu-id="fc40a-125">Этот элемент может возникнуть только один раз в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) и элемент [почтового ящика (доступность)](mailbox-availability.md) .</span><span class="sxs-lookup"><span data-stu-id="fc40a-125">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element and the [Mailbox (Availability)](mailbox-availability.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fc40a-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fc40a-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="fc40a-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fc40a-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc40a-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fc40a-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc40a-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fc40a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="fc40a-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fc40a-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc40a-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fc40a-131">Validation File</span></span>  <br/> |<span data-ttu-id="fc40a-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fc40a-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc40a-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fc40a-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc40a-134">False</span><span class="sxs-lookup"><span data-stu-id="fc40a-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc40a-135">См. также</span><span class="sxs-lookup"><span data-stu-id="fc40a-135">See also</span></span>

- [<span data-ttu-id="fc40a-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="fc40a-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="fc40a-137">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="fc40a-137">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="fc40a-138">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="fc40a-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="fc40a-139">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="fc40a-139">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="fc40a-140">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="fc40a-140">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
- [<span data-ttu-id="fc40a-141">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="fc40a-141">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
- [<span data-ttu-id="fc40a-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="fc40a-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

