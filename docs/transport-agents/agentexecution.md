---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 5848d52a68c8c3f747614015e49becb34bc4cfd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761283"
---
# <a name="agentexecution"></a><span data-ttu-id="a5aa5-103">agentExecution</span><span class="sxs-lookup"><span data-stu-id="a5aa5-103">agentExecution</span></span>
  
<span data-ttu-id="a5aa5-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="a5aa5-104">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="a5aa5-105">Элемент **agentExecution** определяет время, в миллисекундах для сервера клиентского доступа или почтовых ящиков ожидания агента для возврата из события перед записывает в журнал событий.</span><span class="sxs-lookup"><span data-stu-id="a5aa5-105">The **agentExecution** element defines the time, in milliseconds, for the Client Access or Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span> 
  
- [<span data-ttu-id="a5aa5-106">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="a5aa5-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="a5aa5-107">мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5aa5-107">monitoring</span></span>](monitoring.md)
- [<span data-ttu-id="a5aa5-108">agentExecution</span><span class="sxs-lookup"><span data-stu-id="a5aa5-108">agentExecution</span></span>](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

<span data-ttu-id="a5aa5-109">**agentExecutionType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="a5aa5-109">**agentExecutionType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a5aa5-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a5aa5-110">Attributes and elements</span></span>

<span data-ttu-id="a5aa5-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a5aa5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5aa5-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a5aa5-112">Attributes</span></span>

|<span data-ttu-id="a5aa5-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a5aa5-113">**Attribute**</span></span>|<span data-ttu-id="a5aa5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5aa5-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a5aa5-115">**timeLimitInMilliseconds**</span><span class="sxs-lookup"><span data-stu-id="a5aa5-115">**timeLimitInMilliseconds**</span></span> <br/> |<span data-ttu-id="a5aa5-116">Значение положительное целое число, указывающее время в миллисекундах для сервера ожидания агента для возврата из события до предупреждения о записи в журнал событий.</span><span class="sxs-lookup"><span data-stu-id="a5aa5-116">A positive integer value that specifies the time, in milliseconds, for the server to wait for an agent to return from an event before it writes a warning to the event log.</span></span> <span data-ttu-id="a5aa5-117">Если это значение слишком мало, это может привести к производительности.</span><span class="sxs-lookup"><span data-stu-id="a5aa5-117">Performance can decrease if this value is too small.</span></span> <span data-ttu-id="a5aa5-118">Предлагаемое значение этого атрибута — 300 000, что составляет 5 минут.</span><span class="sxs-lookup"><span data-stu-id="a5aa5-118">The suggested value for this attribute is 300,000, which equates to 5 minutes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a5aa5-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a5aa5-119">Child elements</span></span>

<span data-ttu-id="a5aa5-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5aa5-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a5aa5-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a5aa5-121">Parent elements</span></span>

|<span data-ttu-id="a5aa5-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5aa5-122">**Element**</span></span>|<span data-ttu-id="a5aa5-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5aa5-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5aa5-124">мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5aa5-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="a5aa5-125">Содержит сведения о конфигурации, который определяет, как и когда служба транспорта переднего плана или службу транспорта отслеживает агентов, которые устанавливаются.</span><span class="sxs-lookup"><span data-stu-id="a5aa5-125">Contains configuration information that defines how and when the Front End Transport service or the Transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="a5aa5-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a5aa5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5aa5-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a5aa5-127">Namespace</span></span>  <br/> |<span data-ttu-id="a5aa5-128">Этот файл не определяет пространство имен.</span><span class="sxs-lookup"><span data-stu-id="a5aa5-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="a5aa5-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a5aa5-129">Schema Name</span></span>  <br/> |<span data-ttu-id="a5aa5-130">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="a5aa5-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="a5aa5-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a5aa5-131">Validation File</span></span>  <br/> |<span data-ttu-id="a5aa5-132">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="a5aa5-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="a5aa5-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a5aa5-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5aa5-134">false</span><span class="sxs-lookup"><span data-stu-id="a5aa5-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5aa5-135">См. также</span><span class="sxs-lookup"><span data-stu-id="a5aa5-135">See also</span></span>

- [<span data-ttu-id="a5aa5-136">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a5aa5-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

