---
title: ErrorCode (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: Элемент ErrorCode представляет код ошибки, возвращенный службой автообнаружения.
ms.openlocfilehash: d66167e51733ffcaa3d62a985d3e03e2ac80b715
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460094"
---
# <a name="errorcode-soap"></a><span data-ttu-id="93a54-103">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-103">ErrorCode (SOAP)</span></span>

<span data-ttu-id="93a54-104">Элемент **ErrorCode** представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="93a54-104">The **ErrorCode** element represents an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="93a54-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="93a54-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93a54-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="93a54-106">Attributes and elements</span></span>

<span data-ttu-id="93a54-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="93a54-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93a54-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="93a54-108">Attributes</span></span>

<span data-ttu-id="93a54-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="93a54-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93a54-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="93a54-110">Child elements</span></span>

<span data-ttu-id="93a54-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="93a54-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93a54-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="93a54-112">Parent elements</span></span>

|<span data-ttu-id="93a54-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="93a54-113">**Element**</span></span>|<span data-ttu-id="93a54-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93a54-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93a54-115">Аутодисковерреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="93a54-116">Представляет базовый тип для всех ответов, возвращаемых службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="93a54-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="93a54-117">Домаинреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="93a54-118">Содержит запрошенные параметры для указанного домена.</span><span class="sxs-lookup"><span data-stu-id="93a54-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="93a54-119">Жетдомаинсеттингсреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="93a54-120">Содержит ответ на вызов [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.</span><span class="sxs-lookup"><span data-stu-id="93a54-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="93a54-121">Жетфедератионинформатионреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="93a54-122">Содержит ответ на запрос [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="93a54-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="93a54-123">Отклик (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="93a54-124">Содержит ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="93a54-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md)request.</span></span>  <br/> |
|[<span data-ttu-id="93a54-125">Усерсеттинжеррор (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="93a54-126">Представляет ошибку, возвращаемую при получении параметра пользователя.</span><span class="sxs-lookup"><span data-stu-id="93a54-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="93a54-127">Усерреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="93a54-128">Представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="93a54-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93a54-129">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="93a54-129">Text value</span></span>

<span data-ttu-id="93a54-130">Текстовое значение представляет код ошибки для ответа на сообщение об ошибке автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="93a54-130">The text value represents the error code for an Autodiscover error response.</span></span> <span data-ttu-id="93a54-131">В следующей таблице приведены возможные текстовые значения для элемента **ErrorCode** .</span><span class="sxs-lookup"><span data-stu-id="93a54-131">The following table lists the possible text values for the **ErrorCode** element.</span></span> 
  
|<span data-ttu-id="93a54-132">**Текстовое значение кода ошибки**</span><span class="sxs-lookup"><span data-stu-id="93a54-132">**Error code text value**</span></span>|<span data-ttu-id="93a54-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="93a54-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93a54-134">NoError</span><span class="sxs-lookup"><span data-stu-id="93a54-134">NoError</span></span>  <br/> |<span data-ttu-id="93a54-135">Ошибка не обнаружена.</span><span class="sxs-lookup"><span data-stu-id="93a54-135">There was no error.</span></span>  <br/> |
|<span data-ttu-id="93a54-136">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="93a54-136">RedirectAddress</span></span>  <br/> |<span data-ttu-id="93a54-137">Вызывающий абонент должен следовать перенаправлению адресов электронной почты, которое было возвращено службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="93a54-137">The caller must follow the e-mail address redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="93a54-138">RedirectUrl адресом</span><span class="sxs-lookup"><span data-stu-id="93a54-138">RedirectUrl</span></span>  <br/> |<span data-ttu-id="93a54-139">Вызывающий абонент должен следовать перенаправлению URL-адреса, возвращенному службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="93a54-139">The caller must follow the URL redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="93a54-140">InvalidUser</span><span class="sxs-lookup"><span data-stu-id="93a54-140">InvalidUser</span></span>  <br/> |<span data-ttu-id="93a54-141">Недопустимый пользователь, переданный в запросе.</span><span class="sxs-lookup"><span data-stu-id="93a54-141">The user that was passed in the request is invalid.</span></span>  <br/> |
|<span data-ttu-id="93a54-142">InvalidRequest</span><span class="sxs-lookup"><span data-stu-id="93a54-142">InvalidRequest</span></span>  <br/> |<span data-ttu-id="93a54-143">Недопустимый запрос.</span><span class="sxs-lookup"><span data-stu-id="93a54-143">The request is invalid.</span></span>  <br/> |
|<span data-ttu-id="93a54-144">инвалидсеттинг</span><span class="sxs-lookup"><span data-stu-id="93a54-144">InvalidSetting</span></span>  <br/> |<span data-ttu-id="93a54-145">Указан недопустимый параметр.</span><span class="sxs-lookup"><span data-stu-id="93a54-145">A specified setting is invalid.</span></span>  <br/> |
|<span data-ttu-id="93a54-146">сеттингиснотаваилабле</span><span class="sxs-lookup"><span data-stu-id="93a54-146">SettingIsNotAvailable</span></span>  <br/> |<span data-ttu-id="93a54-147">Указанный параметр недоступен.</span><span class="sxs-lookup"><span data-stu-id="93a54-147">A specified setting is not available.</span></span>  <br/> |
|<span data-ttu-id="93a54-148">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="93a54-148">ServerBusy</span></span>  <br/> |<span data-ttu-id="93a54-149">Сервер перегружен и не может обработать запрос.</span><span class="sxs-lookup"><span data-stu-id="93a54-149">The server is too busy to process the request.</span></span>  <br/> |
|<span data-ttu-id="93a54-150">инвалиддомаин</span><span class="sxs-lookup"><span data-stu-id="93a54-150">InvalidDomain</span></span>  <br/> |<span data-ttu-id="93a54-151">Запрошенный домен не является допустимым.</span><span class="sxs-lookup"><span data-stu-id="93a54-151">The requested domain is not valid.</span></span>  <br/> |
|<span data-ttu-id="93a54-152">нотфедератед</span><span class="sxs-lookup"><span data-stu-id="93a54-152">NotFederated</span></span>  <br/> |<span data-ttu-id="93a54-153">Организация не является Федеративной.</span><span class="sxs-lookup"><span data-stu-id="93a54-153">The organization is not federated.</span></span>  <br/> |
|<span data-ttu-id="93a54-154">интерналсервереррор</span><span class="sxs-lookup"><span data-stu-id="93a54-154">InternalServerError</span></span>  <br/> |<span data-ttu-id="93a54-155">Внутренняя ошибка сервера.</span><span class="sxs-lookup"><span data-stu-id="93a54-155">There is an internal server error.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="93a54-156">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="93a54-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93a54-157">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="93a54-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="93a54-158">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="93a54-158">Schema Name</span></span>  <br/> |<span data-ttu-id="93a54-159">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="93a54-159">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="93a54-160">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="93a54-160">Validation File</span></span>  <br/> |<span data-ttu-id="93a54-161">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="93a54-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93a54-162">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="93a54-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="93a54-163">True</span><span class="sxs-lookup"><span data-stu-id="93a54-163">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93a54-164">См. также</span><span class="sxs-lookup"><span data-stu-id="93a54-164">See also</span></span>



[<span data-ttu-id="93a54-165">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-165">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="93a54-166">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-166">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="93a54-167">Операция Жетфедератионинформатион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93a54-167">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

