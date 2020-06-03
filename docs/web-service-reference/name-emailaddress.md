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
ms.openlocfilehash: 2c6b29f1b069f9cc72ac84e7aebfff99437e630a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466957"
---
# <a name="name-emailaddress"></a><span data-ttu-id="7fc1b-103">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="7fc1b-103">Name (EmailAddress)</span></span>

<span data-ttu-id="7fc1b-104">Элемент **Name** представляет отображаемое имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-104">The **Name** element represents the display name of the mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="7fc1b-105">**String**</span><span class="sxs-lookup"><span data-stu-id="7fc1b-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7fc1b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7fc1b-106">Attributes and elements</span></span>

<span data-ttu-id="7fc1b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7fc1b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7fc1b-108">Attributes</span></span>

<span data-ttu-id="7fc1b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7fc1b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7fc1b-110">Child elements</span></span>

<span data-ttu-id="7fc1b-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7fc1b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7fc1b-112">Parent elements</span></span>

|<span data-ttu-id="7fc1b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7fc1b-113">**Element**</span></span>|<span data-ttu-id="7fc1b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7fc1b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7fc1b-115">Электронная почта (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7fc1b-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="7fc1b-116">Представляет пользователя почтового ящика для запроса GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-116">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> <br/><span data-ttu-id="7fc1b-117">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="7fc1b-117">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="7fc1b-118">Mailbox (доступность)</span><span class="sxs-lookup"><span data-stu-id="7fc1b-118">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="7fc1b-119">Представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-119">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="7fc1b-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-120">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7fc1b-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7fc1b-121">Text value</span></span>

<span data-ttu-id="7fc1b-122">При использовании этого элемента необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-122">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7fc1b-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="7fc1b-123">Remarks</span></span>

<span data-ttu-id="7fc1b-124">Этот элемент может встречаться в элементе [электронной почты (EmailAddressType)](email-emailaddresstype.md) не чаще, чем один раз.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-124">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="7fc1b-125">Этот элемент не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-125">This element is not required.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7fc1b-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7fc1b-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="7fc1b-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7fc1b-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7fc1b-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7fc1b-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7fc1b-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7fc1b-129">Schema Name</span></span>  <br/> |<span data-ttu-id="7fc1b-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7fc1b-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="7fc1b-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7fc1b-131">Validation File</span></span>  <br/> |<span data-ttu-id="7fc1b-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7fc1b-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7fc1b-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7fc1b-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="7fc1b-134">False</span><span class="sxs-lookup"><span data-stu-id="7fc1b-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7fc1b-135">См. также</span><span class="sxs-lookup"><span data-stu-id="7fc1b-135">See also</span></span>

- [<span data-ttu-id="7fc1b-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7fc1b-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="7fc1b-137">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="7fc1b-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="7fc1b-138">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="7fc1b-138">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

