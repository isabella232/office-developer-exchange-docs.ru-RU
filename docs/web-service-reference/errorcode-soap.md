---
title: Код ошибки (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: Элемент ErrorCode представляет код ошибки, возвращаемые службой автообнаружения.
ms.openlocfilehash: 2dd91cec4645325c02bc8588af0ee0547909b945
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762378"
---
# <a name="errorcode-soap"></a><span data-ttu-id="b80be-103">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-103">ErrorCode (SOAP)</span></span>

<span data-ttu-id="b80be-104">Элемент **ErrorCode** представляет код ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="b80be-104">The **ErrorCode** element represents an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="b80be-105">**string**</span><span class="sxs-lookup"><span data-stu-id="b80be-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b80be-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b80be-106">Attributes and elements</span></span>

<span data-ttu-id="b80be-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b80be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b80be-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b80be-108">Attributes</span></span>

<span data-ttu-id="b80be-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b80be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b80be-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b80be-110">Child elements</span></span>

<span data-ttu-id="b80be-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b80be-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b80be-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b80be-112">Parent elements</span></span>

|<span data-ttu-id="b80be-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b80be-113">**Element**</span></span>|<span data-ttu-id="b80be-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b80be-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b80be-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="b80be-116">Представляет базовый тип для всех ответов, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="b80be-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="b80be-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="b80be-118">Содержит запрошенные параметры для конкретного домена.</span><span class="sxs-lookup"><span data-stu-id="b80be-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="b80be-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="b80be-120">Содержит ответ на звонок [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.</span><span class="sxs-lookup"><span data-stu-id="b80be-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="b80be-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="b80be-122">Содержит ответ на запрос [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="b80be-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="b80be-123">Ответ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="b80be-124">Содержит ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="b80be-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md)request.</span></span>  <br/> |
|[<span data-ttu-id="b80be-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="b80be-126">Представляет ошибку, который возвращается при получении параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="b80be-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="b80be-127">Ответ пользователя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="b80be-128">Представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b80be-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b80be-129">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b80be-129">Text value</span></span>

<span data-ttu-id="b80be-130">Текстовое значение представляет код ошибки для возврату ошибки службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="b80be-130">The text value represents the error code for an Autodiscover error response.</span></span> <span data-ttu-id="b80be-131">В следующей таблице перечислены возможные значения для элемента **код ошибки** .</span><span class="sxs-lookup"><span data-stu-id="b80be-131">The following table lists the possible text values for the **ErrorCode** element.</span></span> 
  
|<span data-ttu-id="b80be-132">**Текстовое значение кода ошибки**</span><span class="sxs-lookup"><span data-stu-id="b80be-132">**Error code text value**</span></span>|<span data-ttu-id="b80be-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b80be-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b80be-134">NoError</span><span class="sxs-lookup"><span data-stu-id="b80be-134">NoError</span></span>  <br/> |<span data-ttu-id="b80be-135">Ошибок не было.</span><span class="sxs-lookup"><span data-stu-id="b80be-135">There was no error.</span></span>  <br/> |
|<span data-ttu-id="b80be-136">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="b80be-136">RedirectAddress</span></span>  <br/> |<span data-ttu-id="b80be-137">Необходимо выполнить перенаправление адреса электронной почты, возвращаемые автообнаружения, вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="b80be-137">The caller must follow the e-mail address redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="b80be-138">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="b80be-138">RedirectUrl</span></span>  <br/> |<span data-ttu-id="b80be-139">Необходимо выполнить перенаправление URL-адреса, возвращаемые автообнаружения, вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="b80be-139">The caller must follow the URL redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="b80be-140">InvalidUser</span><span class="sxs-lookup"><span data-stu-id="b80be-140">InvalidUser</span></span>  <br/> |<span data-ttu-id="b80be-141">Пользователь, который был передан в запросе является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="b80be-141">The user that was passed in the request is invalid.</span></span>  <br/> |
|<span data-ttu-id="b80be-142">InvalidRequest</span><span class="sxs-lookup"><span data-stu-id="b80be-142">InvalidRequest</span></span>  <br/> |<span data-ttu-id="b80be-143">Недопустимый запрос.</span><span class="sxs-lookup"><span data-stu-id="b80be-143">The request is invalid.</span></span>  <br/> |
|<span data-ttu-id="b80be-144">InvalidSetting</span><span class="sxs-lookup"><span data-stu-id="b80be-144">InvalidSetting</span></span>  <br/> |<span data-ttu-id="b80be-145">Указанный параметр является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="b80be-145">A specified setting is invalid.</span></span>  <br/> |
|<span data-ttu-id="b80be-146">SettingIsNotAvailable</span><span class="sxs-lookup"><span data-stu-id="b80be-146">SettingIsNotAvailable</span></span>  <br/> |<span data-ttu-id="b80be-147">Указанный параметр недоступен.</span><span class="sxs-lookup"><span data-stu-id="b80be-147">A specified setting is not available.</span></span>  <br/> |
|<span data-ttu-id="b80be-148">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="b80be-148">ServerBusy</span></span>  <br/> |<span data-ttu-id="b80be-149">Сервер занят обработать запрос.</span><span class="sxs-lookup"><span data-stu-id="b80be-149">The server is too busy to process the request.</span></span>  <br/> |
|<span data-ttu-id="b80be-150">InvalidDomain</span><span class="sxs-lookup"><span data-stu-id="b80be-150">InvalidDomain</span></span>  <br/> |<span data-ttu-id="b80be-151">Запрошенный домен не является допустимым.</span><span class="sxs-lookup"><span data-stu-id="b80be-151">The requested domain is not valid.</span></span>  <br/> |
|<span data-ttu-id="b80be-152">NotFederated</span><span class="sxs-lookup"><span data-stu-id="b80be-152">NotFederated</span></span>  <br/> |<span data-ttu-id="b80be-153">Организации не федеративными.</span><span class="sxs-lookup"><span data-stu-id="b80be-153">The organization is not federated.</span></span>  <br/> |
|<span data-ttu-id="b80be-154">InternalServerError</span><span class="sxs-lookup"><span data-stu-id="b80be-154">InternalServerError</span></span>  <br/> |<span data-ttu-id="b80be-155">Существует Внутренняя ошибка сервера.</span><span class="sxs-lookup"><span data-stu-id="b80be-155">There is an internal server error.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="b80be-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b80be-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b80be-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b80be-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b80be-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b80be-158">Schema Name</span></span>  <br/> |<span data-ttu-id="b80be-159">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="b80be-159">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b80be-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b80be-160">Validation File</span></span>  <br/> |<span data-ttu-id="b80be-161">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b80be-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b80be-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b80be-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="b80be-163">True</span><span class="sxs-lookup"><span data-stu-id="b80be-163">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b80be-164">См. также</span><span class="sxs-lookup"><span data-stu-id="b80be-164">See also</span></span>



[<span data-ttu-id="b80be-165">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-165">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="b80be-166">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-166">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="b80be-167">Операция GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b80be-167">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

