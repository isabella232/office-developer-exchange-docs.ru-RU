---
title: Версия (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 47c9216e-6bfe-48c8-a27a-26f70db8e8d5
description: Элемент Version представляет описание server версии продукта.
ms.openlocfilehash: b8284880646cb82e6af6715523467021f080b8e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840481"
---
# <a name="version-soap"></a><span data-ttu-id="865ca-103">Версия (SOAP)</span><span class="sxs-lookup"><span data-stu-id="865ca-103">Version (SOAP)</span></span>

<span data-ttu-id="865ca-104">Элемент **Version** представляет описание server версии продукта.</span><span class="sxs-lookup"><span data-stu-id="865ca-104">The **Version** element represents a description of the server product version.</span></span> 
  
```XML
<Version/>
```

 <span data-ttu-id="865ca-105">**string**</span><span class="sxs-lookup"><span data-stu-id="865ca-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="865ca-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="865ca-106">Attributes and elements</span></span>

<span data-ttu-id="865ca-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="865ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="865ca-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="865ca-108">Attributes</span></span>

<span data-ttu-id="865ca-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="865ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="865ca-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="865ca-110">Child elements</span></span>

<span data-ttu-id="865ca-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="865ca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="865ca-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="865ca-112">Parent elements</span></span>

|<span data-ttu-id="865ca-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="865ca-113">**Element**</span></span>|<span data-ttu-id="865ca-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="865ca-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="865ca-115">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="865ca-115">ServerVersionInfo (SOAP)</span></span>](serverversioninfo-soap.md) <br/> |<span data-ttu-id="865ca-116">Содержит версию сервера, на обработку запроса.</span><span class="sxs-lookup"><span data-stu-id="865ca-116">Contains the version of the server that processed the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="865ca-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="865ca-117">Text value</span></span>

<span data-ttu-id="865ca-118">Значение элемента **версии** приведено описание server версии продукта.</span><span class="sxs-lookup"><span data-stu-id="865ca-118">The value of the **Version** element is a description of the server product version.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="865ca-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="865ca-119">Remarks</span></span>

<span data-ttu-id="865ca-120">Элемент **Version** содержится в заголовке ответа SOAP.</span><span class="sxs-lookup"><span data-stu-id="865ca-120">The **Version** element is contained in the SOAP header of a response.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="865ca-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="865ca-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="865ca-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="865ca-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="865ca-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="865ca-123">Schema Name</span></span>  <br/> |<span data-ttu-id="865ca-124">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="865ca-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="865ca-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="865ca-125">Validation File</span></span>  <br/> |<span data-ttu-id="865ca-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="865ca-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="865ca-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="865ca-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="865ca-128">True</span><span class="sxs-lookup"><span data-stu-id="865ca-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="865ca-129">См. также</span><span class="sxs-lookup"><span data-stu-id="865ca-129">See also</span></span>



[<span data-ttu-id="865ca-130">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="865ca-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="865ca-131">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="865ca-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="865ca-132">Операция GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="865ca-132">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

