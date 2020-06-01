---
title: Mailbox (доступность)
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
description: Элемент Mailbox представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.
ms.openlocfilehash: 1bda6e8b90551b86b4e1c2711ac25693a65e5410
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458077"
---
# <a name="mailbox-availability"></a><span data-ttu-id="2caf5-103">Mailbox (доступность)</span><span class="sxs-lookup"><span data-stu-id="2caf5-103">Mailbox (Availability)</span></span>

<span data-ttu-id="2caf5-104">Элемент **Mailbox** представляет пользователя почтового ящика для запроса SetUserOofSettings или GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="2caf5-104">The **Mailbox** element represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span> 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

<span data-ttu-id="2caf5-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="2caf5-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2caf5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2caf5-106">Attributes and elements</span></span>

<span data-ttu-id="2caf5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2caf5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2caf5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2caf5-108">Attributes</span></span>

<span data-ttu-id="2caf5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2caf5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2caf5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2caf5-110">Child elements</span></span>

|<span data-ttu-id="2caf5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2caf5-111">**Element**</span></span>|<span data-ttu-id="2caf5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2caf5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2caf5-113">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2caf5-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="2caf5-114">Представляет отображаемое имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2caf5-114">Represents the display name of the mailbox user.</span></span> <span data-ttu-id="2caf5-115">Этот элемент является необязательным в Сетусеруфсеттингсрекуест.</span><span class="sxs-lookup"><span data-stu-id="2caf5-115">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="2caf5-116">Жетусеруфсеттингсрекуест будет возвращать этот элемент.</span><span class="sxs-lookup"><span data-stu-id="2caf5-116">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
|[<span data-ttu-id="2caf5-117">Address (строка)</span><span class="sxs-lookup"><span data-stu-id="2caf5-117">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="2caf5-118">Представляет адрес электронной почты пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2caf5-118">Represents the e-mail address of the mailbox user.</span></span> <span data-ttu-id="2caf5-119">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="2caf5-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="2caf5-120">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2caf5-120">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="2caf5-121">Представляет протокол маршрутизации для сообщения.</span><span class="sxs-lookup"><span data-stu-id="2caf5-121">Represents the routing protocol for the message.</span></span> <span data-ttu-id="2caf5-122">Этот элемент является необязательным в Сетусеруфсеттингсрекуест.</span><span class="sxs-lookup"><span data-stu-id="2caf5-122">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="2caf5-123">Жетусеруфсеттингсрекуест будет возвращать этот элемент.</span><span class="sxs-lookup"><span data-stu-id="2caf5-123">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2caf5-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2caf5-124">Parent elements</span></span>

|<span data-ttu-id="2caf5-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2caf5-125">**Element**</span></span>|<span data-ttu-id="2caf5-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2caf5-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2caf5-127">жетусеруфсеттингсрекуест</span><span class="sxs-lookup"><span data-stu-id="2caf5-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md) <br/> |<span data-ttu-id="2caf5-128">Используется для получения параметров и сообщений пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2caf5-128">Used to get a mailbox user's Out of Office (OOF) settings and messages.</span></span>  <br/> <span data-ttu-id="2caf5-129">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="2caf5-129">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[<span data-ttu-id="2caf5-130">сетусеруфсеттингсрекуест</span><span class="sxs-lookup"><span data-stu-id="2caf5-130">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="2caf5-131">Используется для настройки параметров и сообщений пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2caf5-131">Used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="2caf5-132">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="2caf5-132">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2caf5-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="2caf5-133">Remarks</span></span>

<span data-ttu-id="2caf5-134">Адрес электронной почты используется для определения папки календаря, в которой содержатся параметры отсутствия на работе.</span><span class="sxs-lookup"><span data-stu-id="2caf5-134">The e-mail address is used to identify the calendar folder that contains the OOF settings.</span></span> 
  
<span data-ttu-id="2caf5-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2caf5-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2caf5-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2caf5-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2caf5-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2caf5-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2caf5-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2caf5-138">Schema Name</span></span>  <br/> |<span data-ttu-id="2caf5-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2caf5-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="2caf5-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2caf5-140">Validation File</span></span>  <br/> |<span data-ttu-id="2caf5-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2caf5-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2caf5-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2caf5-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="2caf5-143">False</span><span class="sxs-lookup"><span data-stu-id="2caf5-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2caf5-144">См. также</span><span class="sxs-lookup"><span data-stu-id="2caf5-144">See also</span></span>

- [<span data-ttu-id="2caf5-145">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="2caf5-145">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="2caf5-146">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="2caf5-146">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

