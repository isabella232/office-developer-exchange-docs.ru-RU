---
title: Жетфедератионинформатионреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: Элемент Жетфедератионинформатионреспонсе содержит ответ операции Жетфедератионинформатион (SOAP).
ms.openlocfilehash: c9e65a2b1759946b8493b3c730f08df6fe353fd8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460045"
---
# <a name="getfederationinformationresponse-soap"></a><span data-ttu-id="24734-103">Жетфедератионинформатионреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24734-103">GetFederationInformationResponse (SOAP)</span></span>

<span data-ttu-id="24734-104">Элемент **жетфедератионинформатионреспонсе** содержит ответ [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="24734-104">The **GetFederationInformationResponse** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span> 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 <span data-ttu-id="24734-105">**жетфедератионинформатионреспонсе**</span><span class="sxs-lookup"><span data-stu-id="24734-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24734-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="24734-106">Attributes and elements</span></span>

<span data-ttu-id="24734-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="24734-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24734-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="24734-108">Attributes</span></span>

<span data-ttu-id="24734-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="24734-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24734-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="24734-110">Child elements</span></span>

|<span data-ttu-id="24734-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="24734-111">**Element**</span></span>|<span data-ttu-id="24734-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24734-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24734-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24734-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="24734-114">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="24734-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="24734-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24734-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="24734-116">Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="24734-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="24734-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24734-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="24734-118">Определяет расположение приложения.</span><span class="sxs-lookup"><span data-stu-id="24734-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="24734-119">Токениссуерс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24734-119">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="24734-120">Представляет коллекцию маркеров безопасности, которая содержит идентификаторы и конечные точки службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="24734-120">Represents a collection of security tokens, which contain security token service identifiers and endpoints.</span></span>  <br/> |
|[<span data-ttu-id="24734-121">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24734-121">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="24734-122">Представляет домены, для которых в операции [жетфедератионинформатион (SOAP) операции (SOAP)](getfederationinformation-operation-soap.md) **жетфедератионинформатион** операции, которые возвращаются в ходе операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) **жетдомаинсеттингс** или домены, в которых участвует Организация.</span><span class="sxs-lookup"><span data-stu-id="24734-122">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** operation or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24734-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="24734-123">Parent elements</span></span>

<span data-ttu-id="24734-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="24734-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="24734-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="24734-125">Text value</span></span>

<span data-ttu-id="24734-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="24734-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24734-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="24734-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24734-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="24734-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="24734-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="24734-129">Schema Name</span></span>  <br/> |<span data-ttu-id="24734-130">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="24734-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="24734-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="24734-131">Validation File</span></span>  <br/> |<span data-ttu-id="24734-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="24734-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="24734-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="24734-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="24734-134">True</span><span class="sxs-lookup"><span data-stu-id="24734-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24734-135">См. также</span><span class="sxs-lookup"><span data-stu-id="24734-135">See also</span></span>



[<span data-ttu-id="24734-136">Операция Жетфедератионинформатион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24734-136">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

