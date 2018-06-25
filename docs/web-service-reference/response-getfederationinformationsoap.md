---
title: Ответ (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: Элемент Response с информацией GetFederationInformation операции (SOAP) ответа.
ms.openlocfilehash: 946cba56d7503a0e20ec59640f4f1258c00a844e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835171"
---
# <a name="response-getfederationinformation-soap"></a><span data-ttu-id="0868f-103">Ответ (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0868f-103">Response (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="0868f-104">Элемент **ответа** содержит сведения ответа [GetFederationInformation операции (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="0868f-104">The **Response** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 <span data-ttu-id="0868f-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="0868f-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0868f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0868f-106">Attributes and elements</span></span>

<span data-ttu-id="0868f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0868f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0868f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0868f-108">Attributes</span></span>

<span data-ttu-id="0868f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0868f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0868f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0868f-110">Child elements</span></span>

|<span data-ttu-id="0868f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0868f-111">**Element**</span></span>|<span data-ttu-id="0868f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0868f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0868f-113">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0868f-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="0868f-114">Представляет код ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0868f-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="0868f-115">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0868f-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="0868f-116">Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0868f-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="0868f-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0868f-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="0868f-118">Определяет расположение приложения.</span><span class="sxs-lookup"><span data-stu-id="0868f-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="0868f-119">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0868f-119">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="0868f-120">Представляет коллекцию домена, конфигурации, для которого возвращаются в [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)или домены, которые организации федеративных в ходе [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="0868f-120">Represents the domain collection the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0868f-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0868f-121">Parent elements</span></span>

|<span data-ttu-id="0868f-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0868f-122">**Element**</span></span>|<span data-ttu-id="0868f-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0868f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0868f-124">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0868f-124">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="0868f-125">Определяет ответ на запрос [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="0868f-125">Defines a response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0868f-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0868f-126">Text value</span></span>

<span data-ttu-id="0868f-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="0868f-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0868f-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0868f-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0868f-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0868f-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0868f-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0868f-130">Schema Name</span></span>  <br/> |<span data-ttu-id="0868f-131">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="0868f-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0868f-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0868f-132">Validation File</span></span>  <br/> |<span data-ttu-id="0868f-133">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0868f-133">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0868f-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0868f-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="0868f-135">True</span><span class="sxs-lookup"><span data-stu-id="0868f-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0868f-136">См. также</span><span class="sxs-lookup"><span data-stu-id="0868f-136">See also</span></span>



[<span data-ttu-id="0868f-137">Операция GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0868f-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

