---
title: ErrorMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: Элемент ErrorMessage представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.
ms.openlocfilehash: 4ebaf91fe26083cf241826e1fc16ac184fddf57c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530644"
---
# <a name="errormessage-soap"></a><span data-ttu-id="05fb3-103">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-103">ErrorMessage (SOAP)</span></span>

<span data-ttu-id="05fb3-104">Элемент **ErrorMessage** представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="05fb3-104">The **ErrorMessage** element represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="05fb3-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="05fb3-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05fb3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="05fb3-106">Attributes and elements</span></span>

<span data-ttu-id="05fb3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="05fb3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05fb3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="05fb3-108">Attributes</span></span>

<span data-ttu-id="05fb3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="05fb3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05fb3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="05fb3-110">Child elements</span></span>

<span data-ttu-id="05fb3-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="05fb3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05fb3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="05fb3-112">Parent elements</span></span>

|<span data-ttu-id="05fb3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="05fb3-113">**Element**</span></span>|<span data-ttu-id="05fb3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="05fb3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05fb3-115">Аутодисковерреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="05fb3-116">Представляет базовый тип для всех ответов, возвращаемых службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="05fb3-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="05fb3-117">Домаинреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="05fb3-118">Содержит запрошенные параметры для указанного домена.</span><span class="sxs-lookup"><span data-stu-id="05fb3-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="05fb3-119">Жетдомаинсеттингсреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="05fb3-120">Содержит ответ на вызов [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.</span><span class="sxs-lookup"><span data-stu-id="05fb3-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="05fb3-121">Жетфедератионинформатионреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="05fb3-122">Содержит ответ на запрос [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="05fb3-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="05fb3-123">Отклик (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="05fb3-124">Содержит ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="05fb3-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="05fb3-125">Усерсеттинжеррор (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="05fb3-126">Представляет ошибку, возвращаемую при получении параметра пользователя.</span><span class="sxs-lookup"><span data-stu-id="05fb3-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="05fb3-127">Усерреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="05fb3-128">Представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="05fb3-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05fb3-129">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="05fb3-129">Text value</span></span>

<span data-ttu-id="05fb3-130">Текстовое значение представляет сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="05fb3-130">The text value represents the error message.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05fb3-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="05fb3-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05fb3-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="05fb3-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="05fb3-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="05fb3-133">Schema Name</span></span>  <br/> |<span data-ttu-id="05fb3-134">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="05fb3-134">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="05fb3-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="05fb3-135">Validation File</span></span>  <br/> |<span data-ttu-id="05fb3-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="05fb3-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="05fb3-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="05fb3-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="05fb3-138">True</span><span class="sxs-lookup"><span data-stu-id="05fb3-138">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05fb3-139">См. также</span><span class="sxs-lookup"><span data-stu-id="05fb3-139">See also</span></span>



[<span data-ttu-id="05fb3-140">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-140">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="05fb3-141">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-141">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="05fb3-142">Операция Жетфедератионинформатион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05fb3-142">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

