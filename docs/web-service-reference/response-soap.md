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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835179"
---
# <a name="response-soap"></a><span data-ttu-id="eb8b5-103">Ответ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb8b5-103">Response (SOAP)</span></span>

<span data-ttu-id="eb8b5-104">Элемент **ответа** содержит ответ на [операцию GetUserSettings (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)или запрос [GetFederationInformation операции (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="eb8b5-104">The **Response** element contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 <span data-ttu-id="eb8b5-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="eb8b5-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb8b5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="eb8b5-106">Attributes and elements</span></span>

<span data-ttu-id="eb8b5-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="eb8b5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb8b5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="eb8b5-108">Attributes</span></span>

<span data-ttu-id="eb8b5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="eb8b5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb8b5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="eb8b5-110">Child elements</span></span>

|<span data-ttu-id="eb8b5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eb8b5-111">**Element**</span></span>|<span data-ttu-id="eb8b5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eb8b5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb8b5-113">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb8b5-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="eb8b5-114">Представляет код ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="eb8b5-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="eb8b5-115">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb8b5-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="eb8b5-116">Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="eb8b5-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="eb8b5-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb8b5-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="eb8b5-118">Содержит параметры конфигурации для каждого запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb8b5-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb8b5-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="eb8b5-119">Parent elements</span></span>

|<span data-ttu-id="eb8b5-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eb8b5-120">**Element**</span></span>|<span data-ttu-id="eb8b5-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eb8b5-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb8b5-122">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb8b5-122">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="eb8b5-123">Определяет ответ на [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span><span class="sxs-lookup"><span data-stu-id="eb8b5-123">Defines a response to a [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span></span> <br/> |
|[<span data-ttu-id="eb8b5-124">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb8b5-124">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="eb8b5-125">Определяет ответ на [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="eb8b5-125">Defines a response to a [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="eb8b5-126">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb8b5-126">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="eb8b5-127">Определяет ответ на [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="eb8b5-127">Defines a response to a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eb8b5-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="eb8b5-128">Text value</span></span>

<span data-ttu-id="eb8b5-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="eb8b5-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb8b5-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="eb8b5-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb8b5-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="eb8b5-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="eb8b5-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="eb8b5-132">Schema Name</span></span>  <br/> |<span data-ttu-id="eb8b5-133">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="eb8b5-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="eb8b5-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="eb8b5-134">Validation File</span></span>  <br/> |<span data-ttu-id="eb8b5-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="eb8b5-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eb8b5-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="eb8b5-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb8b5-137">True</span><span class="sxs-lookup"><span data-stu-id="eb8b5-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb8b5-138">См. также</span><span class="sxs-lookup"><span data-stu-id="eb8b5-138">See also</span></span>



[<span data-ttu-id="eb8b5-139">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb8b5-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="eb8b5-140">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="eb8b5-140">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="eb8b5-141">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="eb8b5-141">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

