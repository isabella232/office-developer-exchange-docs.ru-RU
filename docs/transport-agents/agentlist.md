---
title: ажентлист
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentList
api_type:
- schema
ms.assetid: e877b7ef-e303-4270-964d-8d116ff2a865
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: 99e4e24c3bca77c7e7d5f2c59bb21cee1317fed2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44446394"
---
# <a name="agentlist"></a><span data-ttu-id="5e238-103">ажентлист</span><span class="sxs-lookup"><span data-stu-id="5e238-103">agentList</span></span>
  
<span data-ttu-id="5e238-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="5e238-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="5e238-105">Элемент **ажентлист** содержит элемент [Agent](agent.md) для каждого установленного агента.</span><span class="sxs-lookup"><span data-stu-id="5e238-105">The **agentList** element contains an [agent](agent.md) element for each installed agent.</span></span> 
  
- [<span data-ttu-id="5e238-106">configuration</span><span class="sxs-lookup"><span data-stu-id="5e238-106">configuration</span></span>](configuration.md)
- [<span data-ttu-id="5e238-107">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="5e238-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="5e238-108">ажентлист</span><span class="sxs-lookup"><span data-stu-id="5e238-108">agentList</span></span>](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

<span data-ttu-id="5e238-109">**Ажентлисттипе (complexType)**</span><span class="sxs-lookup"><span data-stu-id="5e238-109">**agentListType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5e238-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5e238-110">Attributes and elements</span></span>

<span data-ttu-id="5e238-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5e238-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e238-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5e238-112">Attributes</span></span>

<span data-ttu-id="5e238-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5e238-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e238-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5e238-114">Child elements</span></span>

|<span data-ttu-id="5e238-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5e238-115">**Element**</span></span>|<span data-ttu-id="5e238-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e238-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e238-117">агента</span><span class="sxs-lookup"><span data-stu-id="5e238-117">agent</span></span>](agent.md) <br/> |<span data-ttu-id="5e238-118">Содержит сведения о конфигурации установленного агента.</span><span class="sxs-lookup"><span data-stu-id="5e238-118">Contains configuration information about an installed agent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5e238-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5e238-119">Parent elements</span></span>

|<span data-ttu-id="5e238-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5e238-120">**Element**</span></span>|<span data-ttu-id="5e238-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e238-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e238-122">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="5e238-122">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="5e238-123">Содержит элементы, определяющие сведения о конфигурации для мониторинга агентов и сведения о конфигурации установленных агентов.</span><span class="sxs-lookup"><span data-stu-id="5e238-123">Contains elements that define configuration information for agent monitoring and configuration information about installed agents.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="5e238-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5e238-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e238-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="5e238-125">Namespace</span></span>  <br/> |<span data-ttu-id="5e238-126">В этом файле не определено пространство имен.</span><span class="sxs-lookup"><span data-stu-id="5e238-126">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="5e238-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5e238-127">Schema Name</span></span>  <br/> |<span data-ttu-id="5e238-128">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="5e238-128">Not available.</span></span>  <br/> |
|<span data-ttu-id="5e238-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5e238-129">Validation File</span></span>  <br/> |<span data-ttu-id="5e238-130">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="5e238-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="5e238-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5e238-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e238-132">Неверно.</span><span class="sxs-lookup"><span data-stu-id="5e238-132">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e238-133">См. также</span><span class="sxs-lookup"><span data-stu-id="5e238-133">See also</span></span>

- [<span data-ttu-id="5e238-134">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="5e238-134">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

