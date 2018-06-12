---
title: Сообщение об ошибке (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: Сообщение об ошибке элемент представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.
ms.openlocfilehash: 888eedc9c7cbbd1aad5cba21e76d999699c7ed02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762388"
---
# <a name="errormessage-soap"></a><span data-ttu-id="adce8-103">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-103">ErrorMessage (SOAP)</span></span>

<span data-ttu-id="adce8-104">**Сообщение об ошибке** элемент представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="adce8-104">The **ErrorMessage** element represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="adce8-105">**string**</span><span class="sxs-lookup"><span data-stu-id="adce8-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="adce8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="adce8-106">Attributes and elements</span></span>

<span data-ttu-id="adce8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="adce8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="adce8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="adce8-108">Attributes</span></span>

<span data-ttu-id="adce8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="adce8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="adce8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="adce8-110">Child elements</span></span>

<span data-ttu-id="adce8-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="adce8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="adce8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="adce8-112">Parent elements</span></span>

|<span data-ttu-id="adce8-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="adce8-113">**Element**</span></span>|<span data-ttu-id="adce8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="adce8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="adce8-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="adce8-116">Представляет базовый тип для всех ответов, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="adce8-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="adce8-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="adce8-118">Содержит запрошенные параметры для конкретного домена.</span><span class="sxs-lookup"><span data-stu-id="adce8-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="adce8-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="adce8-120">Содержит ответ на звонок [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.</span><span class="sxs-lookup"><span data-stu-id="adce8-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="adce8-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="adce8-122">Содержит ответ на запрос [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="adce8-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="adce8-123">Ответ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="adce8-124">Содержит ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="adce8-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="adce8-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="adce8-126">Представляет ошибку, который возвращается при получении параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="adce8-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="adce8-127">Ответ пользователя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="adce8-128">Представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="adce8-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="adce8-129">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="adce8-129">Text value</span></span>

<span data-ttu-id="adce8-130">Текстовое значение представляет сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="adce8-130">The text value represents the error message.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="adce8-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="adce8-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="adce8-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="adce8-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="adce8-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="adce8-133">Schema Name</span></span>  <br/> |<span data-ttu-id="adce8-134">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="adce8-134">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="adce8-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="adce8-135">Validation File</span></span>  <br/> |<span data-ttu-id="adce8-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="adce8-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="adce8-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="adce8-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="adce8-138">True</span><span class="sxs-lookup"><span data-stu-id="adce8-138">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="adce8-139">См. также</span><span class="sxs-lookup"><span data-stu-id="adce8-139">See also</span></span>



[<span data-ttu-id="adce8-140">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-140">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="adce8-141">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-141">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="adce8-142">Операция GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="adce8-142">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

