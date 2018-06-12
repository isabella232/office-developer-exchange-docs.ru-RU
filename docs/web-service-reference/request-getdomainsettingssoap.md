---
title: Запрос (SOAP) (GetDomainSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: Элемент запрос содержит запрос возвращает настройки домена.
ms.openlocfilehash: 71a6072d476fd665dad8b0c0fe388a40db56e059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835135"
---
# <a name="request-getdomainsettings-soap"></a><span data-ttu-id="b72ef-103">Запрос (SOAP) (GetDomainSettings)</span><span class="sxs-lookup"><span data-stu-id="b72ef-103">Request (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="b72ef-104">Элемент **запрос** содержит запрос возвращает настройки домена.</span><span class="sxs-lookup"><span data-stu-id="b72ef-104">The **Request** element contains a request to return domain settings.</span></span> 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 <span data-ttu-id="b72ef-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="b72ef-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b72ef-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b72ef-106">Attributes and elements</span></span>

<span data-ttu-id="b72ef-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b72ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b72ef-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b72ef-108">Attributes</span></span>

<span data-ttu-id="b72ef-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b72ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b72ef-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b72ef-110">Child elements</span></span>

|<span data-ttu-id="b72ef-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b72ef-111">**Element**</span></span>|<span data-ttu-id="b72ef-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b72ef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b72ef-113">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b72ef-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="b72ef-114">Представляет доменов, конфигурации, для которого возвращаются в [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) или домены, которым организации федеративных в ходе [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="b72ef-114">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="b72ef-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b72ef-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="b72ef-116">Содержит имена параметров запрошенные конфигурации.</span><span class="sxs-lookup"><span data-stu-id="b72ef-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b72ef-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b72ef-117">Parent elements</span></span>

|<span data-ttu-id="b72ef-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b72ef-118">**Element**</span></span>|<span data-ttu-id="b72ef-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b72ef-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b72ef-120">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b72ef-120">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="b72ef-121">Представляет запрос [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="b72ef-121">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md)request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b72ef-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b72ef-122">Text value</span></span>

<span data-ttu-id="b72ef-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="b72ef-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b72ef-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b72ef-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b72ef-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b72ef-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b72ef-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b72ef-126">Schema Name</span></span>  <br/> |<span data-ttu-id="b72ef-127">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="b72ef-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b72ef-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b72ef-128">Validation File</span></span>  <br/> |<span data-ttu-id="b72ef-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b72ef-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b72ef-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b72ef-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="b72ef-131">True</span><span class="sxs-lookup"><span data-stu-id="b72ef-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b72ef-132">См. также</span><span class="sxs-lookup"><span data-stu-id="b72ef-132">See also</span></span>



[<span data-ttu-id="b72ef-133">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b72ef-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

