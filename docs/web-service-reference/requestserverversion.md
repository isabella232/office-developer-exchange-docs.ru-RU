---
title: рекуестсерверверсион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: Элемент Рекуестсерверверсион содержит сведения об управлении версиями, которые определяют версию схемы, предназначенную для запроса.
ms.openlocfilehash: c4ae59a03c812d21153e4338734185d933d914ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468322"
---
# <a name="requestserverversion"></a><span data-ttu-id="ac37b-103">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="ac37b-103">RequestServerVersion</span></span>

<span data-ttu-id="ac37b-104">Элемент **рекуестсерверверсион** содержит сведения об управлении версиями, которые определяют версию схемы, предназначенную для запроса.</span><span class="sxs-lookup"><span data-stu-id="ac37b-104">The **RequestServerVersion** element contains the versioning information that identifies the schema version to target for a request.</span></span> 
  
```XML
<RequestServerVersion Version=""/>
```

 <span data-ttu-id="ac37b-105">**Простом типе exchangeversiontype**</span><span class="sxs-lookup"><span data-stu-id="ac37b-105">**ExchangeVersionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac37b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ac37b-106">Attributes and elements</span></span>

<span data-ttu-id="ac37b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ac37b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac37b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ac37b-108">Attributes</span></span>

|<span data-ttu-id="ac37b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ac37b-109">**Attribute**</span></span>|<span data-ttu-id="ac37b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ac37b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ac37b-111">Версия</span><span class="sxs-lookup"><span data-stu-id="ac37b-111">Version</span></span>  <br/> |<span data-ttu-id="ac37b-112">Описывает версию, целевую для запроса.</span><span class="sxs-lookup"><span data-stu-id="ac37b-112">Describes the version to target for the request.</span></span> <span data-ttu-id="ac37b-113">Этот атрибут является обязательным, если версия целевого сервера является версией Exchange, начиная с Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="ac37b-113">This attribute is required when the target server version is a version of Exchange starting with Exchange Server 2010.</span></span>  <br/> |
   
#### <a name="version-attribute-values"></a><span data-ttu-id="ac37b-114">Значения атрибутов Version</span><span class="sxs-lookup"><span data-stu-id="ac37b-114">Version attribute values</span></span>

|<span data-ttu-id="ac37b-115">**Значение**</span><span class="sxs-lookup"><span data-stu-id="ac37b-115">**Value**</span></span>|<span data-ttu-id="ac37b-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ac37b-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ac37b-117">Exchange2007</span><span class="sxs-lookup"><span data-stu-id="ac37b-117">Exchange2007</span></span>  <br/> |<span data-ttu-id="ac37b-118">Нацеливание файлов схемы для первоначальной версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="ac37b-118">Target the schema files for the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="ac37b-119">Exchange2007_SP1</span><span class="sxs-lookup"><span data-stu-id="ac37b-119">Exchange2007_SP1</span></span>  <br/> |<span data-ttu-id="ac37b-120">Нацеливание файлов схемы для Exchange 2007 с пакетом обновления 1 (SP1), Exchange 2007 с пакетом обновления 2 (SP2) и Exchange 2007 с пакетом обновления 3 (SP3).</span><span class="sxs-lookup"><span data-stu-id="ac37b-120">Target the schema files for Exchange 2007 Service Pack 1 (SP1), Exchange 2007 Service Pack 2 (SP2), and Exchange 2007 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="ac37b-121">Exchange2010</span><span class="sxs-lookup"><span data-stu-id="ac37b-121">Exchange2010</span></span>  <br/> |<span data-ttu-id="ac37b-122">Нацеливание файлов схемы для Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="ac37b-122">Target the schema files for Exchange 2010.</span></span>  <br/> |
|<span data-ttu-id="ac37b-123">Exchange2010_SP1</span><span class="sxs-lookup"><span data-stu-id="ac37b-123">Exchange2010_SP1</span></span>  <br/> |<span data-ttu-id="ac37b-124">Нацеливание файлов схемы для Exchange 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ac37b-124">Target the schema files for Exchange 2010 Service Pack 1 (SP1).</span></span>  <br/> |
|<span data-ttu-id="ac37b-125">Exchange2010_SP2</span><span class="sxs-lookup"><span data-stu-id="ac37b-125">Exchange2010_SP2</span></span>  <br/> |<span data-ttu-id="ac37b-126">Нацеливание файлов схемы для Exchange 2010 с пакетом обновления 2 (SP2) и Exchange 2010 с пакетом обновления 3 (SP3).</span><span class="sxs-lookup"><span data-stu-id="ac37b-126">Target the schema files for Exchange 2010 Service Pack 2 (SP2) and Exchange 2010 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="ac37b-127">Exchange2013</span><span class="sxs-lookup"><span data-stu-id="ac37b-127">Exchange2013</span></span>  <br/> |<span data-ttu-id="ac37b-128">Нацеливание файлов схемы для Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ac37b-128">Target the schema files for Exchange 2013.</span></span>  <br/> |
|<span data-ttu-id="ac37b-129">Exchange2013_SP1</span><span class="sxs-lookup"><span data-stu-id="ac37b-129">Exchange2013_SP1</span></span>  <br/> |<span data-ttu-id="ac37b-130">Нацеливание файлов схемы для Exchange 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ac37b-130">Target the schema files for Exchange 2013 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ac37b-131">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ac37b-131">Child elements</span></span>

<span data-ttu-id="ac37b-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ac37b-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac37b-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ac37b-133">Parent elements</span></span>

<span data-ttu-id="ac37b-134">Элемент **рекуестсерверверсион** находится в заголовке SOAP.</span><span class="sxs-lookup"><span data-stu-id="ac37b-134">The **RequestServerVersion** element is located in the SOAP header.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ac37b-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="ac37b-135">Remarks</span></span>

<span data-ttu-id="ac37b-136">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac37b-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac37b-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ac37b-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac37b-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ac37b-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac37b-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ac37b-139">Schema Name</span></span>  <br/> |<span data-ttu-id="ac37b-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ac37b-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="ac37b-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ac37b-141">Validation File</span></span>  <br/> |<span data-ttu-id="ac37b-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ac37b-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac37b-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ac37b-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="ac37b-144">False</span><span class="sxs-lookup"><span data-stu-id="ac37b-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac37b-145">См. также</span><span class="sxs-lookup"><span data-stu-id="ac37b-145">See also</span></span>



- [<span data-ttu-id="ac37b-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ac37b-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ac37b-147">Запросы управления версиями</span><span class="sxs-lookup"><span data-stu-id="ac37b-147">Versioning Requests</span></span>](https://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

