---
title: DocumentSharingLocations (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 394f6015-721b-4800-9286-039d430f09b3
description: Элемент DocumentSharingLocations содержит список местоположения и сведения о метаданных для общего доступа к расположение документа.
ms.openlocfilehash: 72d1ae9f01ad45441b4e255f2fb6353be2dc8d28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762202"
---
# <a name="documentsharinglocations-soap"></a><span data-ttu-id="31d3a-103">DocumentSharingLocations (SOAP)</span><span class="sxs-lookup"><span data-stu-id="31d3a-103">DocumentSharingLocations (SOAP)</span></span>

<span data-ttu-id="31d3a-104">Элемент **DocumentSharingLocations** содержит список местоположения и сведения о метаданных для общего доступа к расположение документа.</span><span class="sxs-lookup"><span data-stu-id="31d3a-104">The **DocumentSharingLocations** element contains a list of location and metadata information for a document sharing location.</span></span> 
  
```XML
<DocumentSharingLocations>
   <DocumentSharingLocation />
</DocumentSharingLocations>
```

 <span data-ttu-id="31d3a-105">**DocumentSharingLocations**</span><span class="sxs-lookup"><span data-stu-id="31d3a-105">**DocumentSharingLocations**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31d3a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="31d3a-106">Attributes and elements</span></span>

<span data-ttu-id="31d3a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="31d3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31d3a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="31d3a-108">Attributes</span></span>

<span data-ttu-id="31d3a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="31d3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31d3a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="31d3a-110">Child elements</span></span>

|<span data-ttu-id="31d3a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="31d3a-111">**Element**</span></span>|<span data-ttu-id="31d3a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="31d3a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31d3a-113">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="31d3a-113">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="31d3a-114">Содержит расположение и метаданных для общего доступа к расположение документа.</span><span class="sxs-lookup"><span data-stu-id="31d3a-114">Contains the location and metadata for a document sharing location.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31d3a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="31d3a-115">Parent elements</span></span>

|<span data-ttu-id="31d3a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="31d3a-116">**Element**</span></span>|<span data-ttu-id="31d3a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="31d3a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31d3a-118">DocumentSharingLocationCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="31d3a-118">DocumentSharingLocationCollectionSetting (SOAP)</span></span>](documentsharinglocationcollectionsetting-soap.md) <br/> |<span data-ttu-id="31d3a-119">Представляет пользователя, то есть параметр коллекцию документации, совместное использование расположения и метаданных.</span><span class="sxs-lookup"><span data-stu-id="31d3a-119">Represents a user setting that is a collection of documentation sharing locations and metadata.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="31d3a-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="31d3a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31d3a-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="31d3a-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="31d3a-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="31d3a-122">Schema Name</span></span>  <br/> |<span data-ttu-id="31d3a-123">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="31d3a-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="31d3a-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="31d3a-124">Validation File</span></span>  <br/> |<span data-ttu-id="31d3a-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="31d3a-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="31d3a-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="31d3a-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="31d3a-127">True</span><span class="sxs-lookup"><span data-stu-id="31d3a-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31d3a-128">См. также</span><span class="sxs-lookup"><span data-stu-id="31d3a-128">See also</span></span>

- [<span data-ttu-id="31d3a-129">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="31d3a-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="31d3a-130">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="31d3a-130">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="31d3a-131">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="31d3a-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

