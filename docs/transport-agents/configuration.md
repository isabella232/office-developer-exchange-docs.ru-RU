---
title: конфигурацион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- configuration
api_type:
- schema
ms.assetid: 6fc04e4d-657a-4999-9431-186ccb7832b5
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: 342e52e879534b6a130d286d358138c6095e4563
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761287"
---
# <a name="configuration"></a><span data-ttu-id="47918-103">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="47918-103">configuration</span></span>
  
<span data-ttu-id="47918-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="47918-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="47918-105">Элемент **Configuration** является корневым элементом для файла конфигурации агентов.</span><span class="sxs-lookup"><span data-stu-id="47918-105">The **configuration** element is the root element for the agents configuration file.</span></span> 
  
- [<span data-ttu-id="47918-106">configuration</span><span class="sxs-lookup"><span data-stu-id="47918-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="47918-107">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="47918-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

<span data-ttu-id="47918-108">**Конфигуратионтипе (complexType)**</span><span class="sxs-lookup"><span data-stu-id="47918-108">**configurationType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="47918-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="47918-109">Attributes and elements</span></span>

<span data-ttu-id="47918-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="47918-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47918-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="47918-111">Attributes</span></span>

<span data-ttu-id="47918-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="47918-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47918-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="47918-113">Child elements</span></span>

|<span data-ttu-id="47918-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="47918-114">**Element**</span></span>|<span data-ttu-id="47918-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="47918-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47918-116">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="47918-116">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="47918-117">Содержит элементы, определяющие сведения о конфигурации для мониторинга агентов и сведения о конфигурации для установленных агентов SMTP и маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="47918-117">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47918-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="47918-118">Parent elements</span></span>

<span data-ttu-id="47918-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="47918-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47918-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="47918-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47918-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="47918-121">Namespace</span></span>  <br/> |<span data-ttu-id="47918-122">В этом файле не определено пространство имен.</span><span class="sxs-lookup"><span data-stu-id="47918-122">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="47918-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="47918-123">Schema Name</span></span>  <br/> |<span data-ttu-id="47918-124">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="47918-124">Not available.</span></span>  <br/> |
|<span data-ttu-id="47918-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="47918-125">Validation File</span></span>  <br/> |<span data-ttu-id="47918-126">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="47918-126">Not available.</span></span>  <br/> |
|<span data-ttu-id="47918-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="47918-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="47918-128">Неверно.</span><span class="sxs-lookup"><span data-stu-id="47918-128">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47918-129">См. также</span><span class="sxs-lookup"><span data-stu-id="47918-129">See also</span></span>

- [<span data-ttu-id="47918-130">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="47918-130">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

