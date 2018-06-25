---
title: configuration
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
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 342e52e879534b6a130d286d358138c6095e4563
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761287"
---
# <a name="configuration"></a><span data-ttu-id="b46e4-103">configuration</span><span class="sxs-lookup"><span data-stu-id="b46e4-103">configuration</span></span>
  
<span data-ttu-id="b46e4-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="b46e4-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="b46e4-105">Элемент **конфигурации** является корневым элементом для файла конфигурации агентов.</span><span class="sxs-lookup"><span data-stu-id="b46e4-105">The **configuration** element is the root element for the agents configuration file.</span></span> 
  
- [<span data-ttu-id="b46e4-106">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="b46e4-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="b46e4-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="b46e4-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

<span data-ttu-id="b46e4-108">**configurationType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="b46e4-108">**configurationType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b46e4-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b46e4-109">Attributes and elements</span></span>

<span data-ttu-id="b46e4-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b46e4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b46e4-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b46e4-111">Attributes</span></span>

<span data-ttu-id="b46e4-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="b46e4-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b46e4-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b46e4-113">Child elements</span></span>

|<span data-ttu-id="b46e4-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b46e4-114">**Element**</span></span>|<span data-ttu-id="b46e4-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b46e4-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b46e4-116">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="b46e4-116">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="b46e4-117">Содержит элементы, определяющие данные конфигурации для наблюдение за агентом и данные конфигурации для SMTP и агенты маршрутизации, которые устанавливаются.</span><span class="sxs-lookup"><span data-stu-id="b46e4-117">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b46e4-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b46e4-118">Parent elements</span></span>

<span data-ttu-id="b46e4-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="b46e4-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b46e4-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b46e4-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b46e4-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b46e4-121">Namespace</span></span>  <br/> |<span data-ttu-id="b46e4-122">Этот файл не определяет пространство имен.</span><span class="sxs-lookup"><span data-stu-id="b46e4-122">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="b46e4-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b46e4-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b46e4-124">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="b46e4-124">Not available.</span></span>  <br/> |
|<span data-ttu-id="b46e4-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b46e4-125">Validation File</span></span>  <br/> |<span data-ttu-id="b46e4-126">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="b46e4-126">Not available.</span></span>  <br/> |
|<span data-ttu-id="b46e4-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b46e4-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b46e4-128">false</span><span class="sxs-lookup"><span data-stu-id="b46e4-128">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b46e4-129">См. также</span><span class="sxs-lookup"><span data-stu-id="b46e4-129">See also</span></span>

- [<span data-ttu-id="b46e4-130">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b46e4-130">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

