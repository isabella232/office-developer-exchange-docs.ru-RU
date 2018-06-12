---
title: RequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestType
api_type:
- schema
ms.assetid: 4e657e57-528f-4250-a99c-f9850bbbcec5
description: Элемент RequestType определяет, является ли запрос на прокси-сервер между узлами или запросов между лесами.
ms.openlocfilehash: 96a4d57432b15aa54fff2618df458fc75cb227f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835139"
---
# <a name="requesttype"></a><span data-ttu-id="79d5d-103">RequestType</span><span class="sxs-lookup"><span data-stu-id="79d5d-103">RequestType</span></span>

<span data-ttu-id="79d5d-104">Элемент **RequestType** определяет, является ли запрос на прокси-сервер между узлами или запросов между лесами.</span><span class="sxs-lookup"><span data-stu-id="79d5d-104">The **RequestType** element identifies whether a proxy request is a cross-site or a cross-forest request.</span></span> 
  
```xml
<RequestType>CrossSite or CrossForest</RequestType>
```

 <span data-ttu-id="79d5d-105">**AvailabilityProxyRequestType**</span><span class="sxs-lookup"><span data-stu-id="79d5d-105">**AvailabilityProxyRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79d5d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="79d5d-106">Attributes and elements</span></span>

<span data-ttu-id="79d5d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="79d5d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79d5d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="79d5d-108">Attributes</span></span>

<span data-ttu-id="79d5d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="79d5d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79d5d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="79d5d-110">Child elements</span></span>

<span data-ttu-id="79d5d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="79d5d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79d5d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="79d5d-112">Parent elements</span></span>

<span data-ttu-id="79d5d-113">Этот элемент не имеет родительского в схеме.</span><span class="sxs-lookup"><span data-stu-id="79d5d-113">This element does not have a parent in the schema.</span></span> <span data-ttu-id="79d5d-114">Данный элемент используется в заголовке SOAP.</span><span class="sxs-lookup"><span data-stu-id="79d5d-114">This element is used in the SOAP header.</span></span> <span data-ttu-id="79d5d-115">Дополнительные сведения об использовании этого элемента содержатся в файле WSDL.</span><span class="sxs-lookup"><span data-stu-id="79d5d-115">For more information about how this element is used, see the WSDL file.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="79d5d-116">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="79d5d-116">Text value</span></span>

<span data-ttu-id="79d5d-117">Для этого элемента требуется указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="79d5d-117">A text value is required for this element.</span></span> <span data-ttu-id="79d5d-118">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="79d5d-118">The following are the possible values:</span></span>
  
- <span data-ttu-id="79d5d-119">CrossSite</span><span class="sxs-lookup"><span data-stu-id="79d5d-119">CrossSite</span></span>
    
- <span data-ttu-id="79d5d-120">CrossForest</span><span class="sxs-lookup"><span data-stu-id="79d5d-120">CrossForest</span></span>
    
## <a name="element-information"></a><span data-ttu-id="79d5d-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="79d5d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79d5d-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="79d5d-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79d5d-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="79d5d-123">Schema name</span></span>  <br/> |<span data-ttu-id="79d5d-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="79d5d-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="79d5d-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="79d5d-125">Validation file</span></span>  <br/> |<span data-ttu-id="79d5d-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="79d5d-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79d5d-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="79d5d-127">Can be empty</span></span>  <br/> |<span data-ttu-id="79d5d-128">False</span><span class="sxs-lookup"><span data-stu-id="79d5d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79d5d-129">См. также</span><span class="sxs-lookup"><span data-stu-id="79d5d-129">See also</span></span>



- [<span data-ttu-id="79d5d-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="79d5d-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

