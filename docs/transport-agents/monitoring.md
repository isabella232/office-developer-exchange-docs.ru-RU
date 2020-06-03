---
title: текущего
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
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: 5614ac2c6428da9b6845769a9335486d3ded5754
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455830"
---
# <a name="monitoring"></a><span data-ttu-id="cf7f2-103">текущего</span><span class="sxs-lookup"><span data-stu-id="cf7f2-103">monitoring</span></span>
  
<span data-ttu-id="cf7f2-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="cf7f2-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="cf7f2-105">Элемент **Monitor** содержит сведения о конфигурации, которые определяют, как и когда внешняя служба транспорта или служба транспорта наблюдает за установленными агентами.</span><span class="sxs-lookup"><span data-stu-id="cf7f2-105">The **monitoring** element contains configuration information that defines how and when the Front End transport service or the Transport service monitors agents that are installed.</span></span> 
  
- [<span data-ttu-id="cf7f2-106">configuration</span><span class="sxs-lookup"><span data-stu-id="cf7f2-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="cf7f2-107">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="cf7f2-107">mexRuntime</span></span>](mexruntime.md)  
- [<span data-ttu-id="cf7f2-108">текущего</span><span class="sxs-lookup"><span data-stu-id="cf7f2-108">monitoring</span></span>](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

<span data-ttu-id="cf7f2-109">**Мониторингтипе (complexType)**</span><span class="sxs-lookup"><span data-stu-id="cf7f2-109">**monitoringType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cf7f2-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cf7f2-110">Attributes and elements</span></span>

<span data-ttu-id="cf7f2-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cf7f2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf7f2-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cf7f2-112">Attributes</span></span>

<span data-ttu-id="cf7f2-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cf7f2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf7f2-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cf7f2-114">Child elements</span></span>

|<span data-ttu-id="cf7f2-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf7f2-115">**Element**</span></span>|<span data-ttu-id="cf7f2-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf7f2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf7f2-117">ажентексекутион</span><span class="sxs-lookup"><span data-stu-id="cf7f2-117">agentExecution</span></span>](agentexecution.md) <br/> |<span data-ttu-id="cf7f2-118">Определяет время в миллисекундах для клиентского доступа или сервера почтовых ящиков для ожидания возврата агентом из события перед записью в журнал событий.</span><span class="sxs-lookup"><span data-stu-id="cf7f2-118">Defines the time, in milliseconds, for the Client Access or the Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span>  <br/> |
|[<span data-ttu-id="cf7f2-119">мессажеснапшот</span><span class="sxs-lookup"><span data-stu-id="cf7f2-119">messageSnapshot</span></span>](messagesnapshot.md) <br/> |<span data-ttu-id="cf7f2-120">Содержит атрибут, указывающий, включена ли функция трассировки конвейера для клиентского доступа или сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="cf7f2-120">Contains an attribute that specifies whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf7f2-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cf7f2-121">Parent elements</span></span>

|<span data-ttu-id="cf7f2-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf7f2-122">**Element**</span></span>|<span data-ttu-id="cf7f2-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf7f2-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf7f2-124">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="cf7f2-124">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="cf7f2-125">Содержит элементы, определяющие сведения о конфигурации для мониторинга агентов и сведения о конфигурации для установленных агентов SMTP и маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="cf7f2-125">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="cf7f2-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cf7f2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf7f2-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="cf7f2-127">Namespace</span></span>  <br/> |<span data-ttu-id="cf7f2-128">В этом файле не определено пространство имен.</span><span class="sxs-lookup"><span data-stu-id="cf7f2-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="cf7f2-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cf7f2-129">Schema Name</span></span>  <br/> |<span data-ttu-id="cf7f2-130">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="cf7f2-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="cf7f2-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cf7f2-131">Validation File</span></span>  <br/> |<span data-ttu-id="cf7f2-132">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="cf7f2-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="cf7f2-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cf7f2-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf7f2-134">Неверно.</span><span class="sxs-lookup"><span data-stu-id="cf7f2-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf7f2-135">См. также</span><span class="sxs-lookup"><span data-stu-id="cf7f2-135">See also</span></span>

- [<span data-ttu-id="cf7f2-136">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="cf7f2-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

