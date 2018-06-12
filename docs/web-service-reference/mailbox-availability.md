---
title: Почтовый ящик (доступность)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: Представляет элемент почтового ящика пользователя почтового ящика для SetUserOofSettings или GetUserOofSettings запроса.
ms.openlocfilehash: 2e901ae0df56542f56f247184254294735018468
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834254"
---
# <a name="mailbox-availability"></a><span data-ttu-id="b8a75-103">Почтовый ящик (доступность)</span><span class="sxs-lookup"><span data-stu-id="b8a75-103">Mailbox (Availability)</span></span>

<span data-ttu-id="b8a75-104">Представляет элемент **почтового ящика** пользователя почтового ящика для SetUserOofSettings или GetUserOofSettings запроса.</span><span class="sxs-lookup"><span data-stu-id="b8a75-104">The **Mailbox** element represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span> 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

<span data-ttu-id="b8a75-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="b8a75-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b8a75-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b8a75-106">Attributes and elements</span></span>

<span data-ttu-id="b8a75-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b8a75-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8a75-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b8a75-108">Attributes</span></span>

<span data-ttu-id="b8a75-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b8a75-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8a75-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b8a75-110">Child elements</span></span>

|<span data-ttu-id="b8a75-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b8a75-111">**Element**</span></span>|<span data-ttu-id="b8a75-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b8a75-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8a75-113">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="b8a75-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="b8a75-114">Представляет отображаемое имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b8a75-114">Represents the display name of the mailbox user.</span></span> <span data-ttu-id="b8a75-115">Этот элемент является необязательным в SetUserOofSettingsRequest.</span><span class="sxs-lookup"><span data-stu-id="b8a75-115">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="b8a75-116">GetUserOofSettingsRequest возвращает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="b8a75-116">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
|[<span data-ttu-id="b8a75-117">Адрес (строка)</span><span class="sxs-lookup"><span data-stu-id="b8a75-117">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="b8a75-118">Представляет адрес электронной почты пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b8a75-118">Represents the e-mail address of the mailbox user.</span></span> <span data-ttu-id="b8a75-119">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8a75-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="b8a75-120">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="b8a75-120">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="b8a75-121">Представляет протокол маршрутизации для сообщения.</span><span class="sxs-lookup"><span data-stu-id="b8a75-121">Represents the routing protocol for the message.</span></span> <span data-ttu-id="b8a75-122">Этот элемент является необязательным в SetUserOofSettingsRequest.</span><span class="sxs-lookup"><span data-stu-id="b8a75-122">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="b8a75-123">GetUserOofSettingsRequest возвращает этот элемент.</span><span class="sxs-lookup"><span data-stu-id="b8a75-123">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8a75-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b8a75-124">Parent elements</span></span>

|<span data-ttu-id="b8a75-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b8a75-125">**Element**</span></span>|<span data-ttu-id="b8a75-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b8a75-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8a75-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="b8a75-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md) <br/> |<span data-ttu-id="b8a75-128">Используется для получения параметров из Office (OOF) и сообщения пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b8a75-128">Used to get a mailbox user's Out of Office (OOF) settings and messages.</span></span>  <br/> <span data-ttu-id="b8a75-129">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="b8a75-129">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[<span data-ttu-id="b8a75-130">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="b8a75-130">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="b8a75-131">Используется для задания параметров об отсутствии на работе и сообщения пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b8a75-131">Used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="b8a75-132">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="b8a75-132">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b8a75-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="b8a75-133">Remarks</span></span>

<span data-ttu-id="b8a75-134">Адрес электронной почты используется для идентификации в папке календаря, содержащим параметры об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="b8a75-134">The e-mail address is used to identify the calendar folder that contains the OOF settings.</span></span> 
  
<span data-ttu-id="b8a75-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b8a75-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8a75-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b8a75-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8a75-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b8a75-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8a75-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b8a75-138">Schema Name</span></span>  <br/> |<span data-ttu-id="b8a75-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b8a75-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="b8a75-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b8a75-140">Validation File</span></span>  <br/> |<span data-ttu-id="b8a75-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b8a75-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8a75-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b8a75-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8a75-143">False</span><span class="sxs-lookup"><span data-stu-id="b8a75-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8a75-144">См. также</span><span class="sxs-lookup"><span data-stu-id="b8a75-144">See also</span></span>

- [<span data-ttu-id="b8a75-145">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="b8a75-145">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="b8a75-146">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="b8a75-146">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

