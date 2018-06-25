---
title: agentList
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
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 7dd9d48356932c82dbc048a85b9f02437c6366de
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761285"
---
# <a name="agentlist"></a><span data-ttu-id="3f39b-103">agentList</span><span class="sxs-lookup"><span data-stu-id="3f39b-103">agentList</span></span>
  
<span data-ttu-id="3f39b-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="3f39b-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="3f39b-105">Элемент **agentList** содержит элемент [агентов](agent.md) для каждого установленного агента.</span><span class="sxs-lookup"><span data-stu-id="3f39b-105">The **agentList** element contains an [agent](agent.md) element for each installed agent.</span></span> 
  
- [<span data-ttu-id="3f39b-106">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="3f39b-106">configuration</span></span>](configuration.md)
- [<span data-ttu-id="3f39b-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="3f39b-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="3f39b-108">agentList</span><span class="sxs-lookup"><span data-stu-id="3f39b-108">agentList</span></span>](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

<span data-ttu-id="3f39b-109">**agentListType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="3f39b-109">**agentListType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3f39b-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3f39b-110">Attributes and elements</span></span>

<span data-ttu-id="3f39b-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3f39b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f39b-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3f39b-112">Attributes</span></span>

<span data-ttu-id="3f39b-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="3f39b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f39b-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3f39b-114">Child elements</span></span>

|<span data-ttu-id="3f39b-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3f39b-115">**Element**</span></span>|<span data-ttu-id="3f39b-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f39b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f39b-117">агент</span><span class="sxs-lookup"><span data-stu-id="3f39b-117">agent</span></span>](agent.md) <br/> |<span data-ttu-id="3f39b-118">Содержит сведения о конфигурации об установленных агентов.</span><span class="sxs-lookup"><span data-stu-id="3f39b-118">Contains configuration information about an installed agent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f39b-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3f39b-119">Parent elements</span></span>

|<span data-ttu-id="3f39b-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3f39b-120">**Element**</span></span>|<span data-ttu-id="3f39b-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3f39b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f39b-122">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="3f39b-122">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="3f39b-123">Содержит элементы, определяющие данные конфигурации для наблюдение за агентом и сведений о конфигурации об установленных агентов.</span><span class="sxs-lookup"><span data-stu-id="3f39b-123">Contains elements that define configuration information for agent monitoring and configuration information about installed agents.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="3f39b-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3f39b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f39b-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3f39b-125">Namespace</span></span>  <br/> |<span data-ttu-id="3f39b-126">Этот файл не определяет пространство имен.</span><span class="sxs-lookup"><span data-stu-id="3f39b-126">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="3f39b-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3f39b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3f39b-128">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="3f39b-128">Not available.</span></span>  <br/> |
|<span data-ttu-id="3f39b-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3f39b-129">Validation File</span></span>  <br/> |<span data-ttu-id="3f39b-130">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="3f39b-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="3f39b-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3f39b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f39b-132">false</span><span class="sxs-lookup"><span data-stu-id="3f39b-132">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f39b-133">См. также</span><span class="sxs-lookup"><span data-stu-id="3f39b-133">See also</span></span>

- [<span data-ttu-id="3f39b-134">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="3f39b-134">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

