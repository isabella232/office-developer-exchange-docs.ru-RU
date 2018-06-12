---
title: Конечная точка (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: Элемент конечной точки Указывает конечную точку службы маркеров безопасности.
ms.openlocfilehash: 85e1ad785b35649238ac3944f51472addf617c20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762353"
---
# <a name="endpoint-soap"></a><span data-ttu-id="88db2-103">Конечная точка (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88db2-103">Endpoint (SOAP)</span></span>

<span data-ttu-id="88db2-104">Элемент **конечной точки** Указывает конечную точку службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="88db2-104">The **Endpoint** element specifies the security token service endpoint.</span></span> 
  
```XML
<Endpoint/>
```

 <span data-ttu-id="88db2-105">**xs: anyURI**</span><span class="sxs-lookup"><span data-stu-id="88db2-105">**xs:anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88db2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="88db2-106">Attributes and elements</span></span>

<span data-ttu-id="88db2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="88db2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88db2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="88db2-108">Attributes</span></span>

<span data-ttu-id="88db2-109">Нет</span><span class="sxs-lookup"><span data-stu-id="88db2-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88db2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="88db2-110">Child elements</span></span>

<span data-ttu-id="88db2-111">Нет</span><span class="sxs-lookup"><span data-stu-id="88db2-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="88db2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="88db2-112">Parent elements</span></span>

|<span data-ttu-id="88db2-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88db2-113">**Element**</span></span>|<span data-ttu-id="88db2-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88db2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88db2-115">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88db2-115">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="88db2-116">Указывает URI и конечной точки для службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="88db2-116">Specifies the URI and Endpoint for the security token service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88db2-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="88db2-117">Text value</span></span>

<span data-ttu-id="88db2-118">Текстовое значение представляет конечной точки для службы маркеров web безопасности.</span><span class="sxs-lookup"><span data-stu-id="88db2-118">The text value represents the endpoint for the security token web service.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="88db2-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="88db2-119">Remarks</span></span>

<span data-ttu-id="88db2-120">Конечная точка используется для обмена данными с помощью маркеров веб-службы безопасности.</span><span class="sxs-lookup"><span data-stu-id="88db2-120">The endpoint is used for communicating with the security token web service.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88db2-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="88db2-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88db2-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="88db2-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="88db2-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="88db2-123">Schema Name</span></span>  <br/> |<span data-ttu-id="88db2-124">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="88db2-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="88db2-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="88db2-125">Validation File</span></span>  <br/> |<span data-ttu-id="88db2-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="88db2-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="88db2-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="88db2-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="88db2-128">True</span><span class="sxs-lookup"><span data-stu-id="88db2-128">True</span></span>  <br/> |
   
