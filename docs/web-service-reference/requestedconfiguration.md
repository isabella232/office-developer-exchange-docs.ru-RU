---
title: рекуестедконфигуратион
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
description: Элемент Рекуестедконфигуратион содержит требуемые конфигурации службы.
ms.openlocfilehash: bbc503e6d6f7c56c785365924106bc2468965d0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457153"
---
# <a name="requestedconfiguration"></a><span data-ttu-id="5c13e-103">рекуестедконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5c13e-103">RequestedConfiguration</span></span>

<span data-ttu-id="5c13e-104">Элемент **рекуестедконфигуратион** содержит требуемые конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="5c13e-104">The **RequestedConfiguration** element contains the requested service configurations.</span></span> 
  
```XML
<RequestedConfiguration>
   <ConfigurationName/>
</RequestedConfiguration>
```

 <span data-ttu-id="5c13e-105">**аррайофсервицеконфигуратионтипе**</span><span class="sxs-lookup"><span data-stu-id="5c13e-105">**ArrayOfServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c13e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5c13e-106">Attributes and elements</span></span>

<span data-ttu-id="5c13e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5c13e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c13e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5c13e-108">Attributes</span></span>

<span data-ttu-id="5c13e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5c13e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c13e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5c13e-110">Child elements</span></span>

|<span data-ttu-id="5c13e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5c13e-111">**Element**</span></span>|<span data-ttu-id="5c13e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5c13e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c13e-113">Указав</span><span class="sxs-lookup"><span data-stu-id="5c13e-113">ConfigurationName</span></span>](configurationname.md) <br/> |<span data-ttu-id="5c13e-114">Задает имя запрашиваемой конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="5c13e-114">Specifies the requested service configurations by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c13e-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5c13e-115">Parent elements</span></span>

|<span data-ttu-id="5c13e-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5c13e-116">**Element**</span></span>|<span data-ttu-id="5c13e-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5c13e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c13e-118">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c13e-118">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="5c13e-119">Определяет запрос GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5c13e-119">Defines a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c13e-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5c13e-120">Text value</span></span>

<span data-ttu-id="5c13e-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="5c13e-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c13e-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="5c13e-122">Remarks</span></span>

<span data-ttu-id="5c13e-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c13e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c13e-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5c13e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c13e-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5c13e-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c13e-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5c13e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="5c13e-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5c13e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5c13e-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5c13e-128">Validation File</span></span>  <br/> |<span data-ttu-id="5c13e-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5c13e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c13e-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5c13e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c13e-131">False</span><span class="sxs-lookup"><span data-stu-id="5c13e-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c13e-132">См. также</span><span class="sxs-lookup"><span data-stu-id="5c13e-132">See also</span></span>



- [<span data-ttu-id="5c13e-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5c13e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

