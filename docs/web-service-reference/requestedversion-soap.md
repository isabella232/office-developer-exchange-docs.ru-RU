---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: Элемент RequestedVersion указывает, что клиенту запрос для обработки в версию минимальные службы.
ms.openlocfilehash: 0d8682c33790d2d26001512ad9e2191ae52074d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835134"
---
# <a name="requestedversion-soap"></a><span data-ttu-id="48e20-103">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="48e20-103">RequestedVersion (SOAP)</span></span>

<span data-ttu-id="48e20-104">Элемент **RequestedVersion** указывает, что клиенту запрос для обработки в версию минимальные службы.</span><span class="sxs-lookup"><span data-stu-id="48e20-104">The **RequestedVersion** element specifies the minimum service version that the client wants the request to be processed on.</span></span> 
  
```XML
<RequestedVersion/>
```

 <span data-ttu-id="48e20-105">**ExchangeVersion**</span><span class="sxs-lookup"><span data-stu-id="48e20-105">**ExchangeVersion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="48e20-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="48e20-106">Attributes and elements</span></span>

<span data-ttu-id="48e20-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="48e20-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48e20-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="48e20-108">Attributes</span></span>

<span data-ttu-id="48e20-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="48e20-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48e20-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="48e20-110">Child elements</span></span>

<span data-ttu-id="48e20-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="48e20-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="48e20-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="48e20-112">Parent elements</span></span>

|<span data-ttu-id="48e20-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="48e20-113">**Element**</span></span>|<span data-ttu-id="48e20-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="48e20-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48e20-115">Запрос (SOAP)</span><span class="sxs-lookup"><span data-stu-id="48e20-115">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="48e20-116">Содержит параметры запрошенные конфигурации и к конечным пользователям.</span><span class="sxs-lookup"><span data-stu-id="48e20-116">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="48e20-117">Запрос (SOAP) (GetDomainSettings)</span><span class="sxs-lookup"><span data-stu-id="48e20-117">Request (GetDomainSettings) (SOAP)</span></span>](request-getdomainsettingssoap.md) <br/> |<span data-ttu-id="48e20-118">Представляет запрос на получение параметров домена.</span><span class="sxs-lookup"><span data-stu-id="48e20-118">Represents a request to get domain settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="48e20-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="48e20-119">Text value</span></span>

<span data-ttu-id="48e20-120">Текстовое значение для элемента **RequestedVersion** может быть Exchange2010, Exchange2010_SP1, Exchange2010_SP2 или Exchange2013.</span><span class="sxs-lookup"><span data-stu-id="48e20-120">The text value for the **RequestedVersion** element can be Exchange2010, Exchange2010_SP1, Exchange2010_SP2, or Exchange2013.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="48e20-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="48e20-121">Remarks</span></span>

<span data-ttu-id="48e20-122">Если этот элемент не указан, используется последнюю версию обновления.</span><span class="sxs-lookup"><span data-stu-id="48e20-122">If this element is not present, the latest service version is used.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48e20-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="48e20-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48e20-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="48e20-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="48e20-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="48e20-125">Schema Name</span></span>  <br/> |<span data-ttu-id="48e20-126">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="48e20-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="48e20-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="48e20-127">Validation File</span></span>  <br/> |<span data-ttu-id="48e20-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="48e20-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="48e20-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="48e20-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="48e20-130">False</span><span class="sxs-lookup"><span data-stu-id="48e20-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48e20-131">См. также</span><span class="sxs-lookup"><span data-stu-id="48e20-131">See also</span></span>



[<span data-ttu-id="48e20-132">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="48e20-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="48e20-133">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="48e20-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

