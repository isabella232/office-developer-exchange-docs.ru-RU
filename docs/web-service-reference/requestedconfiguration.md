---
title: RequestedConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestedConfiguration
api_type:
- schema
ms.assetid: 24921387-f676-49e6-8d7a-ef3115024866
description: Элемент RequestedConfiguration содержит требуемую службу конфигураций.
ms.openlocfilehash: 1edc6394360250c9a9810fe614c975cb48eba3f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835130"
---
# <a name="requestedconfiguration"></a><span data-ttu-id="f0615-103">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0615-103">RequestedConfiguration</span></span>

<span data-ttu-id="f0615-104">Элемент **RequestedConfiguration** содержит требуемую службу конфигураций.</span><span class="sxs-lookup"><span data-stu-id="f0615-104">The **RequestedConfiguration** element contains the requested service configurations.</span></span> 
  
```XML
<RequestedConfiguration>
   <ConfigurationName/>
</RequestedConfiguration>
```

 <span data-ttu-id="f0615-105">**ArrayOfServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="f0615-105">**ArrayOfServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0615-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f0615-106">Attributes and elements</span></span>

<span data-ttu-id="f0615-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f0615-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0615-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f0615-108">Attributes</span></span>

<span data-ttu-id="f0615-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f0615-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0615-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f0615-110">Child elements</span></span>

|<span data-ttu-id="f0615-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f0615-111">**Element**</span></span>|<span data-ttu-id="f0615-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0615-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0615-113">Имя_конфигурации</span><span class="sxs-lookup"><span data-stu-id="f0615-113">ConfigurationName</span></span>](configurationname.md) <br/> |<span data-ttu-id="f0615-114">Задает конфигураций запрошенную службу по имени.</span><span class="sxs-lookup"><span data-stu-id="f0615-114">Specifies the requested service configurations by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0615-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f0615-115">Parent elements</span></span>

|<span data-ttu-id="f0615-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f0615-116">**Element**</span></span>|<span data-ttu-id="f0615-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0615-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0615-118">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0615-118">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="f0615-119">Определяет запрос GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f0615-119">Defines a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f0615-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f0615-120">Text value</span></span>

<span data-ttu-id="f0615-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="f0615-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f0615-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="f0615-122">Remarks</span></span>

<span data-ttu-id="f0615-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0615-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0615-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f0615-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0615-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f0615-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0615-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f0615-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f0615-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f0615-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0615-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f0615-128">Validation File</span></span>  <br/> |<span data-ttu-id="f0615-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f0615-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0615-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f0615-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0615-131">False</span><span class="sxs-lookup"><span data-stu-id="f0615-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0615-132">См. также</span><span class="sxs-lookup"><span data-stu-id="f0615-132">See also</span></span>



- [<span data-ttu-id="f0615-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f0615-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

