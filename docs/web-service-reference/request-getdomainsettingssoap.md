---
title: Request (Жетдомаинсеттингс) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: Элемент Request содержит запрос на возврат параметров домена.
ms.openlocfilehash: 71a6072d476fd665dad8b0c0fe388a40db56e059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835135"
---
# <a name="request-getdomainsettings-soap"></a><span data-ttu-id="cf723-103">Request (Жетдомаинсеттингс) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf723-103">Request (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="cf723-104">Элемент **request** содержит запрос на возврат параметров домена.</span><span class="sxs-lookup"><span data-stu-id="cf723-104">The **Request** element contains a request to return domain settings.</span></span> 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 <span data-ttu-id="cf723-105">**жетдомаинсеттингсрекуест**</span><span class="sxs-lookup"><span data-stu-id="cf723-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf723-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cf723-106">Attributes and elements</span></span>

<span data-ttu-id="cf723-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cf723-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf723-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cf723-108">Attributes</span></span>

<span data-ttu-id="cf723-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf723-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf723-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cf723-110">Child elements</span></span>

|<span data-ttu-id="cf723-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf723-111">**Element**</span></span>|<span data-ttu-id="cf723-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf723-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf723-113">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf723-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="cf723-114">Представляет домены конфигурации, для которых в операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) или доменах, в которых Организация имеет Федеративные результаты, в [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="cf723-114">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="cf723-115">Рекуестедсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf723-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="cf723-116">Содержит имена запрошенных параметров конфигурации.</span><span class="sxs-lookup"><span data-stu-id="cf723-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf723-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cf723-117">Parent elements</span></span>

|<span data-ttu-id="cf723-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf723-118">**Element**</span></span>|<span data-ttu-id="cf723-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf723-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf723-120">Жетдомаинсеттингсрекуестмессаже (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf723-120">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="cf723-121">Представляет запрос [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="cf723-121">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md)request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf723-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cf723-122">Text value</span></span>

<span data-ttu-id="cf723-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf723-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf723-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cf723-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf723-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cf723-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="cf723-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cf723-126">Schema Name</span></span>  <br/> |<span data-ttu-id="cf723-127">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="cf723-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="cf723-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cf723-128">Validation File</span></span>  <br/> |<span data-ttu-id="cf723-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cf723-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cf723-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cf723-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf723-131">True</span><span class="sxs-lookup"><span data-stu-id="cf723-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf723-132">См. также</span><span class="sxs-lookup"><span data-stu-id="cf723-132">See also</span></span>



[<span data-ttu-id="cf723-133">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf723-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

