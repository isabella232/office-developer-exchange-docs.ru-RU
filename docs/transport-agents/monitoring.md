---
title: мониторинг
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- monitoring
api_type:
- schema
ms.assetid: 350d7b46-9260-41a7-8613-3cb8cc1b29a5
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 1b5484467def0bf3d22ba0707357977d5ed461ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761313"
---
# <a name="monitoring"></a><span data-ttu-id="101cf-103">мониторинг</span><span class="sxs-lookup"><span data-stu-id="101cf-103">monitoring</span></span>
  
<span data-ttu-id="101cf-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="101cf-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="101cf-105">Элемент **мониторинга** содержит сведения о конфигурации, который определяет, как и когда транспортная служба переднего плана или службу транспорта отслеживает агентов, которые устанавливаются.</span><span class="sxs-lookup"><span data-stu-id="101cf-105">The **monitoring** element contains configuration information that defines how and when the Front End transport service or the Transport service monitors agents that are installed.</span></span> 
  
- [<span data-ttu-id="101cf-106">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="101cf-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="101cf-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="101cf-107">mexRuntime</span></span>](mexruntime.md)  
- [<span data-ttu-id="101cf-108">мониторинг</span><span class="sxs-lookup"><span data-stu-id="101cf-108">monitoring</span></span>](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

<span data-ttu-id="101cf-109">**monitoringType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="101cf-109">**monitoringType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="101cf-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="101cf-110">Attributes and elements</span></span>

<span data-ttu-id="101cf-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="101cf-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="101cf-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="101cf-112">Attributes</span></span>

<span data-ttu-id="101cf-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="101cf-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="101cf-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="101cf-114">Child elements</span></span>

|<span data-ttu-id="101cf-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="101cf-115">**Element**</span></span>|<span data-ttu-id="101cf-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="101cf-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="101cf-117">agentExecution</span><span class="sxs-lookup"><span data-stu-id="101cf-117">agentExecution</span></span>](agentexecution.md) <br/> |<span data-ttu-id="101cf-118">Задает время в миллисекундах для клиентского доступа или сервера почтовых ящиков ожидания агента для возврата из события перед записывает в журнал событий.</span><span class="sxs-lookup"><span data-stu-id="101cf-118">Defines the time, in milliseconds, for the Client Access or the Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span>  <br/> |
|[<span data-ttu-id="101cf-119">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="101cf-119">messageSnapshot</span></span>](messagesnapshot.md) <br/> |<span data-ttu-id="101cf-120">Содержит атрибут, который указывает, включена ли функция конвейерной трассировки для клиентского доступа и сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="101cf-120">Contains an attribute that specifies whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="101cf-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="101cf-121">Parent elements</span></span>

|<span data-ttu-id="101cf-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="101cf-122">**Element**</span></span>|<span data-ttu-id="101cf-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="101cf-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="101cf-124">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="101cf-124">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="101cf-125">Содержит элементы, определяющие данные конфигурации для наблюдение за агентом и данные конфигурации для SMTP и агенты маршрутизации, которые устанавливаются.</span><span class="sxs-lookup"><span data-stu-id="101cf-125">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="101cf-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="101cf-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="101cf-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="101cf-127">Namespace</span></span>  <br/> |<span data-ttu-id="101cf-128">Этот файл не определяет пространство имен.</span><span class="sxs-lookup"><span data-stu-id="101cf-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="101cf-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="101cf-129">Schema Name</span></span>  <br/> |<span data-ttu-id="101cf-130">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="101cf-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="101cf-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="101cf-131">Validation File</span></span>  <br/> |<span data-ttu-id="101cf-132">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="101cf-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="101cf-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="101cf-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="101cf-134">false</span><span class="sxs-lookup"><span data-stu-id="101cf-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="101cf-135">См. также</span><span class="sxs-lookup"><span data-stu-id="101cf-135">See also</span></span>

- [<span data-ttu-id="101cf-136">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="101cf-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

