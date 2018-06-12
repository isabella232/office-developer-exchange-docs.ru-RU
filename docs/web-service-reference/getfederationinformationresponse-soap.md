---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: Элемент GetFederationInformationResponse содержит ответа GetFederationInformation операции (SOAP).
ms.openlocfilehash: 28b002b45968278ad4c7160b4eed29721422646d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762788"
---
# <a name="getfederationinformationresponse-soap"></a><span data-ttu-id="16420-103">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="16420-103">GetFederationInformationResponse (SOAP)</span></span>

<span data-ttu-id="16420-104">Элемент **GetFederationInformationResponse** содержит ответа [GetFederationInformation операции (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="16420-104">The **GetFederationInformationResponse** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span> 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 <span data-ttu-id="16420-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="16420-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16420-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="16420-106">Attributes and elements</span></span>

<span data-ttu-id="16420-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="16420-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16420-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="16420-108">Attributes</span></span>

<span data-ttu-id="16420-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="16420-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16420-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="16420-110">Child elements</span></span>

|<span data-ttu-id="16420-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="16420-111">**Element**</span></span>|<span data-ttu-id="16420-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="16420-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16420-113">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="16420-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="16420-114">Представляет код ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="16420-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="16420-115">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="16420-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="16420-116">Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="16420-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="16420-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="16420-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="16420-118">Определяет расположение приложения.</span><span class="sxs-lookup"><span data-stu-id="16420-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="16420-119">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="16420-119">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="16420-120">Представляет коллекцию маркеров безопасности, которые содержат идентификаторы службы маркеров безопасности и конечных точек.</span><span class="sxs-lookup"><span data-stu-id="16420-120">Represents a collection of security tokens, which contain security token service identifiers and endpoints.</span></span>  <br/> |
|[<span data-ttu-id="16420-121">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="16420-121">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="16420-122">Представляет доменов, конфигурации, для которого возвращаются в ходе операции [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** или домены, которым организации федеративных в ходе [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) Операция **GetFederationInformation** .</span><span class="sxs-lookup"><span data-stu-id="16420-122">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** operation or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="16420-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="16420-123">Parent elements</span></span>

<span data-ttu-id="16420-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="16420-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="16420-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="16420-125">Text value</span></span>

<span data-ttu-id="16420-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="16420-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16420-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="16420-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16420-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="16420-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="16420-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="16420-129">Schema Name</span></span>  <br/> |<span data-ttu-id="16420-130">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="16420-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="16420-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="16420-131">Validation File</span></span>  <br/> |<span data-ttu-id="16420-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="16420-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="16420-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="16420-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="16420-134">True</span><span class="sxs-lookup"><span data-stu-id="16420-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16420-135">См. также</span><span class="sxs-lookup"><span data-stu-id="16420-135">See also</span></span>



[<span data-ttu-id="16420-136">Операция GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="16420-136">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

