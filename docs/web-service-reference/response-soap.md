---
title: Ответ (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: Элемент ответа содержит ответ на операцию GetUserSettings (SOAP), операция GetDomainSettings (SOAP) или запрос операции (SOAP) GetFederationInformation.
ms.openlocfilehash: 240c8e1f904ad685b51c1f657b2bc18e14fd985e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835179"
---
# <a name="response-soap"></a><span data-ttu-id="0e949-103">Ответ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e949-103">Response (SOAP)</span></span>

<span data-ttu-id="0e949-104">Элемент **ответа** содержит ответ на [операцию GetUserSettings (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)или запрос [GetFederationInformation операции (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="0e949-104">The **Response** element contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 <span data-ttu-id="0e949-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="0e949-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e949-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0e949-106">Attributes and elements</span></span>

<span data-ttu-id="0e949-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0e949-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e949-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0e949-108">Attributes</span></span>

<span data-ttu-id="0e949-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0e949-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e949-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0e949-110">Child elements</span></span>

|<span data-ttu-id="0e949-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0e949-111">**Element**</span></span>|<span data-ttu-id="0e949-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0e949-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e949-113">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e949-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="0e949-114">Представляет код ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0e949-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="0e949-115">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e949-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="0e949-116">Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0e949-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="0e949-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e949-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="0e949-118">Содержит параметры конфигурации для каждого запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e949-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0e949-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0e949-119">Parent elements</span></span>

|<span data-ttu-id="0e949-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0e949-120">**Element**</span></span>|<span data-ttu-id="0e949-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0e949-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e949-122">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e949-122">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="0e949-123">Определяет ответ на [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span><span class="sxs-lookup"><span data-stu-id="0e949-123">Defines a response to a [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span></span> <br/> |
|[<span data-ttu-id="0e949-124">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e949-124">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="0e949-125">Определяет ответ на [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="0e949-125">Defines a response to a [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="0e949-126">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e949-126">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="0e949-127">Определяет ответ на [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="0e949-127">Defines a response to a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e949-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0e949-128">Text value</span></span>

<span data-ttu-id="0e949-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="0e949-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e949-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0e949-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e949-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0e949-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0e949-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0e949-132">Schema Name</span></span>  <br/> |<span data-ttu-id="0e949-133">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="0e949-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0e949-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0e949-134">Validation File</span></span>  <br/> |<span data-ttu-id="0e949-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0e949-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0e949-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0e949-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e949-137">True</span><span class="sxs-lookup"><span data-stu-id="0e949-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e949-138">См. также</span><span class="sxs-lookup"><span data-stu-id="0e949-138">See also</span></span>



[<span data-ttu-id="0e949-139">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e949-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="0e949-140">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="0e949-140">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="0e949-141">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0e949-141">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

