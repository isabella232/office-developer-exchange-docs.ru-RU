---
title: Отклик (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: Элемент Response содержит ответ на операцию GetUserSettings (SOAP), операцию Жетдомаинсеттингс (SOAP) или запрос операции Жетфедератионинформатион (SOAP).
ms.openlocfilehash: 90cb29dd4ce4026211a5b592f149c8190dc81d29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456418"
---
# <a name="response-soap"></a><span data-ttu-id="8d748-103">Отклик (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d748-103">Response (SOAP)</span></span>

<span data-ttu-id="8d748-104">Элемент **Response** содержит ответ на [операцию GetUserSettings (SOAP)](getusersettings-operation-soap.md), [операцию жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)или запрос [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="8d748-104">The **Response** element contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 <span data-ttu-id="8d748-105">**жетусерсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="8d748-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d748-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8d748-106">Attributes and elements</span></span>

<span data-ttu-id="8d748-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8d748-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d748-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8d748-108">Attributes</span></span>

<span data-ttu-id="8d748-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8d748-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d748-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8d748-110">Child elements</span></span>

|<span data-ttu-id="8d748-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8d748-111">**Element**</span></span>|<span data-ttu-id="8d748-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8d748-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d748-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d748-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="8d748-114">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="8d748-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="8d748-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d748-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="8d748-116">Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="8d748-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="8d748-117">Усерреспонсес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d748-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="8d748-118">Содержит параметры конфигурации для каждого запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d748-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8d748-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8d748-119">Parent elements</span></span>

|<span data-ttu-id="8d748-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8d748-120">**Element**</span></span>|<span data-ttu-id="8d748-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8d748-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d748-122">Жетусерсеттингсреспонсемессаже (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d748-122">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="8d748-123">Определяет ответ на [жетусерсеттингсрекуест (SOAP)](getusersettingsrequest-soap.md)</span><span class="sxs-lookup"><span data-stu-id="8d748-123">Defines a response to a [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span></span> <br/> |
|[<span data-ttu-id="8d748-124">Жетдомаинсеттингсреспонсемессаже (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d748-124">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="8d748-125">Определяет ответ на [жетдомаинсеттингсрекуест (SOAP)](getdomainsettingsrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="8d748-125">Defines a response to a [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="8d748-126">Жетфедератионинформатионреспонсемессаже (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d748-126">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="8d748-127">Определяет ответ на [жетфедератионинформатионрекуест (SOAP)](getfederationinformationrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="8d748-127">Defines a response to a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d748-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8d748-128">Text value</span></span>

<span data-ttu-id="8d748-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8d748-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d748-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8d748-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d748-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8d748-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="8d748-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8d748-132">Schema Name</span></span>  <br/> |<span data-ttu-id="8d748-133">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="8d748-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="8d748-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8d748-134">Validation File</span></span>  <br/> |<span data-ttu-id="8d748-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8d748-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8d748-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8d748-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d748-137">True</span><span class="sxs-lookup"><span data-stu-id="8d748-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d748-138">См. также</span><span class="sxs-lookup"><span data-stu-id="8d748-138">See also</span></span>



[<span data-ttu-id="8d748-139">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d748-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="8d748-140">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="8d748-140">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="8d748-141">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8d748-141">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

