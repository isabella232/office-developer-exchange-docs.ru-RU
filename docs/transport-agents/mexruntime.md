---
title: мексрунтиме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: 4a34eedfc16d64cbfa67003ed23cf6eba2bb4bad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761317"
---
# <a name="mexruntime"></a><span data-ttu-id="10170-103">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="10170-103">mexRuntime</span></span>
  
<span data-ttu-id="10170-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="10170-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="10170-105">Элемент **мексрунтиме** содержит элементы, определяющие сведения о конфигурации для мониторинга агентов и сведения о конфигурации агентов маршрутизации SMTP и маршрутизации, которые установлены.</span><span class="sxs-lookup"><span data-stu-id="10170-105">The **mexRuntime** element contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span> 
  
- [<span data-ttu-id="10170-106">configuration</span><span class="sxs-lookup"><span data-stu-id="10170-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="10170-107">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="10170-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

<span data-ttu-id="10170-108">**Мексрунтиметипе (complexType)**</span><span class="sxs-lookup"><span data-stu-id="10170-108">**mexRuntimeType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="10170-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="10170-109">Attributes and elements</span></span>

<span data-ttu-id="10170-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="10170-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10170-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="10170-111">Attributes</span></span>

<span data-ttu-id="10170-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="10170-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10170-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="10170-113">Child elements</span></span>

|<span data-ttu-id="10170-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="10170-114">**Element**</span></span>|<span data-ttu-id="10170-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="10170-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10170-116">текущего</span><span class="sxs-lookup"><span data-stu-id="10170-116">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="10170-117">Содержит сведения о конфигурации, определяющие, как и когда транспортный монитор устанавливает агенты.</span><span class="sxs-lookup"><span data-stu-id="10170-117">Contains configuration information that defines how and when transport monitors agents that are installed.</span></span>  <br/> |
|[<span data-ttu-id="10170-118">ажентлист</span><span class="sxs-lookup"><span data-stu-id="10170-118">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="10170-119">Содержит элемент [Agent](agent.md) для каждого установленного агента.</span><span class="sxs-lookup"><span data-stu-id="10170-119">Contains an [agent](agent.md) element for each agent that is installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="10170-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="10170-120">Parent elements</span></span>

|<span data-ttu-id="10170-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="10170-121">**Element**</span></span>|<span data-ttu-id="10170-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="10170-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10170-123">configuration</span><span class="sxs-lookup"><span data-stu-id="10170-123">configuration</span></span>](configuration.md) <br/> |<span data-ttu-id="10170-124">Корневой элемент для файла конфигурации агентов.</span><span class="sxs-lookup"><span data-stu-id="10170-124">The root element for the agents configuration file.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="10170-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="10170-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10170-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="10170-126">Namespace</span></span>  <br/> |<span data-ttu-id="10170-127">В этом файле не определено пространство имен.</span><span class="sxs-lookup"><span data-stu-id="10170-127">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="10170-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="10170-128">Schema Name</span></span>  <br/> |<span data-ttu-id="10170-129">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="10170-129">Not available.</span></span>  <br/> |
|<span data-ttu-id="10170-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="10170-130">Validation File</span></span>  <br/> |<span data-ttu-id="10170-131">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="10170-131">Not available.</span></span>  <br/> |
|<span data-ttu-id="10170-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="10170-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="10170-133">Неверно.</span><span class="sxs-lookup"><span data-stu-id="10170-133">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10170-134">См. также</span><span class="sxs-lookup"><span data-stu-id="10170-134">See also</span></span>

- [<span data-ttu-id="10170-135">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="10170-135">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

