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
ms.openlocfilehash: f192965a8375eb46d1ca5b46d3b768a3299c284d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461837"
---
# <a name="mexruntime"></a><span data-ttu-id="a63ff-103">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="a63ff-103">mexRuntime</span></span>
  
<span data-ttu-id="a63ff-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="a63ff-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="a63ff-105">Элемент **мексрунтиме** содержит элементы, определяющие сведения о конфигурации для мониторинга агентов и сведения о конфигурации агентов маршрутизации SMTP и маршрутизации, которые установлены.</span><span class="sxs-lookup"><span data-stu-id="a63ff-105">The **mexRuntime** element contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span> 
  
- [<span data-ttu-id="a63ff-106">configuration</span><span class="sxs-lookup"><span data-stu-id="a63ff-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="a63ff-107">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="a63ff-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

<span data-ttu-id="a63ff-108">**Мексрунтиметипе (complexType)**</span><span class="sxs-lookup"><span data-stu-id="a63ff-108">**mexRuntimeType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a63ff-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a63ff-109">Attributes and elements</span></span>

<span data-ttu-id="a63ff-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a63ff-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a63ff-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a63ff-111">Attributes</span></span>

<span data-ttu-id="a63ff-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a63ff-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a63ff-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a63ff-113">Child elements</span></span>

|<span data-ttu-id="a63ff-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a63ff-114">**Element**</span></span>|<span data-ttu-id="a63ff-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a63ff-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a63ff-116">текущего</span><span class="sxs-lookup"><span data-stu-id="a63ff-116">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="a63ff-117">Содержит сведения о конфигурации, определяющие, как и когда транспортный монитор устанавливает агенты.</span><span class="sxs-lookup"><span data-stu-id="a63ff-117">Contains configuration information that defines how and when transport monitors agents that are installed.</span></span>  <br/> |
|[<span data-ttu-id="a63ff-118">ажентлист</span><span class="sxs-lookup"><span data-stu-id="a63ff-118">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="a63ff-119">Содержит элемент [Agent](agent.md) для каждого установленного агента.</span><span class="sxs-lookup"><span data-stu-id="a63ff-119">Contains an [agent](agent.md) element for each agent that is installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a63ff-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a63ff-120">Parent elements</span></span>

|<span data-ttu-id="a63ff-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a63ff-121">**Element**</span></span>|<span data-ttu-id="a63ff-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a63ff-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a63ff-123">configuration</span><span class="sxs-lookup"><span data-stu-id="a63ff-123">configuration</span></span>](configuration.md) <br/> |<span data-ttu-id="a63ff-124">Корневой элемент для файла конфигурации агентов.</span><span class="sxs-lookup"><span data-stu-id="a63ff-124">The root element for the agents configuration file.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="a63ff-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a63ff-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a63ff-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="a63ff-126">Namespace</span></span>  <br/> |<span data-ttu-id="a63ff-127">В этом файле не определено пространство имен.</span><span class="sxs-lookup"><span data-stu-id="a63ff-127">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="a63ff-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a63ff-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a63ff-129">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="a63ff-129">Not available.</span></span>  <br/> |
|<span data-ttu-id="a63ff-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a63ff-130">Validation File</span></span>  <br/> |<span data-ttu-id="a63ff-131">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="a63ff-131">Not available.</span></span>  <br/> |
|<span data-ttu-id="a63ff-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a63ff-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a63ff-133">Неверно.</span><span class="sxs-lookup"><span data-stu-id="a63ff-133">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a63ff-134">См. также</span><span class="sxs-lookup"><span data-stu-id="a63ff-134">See also</span></span>

- [<span data-ttu-id="a63ff-135">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a63ff-135">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

