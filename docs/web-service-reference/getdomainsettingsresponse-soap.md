---
title: GetDomainSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43ebd17b-3a70-4878-9254-97a4c2c87b77
description: Элемент GetDomainSettingsResponse представляет ответ на операцию GetDomainSettings (SOAP), которая возвращает настройки домена.
ms.openlocfilehash: c4984c2c6c532fcbd45c1a75733e578f6d9491fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762758"
---
# <a name="getdomainsettingsresponse-soap"></a><span data-ttu-id="444ed-103">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="444ed-103">GetDomainSettingsResponse (SOAP)</span></span>

<span data-ttu-id="444ed-104">Элемент **GetDomainSettingsResponse** представляет ответ на [операцию GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), который возвращает настройки домена.</span><span class="sxs-lookup"><span data-stu-id="444ed-104">The **GetDomainSettingsResponse** element represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), which returns the domain settings.</span></span>
  
```XML
<GetDomainSettingsResponse>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</GetDomainSettingsResponse>
```

 <span data-ttu-id="444ed-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="444ed-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="444ed-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="444ed-106">Attributes and elements</span></span>

<span data-ttu-id="444ed-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="444ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="444ed-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="444ed-108">Attributes</span></span>

<span data-ttu-id="444ed-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="444ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="444ed-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="444ed-110">Child elements</span></span>

|<span data-ttu-id="444ed-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="444ed-111">**Element**</span></span>|<span data-ttu-id="444ed-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="444ed-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="444ed-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="444ed-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="444ed-114">Содержит массив ответ для каждого домена запрошенные параметры.</span><span class="sxs-lookup"><span data-stu-id="444ed-114">Contains an array of responses for each requested domain's settings.</span></span>  <br/> |
|[<span data-ttu-id="444ed-115">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="444ed-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="444ed-116">Представляет код ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="444ed-116">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="444ed-117">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="444ed-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="444ed-118">Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="444ed-118">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="444ed-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="444ed-119">Parent elements</span></span>

<span data-ttu-id="444ed-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="444ed-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="444ed-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="444ed-121">Text value</span></span>

<span data-ttu-id="444ed-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="444ed-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="444ed-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="444ed-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="444ed-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="444ed-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="444ed-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="444ed-125">Schema Name</span></span>  <br/> |<span data-ttu-id="444ed-126">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="444ed-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="444ed-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="444ed-127">Validation File</span></span>  <br/> |<span data-ttu-id="444ed-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="444ed-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="444ed-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="444ed-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="444ed-130">True</span><span class="sxs-lookup"><span data-stu-id="444ed-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="444ed-131">См. также</span><span class="sxs-lookup"><span data-stu-id="444ed-131">See also</span></span>



[<span data-ttu-id="444ed-132">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="444ed-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

