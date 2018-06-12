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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835130"
---
# <a name="requestedconfiguration"></a><span data-ttu-id="b78e9-103">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="b78e9-103">RequestedConfiguration</span></span>

<span data-ttu-id="b78e9-104">Элемент **RequestedConfiguration** содержит требуемую службу конфигураций.</span><span class="sxs-lookup"><span data-stu-id="b78e9-104">The **RequestedConfiguration** element contains the requested service configurations.</span></span> 
  
```XML
<RequestedConfiguration>
   <ConfigurationName/>
</RequestedConfiguration>
```

 <span data-ttu-id="b78e9-105">**ArrayOfServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="b78e9-105">**ArrayOfServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b78e9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b78e9-106">Attributes and elements</span></span>

<span data-ttu-id="b78e9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b78e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b78e9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b78e9-108">Attributes</span></span>

<span data-ttu-id="b78e9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b78e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b78e9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b78e9-110">Child elements</span></span>

|<span data-ttu-id="b78e9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b78e9-111">**Element**</span></span>|<span data-ttu-id="b78e9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b78e9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b78e9-113">Имя_конфигурации</span><span class="sxs-lookup"><span data-stu-id="b78e9-113">ConfigurationName</span></span>](configurationname.md) <br/> |<span data-ttu-id="b78e9-114">Задает конфигураций запрошенную службу по имени.</span><span class="sxs-lookup"><span data-stu-id="b78e9-114">Specifies the requested service configurations by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b78e9-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b78e9-115">Parent elements</span></span>

|<span data-ttu-id="b78e9-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b78e9-116">**Element**</span></span>|<span data-ttu-id="b78e9-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b78e9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b78e9-118">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b78e9-118">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="b78e9-119">Определяет запрос GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b78e9-119">Defines a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b78e9-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b78e9-120">Text value</span></span>

<span data-ttu-id="b78e9-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="b78e9-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b78e9-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="b78e9-122">Remarks</span></span>

<span data-ttu-id="b78e9-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b78e9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b78e9-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b78e9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b78e9-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b78e9-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b78e9-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b78e9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="b78e9-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b78e9-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b78e9-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b78e9-128">Validation File</span></span>  <br/> |<span data-ttu-id="b78e9-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b78e9-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b78e9-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b78e9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="b78e9-131">False</span><span class="sxs-lookup"><span data-stu-id="b78e9-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b78e9-132">См. также</span><span class="sxs-lookup"><span data-stu-id="b78e9-132">See also</span></span>



- [<span data-ttu-id="b78e9-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b78e9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

