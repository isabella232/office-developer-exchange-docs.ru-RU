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
ms.openlocfilehash: 0092d90a5fc479363f6d774b793c7148ad29f21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835143"
---
# <a name="requestserverversion"></a><span data-ttu-id="73990-103">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="73990-103">RequestServerVersion</span></span>

<span data-ttu-id="73990-104">Элемент **рекуестсерверверсион** содержит сведения об управлении версиями, которые определяют версию схемы, предназначенную для запроса.</span><span class="sxs-lookup"><span data-stu-id="73990-104">The **RequestServerVersion** element contains the versioning information that identifies the schema version to target for a request.</span></span> 
  
```XML
<RequestServerVersion Version=""/>
```

 <span data-ttu-id="73990-105">**Простом типе exchangeversiontype**</span><span class="sxs-lookup"><span data-stu-id="73990-105">**ExchangeVersionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73990-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="73990-106">Attributes and elements</span></span>

<span data-ttu-id="73990-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="73990-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73990-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="73990-108">Attributes</span></span>

|<span data-ttu-id="73990-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="73990-109">**Attribute**</span></span>|<span data-ttu-id="73990-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="73990-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="73990-111">Версия</span><span class="sxs-lookup"><span data-stu-id="73990-111">Version</span></span>  <br/> |<span data-ttu-id="73990-112">Описывает версию, целевую для запроса.</span><span class="sxs-lookup"><span data-stu-id="73990-112">Describes the version to target for the request.</span></span> <span data-ttu-id="73990-113">Этот атрибут является обязательным, если версия целевого сервера является версией Exchange, начиная с Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="73990-113">This attribute is required when the target server version is a version of Exchange starting with Exchange Server 2010.</span></span>  <br/> |
   
#### <a name="version-attribute-values"></a><span data-ttu-id="73990-114">Значения атрибутов Version</span><span class="sxs-lookup"><span data-stu-id="73990-114">Version attribute values</span></span>

|<span data-ttu-id="73990-115">**Значение**</span><span class="sxs-lookup"><span data-stu-id="73990-115">**Value**</span></span>|<span data-ttu-id="73990-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="73990-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="73990-117">Exchange2007</span><span class="sxs-lookup"><span data-stu-id="73990-117">Exchange2007</span></span>  <br/> |<span data-ttu-id="73990-118">Нацеливание файлов схемы для первоначальной версии Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="73990-118">Target the schema files for the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="73990-119">Exchange2007_SP1</span><span class="sxs-lookup"><span data-stu-id="73990-119">Exchange2007_SP1</span></span>  <br/> |<span data-ttu-id="73990-120">Нацеливание файлов схемы для Exchange 2007 с пакетом обновления 1 (SP1), Exchange 2007 с пакетом обновления 2 (SP2) и Exchange 2007 с пакетом обновления 3 (SP3).</span><span class="sxs-lookup"><span data-stu-id="73990-120">Target the schema files for Exchange 2007 Service Pack 1 (SP1), Exchange 2007 Service Pack 2 (SP2), and Exchange 2007 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="73990-121">Exchange2010</span><span class="sxs-lookup"><span data-stu-id="73990-121">Exchange2010</span></span>  <br/> |<span data-ttu-id="73990-122">Нацеливание файлов схемы для Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="73990-122">Target the schema files for Exchange 2010.</span></span>  <br/> |
|<span data-ttu-id="73990-123">Exchange2010_SP1</span><span class="sxs-lookup"><span data-stu-id="73990-123">Exchange2010_SP1</span></span>  <br/> |<span data-ttu-id="73990-124">Нацеливание файлов схемы для Exchange 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="73990-124">Target the schema files for Exchange 2010 Service Pack 1 (SP1).</span></span>  <br/> |
|<span data-ttu-id="73990-125">Exchange2010_SP2</span><span class="sxs-lookup"><span data-stu-id="73990-125">Exchange2010_SP2</span></span>  <br/> |<span data-ttu-id="73990-126">Нацеливание файлов схемы для Exchange 2010 с пакетом обновления 2 (SP2) и Exchange 2010 с пакетом обновления 3 (SP3).</span><span class="sxs-lookup"><span data-stu-id="73990-126">Target the schema files for Exchange 2010 Service Pack 2 (SP2) and Exchange 2010 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="73990-127">Exchange2013</span><span class="sxs-lookup"><span data-stu-id="73990-127">Exchange2013</span></span>  <br/> |<span data-ttu-id="73990-128">Нацеливание файлов схемы для Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="73990-128">Target the schema files for Exchange 2013.</span></span>  <br/> |
|<span data-ttu-id="73990-129">Exchange2013_SP1</span><span class="sxs-lookup"><span data-stu-id="73990-129">Exchange2013_SP1</span></span>  <br/> |<span data-ttu-id="73990-130">Нацеливание файлов схемы для Exchange 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="73990-130">Target the schema files for Exchange 2013 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="73990-131">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="73990-131">Child elements</span></span>

<span data-ttu-id="73990-132">Нет.</span><span class="sxs-lookup"><span data-stu-id="73990-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73990-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="73990-133">Parent elements</span></span>

<span data-ttu-id="73990-134">Элемент **рекуестсерверверсион** находится в заголовке SOAP.</span><span class="sxs-lookup"><span data-stu-id="73990-134">The **RequestServerVersion** element is located in the SOAP header.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="73990-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="73990-135">Remarks</span></span>

<span data-ttu-id="73990-136">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="73990-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73990-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="73990-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73990-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="73990-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="73990-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="73990-139">Schema Name</span></span>  <br/> |<span data-ttu-id="73990-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="73990-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="73990-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="73990-141">Validation File</span></span>  <br/> |<span data-ttu-id="73990-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="73990-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="73990-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="73990-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="73990-144">False</span><span class="sxs-lookup"><span data-stu-id="73990-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73990-145">См. также</span><span class="sxs-lookup"><span data-stu-id="73990-145">See also</span></span>



- [<span data-ttu-id="73990-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="73990-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="73990-147">Запросы управления версиями</span><span class="sxs-lookup"><span data-stu-id="73990-147">Versioning Requests</span></span>](http://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

