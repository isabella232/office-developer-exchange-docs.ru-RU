---
title: Address (строка)
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
description: Элемент Address представляет адрес электронной почты пользователя почтового ящика.
ms.openlocfilehash: 839107050f22df5c00cb4dea9c531563df52933d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463645"
---
# <a name="address-string"></a><span data-ttu-id="f51f2-103">Address (строка)</span><span class="sxs-lookup"><span data-stu-id="f51f2-103">Address (string)</span></span>

<span data-ttu-id="f51f2-104">Элемент **Address** представляет адрес электронной почты пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f51f2-104">The **Address** element represents the e-mail address of the mailbox user.</span></span> 
  
```xml
<Address>...</Address>
```

 <span data-ttu-id="f51f2-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="f51f2-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f51f2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f51f2-106">Attributes and elements</span></span>

<span data-ttu-id="f51f2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f51f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f51f2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f51f2-108">Attributes</span></span>

<span data-ttu-id="f51f2-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f51f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f51f2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f51f2-110">Child elements</span></span>

<span data-ttu-id="f51f2-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f51f2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f51f2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f51f2-112">Parent elements</span></span>

|<span data-ttu-id="f51f2-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f51f2-113">**Element**</span></span>|<span data-ttu-id="f51f2-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f51f2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f51f2-115">Электронная почта (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="f51f2-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="f51f2-116">Задает адрес электронной почты объекта MailboxData.</span><span class="sxs-lookup"><span data-stu-id="f51f2-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="f51f2-117">Этот элемент используется в [операции GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f51f2-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span><br/><br/> <span data-ttu-id="f51f2-118">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="f51f2-118">The following is the XPath to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="f51f2-119">Mailbox (доступность)</span><span class="sxs-lookup"><span data-stu-id="f51f2-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="f51f2-120">Представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="f51f2-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span><br/><br/>  <span data-ttu-id="f51f2-121">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="f51f2-121">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f51f2-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f51f2-122">Text value</span></span>

<span data-ttu-id="f51f2-123">При использовании этого элемента необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="f51f2-123">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f51f2-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="f51f2-124">Remarks</span></span>

<span data-ttu-id="f51f2-125">Этот элемент может встречаться не более одного раз в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) и элементе [Mailbox (Availability)](mailbox-availability.md) .</span><span class="sxs-lookup"><span data-stu-id="f51f2-125">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element and the [Mailbox (Availability)](mailbox-availability.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f51f2-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f51f2-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f51f2-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f51f2-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f51f2-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f51f2-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f51f2-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f51f2-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f51f2-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f51f2-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="f51f2-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f51f2-131">Validation File</span></span>  <br/> |<span data-ttu-id="f51f2-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f51f2-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f51f2-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f51f2-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="f51f2-134">False</span><span class="sxs-lookup"><span data-stu-id="f51f2-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f51f2-135">См. также</span><span class="sxs-lookup"><span data-stu-id="f51f2-135">See also</span></span>

- [<span data-ttu-id="f51f2-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f51f2-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="f51f2-137">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="f51f2-137">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="f51f2-138">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="f51f2-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="f51f2-139">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="f51f2-139">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="f51f2-140">жетусеруфсеттингсрекуест</span><span class="sxs-lookup"><span data-stu-id="f51f2-140">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
- [<span data-ttu-id="f51f2-141">сетусеруфсеттингсрекуест</span><span class="sxs-lookup"><span data-stu-id="f51f2-141">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
- [<span data-ttu-id="f51f2-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="f51f2-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

