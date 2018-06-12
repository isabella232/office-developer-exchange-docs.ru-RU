---
title: DomainResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d9c7fd91-22cd-4c72-a841-25cb9d415e0c
description: Элемент DomainResponses содержит массив ответ для каждого домена запрошенные параметры.
ms.openlocfilehash: 77a3efc1605337ab436f6aea2b61a67f22e4f8ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762213"
---
# <a name="domainresponses-soap"></a><span data-ttu-id="fd96b-103">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fd96b-103">DomainResponses (SOAP)</span></span>

<span data-ttu-id="fd96b-104">Элемент **DomainResponses** содержит массив ответ для каждого домена запрошенные параметры.</span><span class="sxs-lookup"><span data-stu-id="fd96b-104">The **DomainResponses** element contains an array of responses for each requested domain's settings.</span></span> 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 <span data-ttu-id="fd96b-105">**ArrayOfDomainResponse**</span><span class="sxs-lookup"><span data-stu-id="fd96b-105">**ArrayOfDomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd96b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fd96b-106">Attributes and elements</span></span>

<span data-ttu-id="fd96b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fd96b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd96b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fd96b-108">Attributes</span></span>

<span data-ttu-id="fd96b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fd96b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd96b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fd96b-110">Child elements</span></span>

|<span data-ttu-id="fd96b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fd96b-111">**Element**</span></span>|<span data-ttu-id="fd96b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd96b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd96b-113">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fd96b-113">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="fd96b-114">Содержит запрошенные параметры для конкретного домена.</span><span class="sxs-lookup"><span data-stu-id="fd96b-114">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd96b-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fd96b-115">Parent elements</span></span>

|<span data-ttu-id="fd96b-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fd96b-116">**Element**</span></span>|<span data-ttu-id="fd96b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fd96b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd96b-118">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fd96b-118">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="fd96b-119">Представляет ответ на запрос [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) для домена и возвращает параметры домена.</span><span class="sxs-lookup"><span data-stu-id="fd96b-119">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request for a domain, and returns the domain settings.</span></span>  <br/> |
|[<span data-ttu-id="fd96b-120">Ответ (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fd96b-120">Response (GetDomainSettings) (SOAP)</span></span>](response-getdomainsettingssoap.md) <br/> |<span data-ttu-id="fd96b-121">Представляет ответ на звонок [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.</span><span class="sxs-lookup"><span data-stu-id="fd96b-121">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fd96b-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fd96b-122">Text value</span></span>

<span data-ttu-id="fd96b-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="fd96b-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd96b-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fd96b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd96b-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fd96b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fd96b-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fd96b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="fd96b-127">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="fd96b-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fd96b-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fd96b-128">Validation File</span></span>  <br/> |<span data-ttu-id="fd96b-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fd96b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fd96b-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fd96b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd96b-131">True</span><span class="sxs-lookup"><span data-stu-id="fd96b-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd96b-132">См. также</span><span class="sxs-lookup"><span data-stu-id="fd96b-132">See also</span></span>

- [<span data-ttu-id="fd96b-133">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fd96b-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

