---
title: ажентексекутион
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
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: 457257e59fb37659daf2f91b0fa5dfced5c48c03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44446492"
---
# <a name="agentexecution"></a><span data-ttu-id="9abef-103">ажентексекутион</span><span class="sxs-lookup"><span data-stu-id="9abef-103">agentExecution</span></span>
  
<span data-ttu-id="9abef-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="9abef-104">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="9abef-105">Элемент **ажентексекутион** определяет время в миллисекундах, в течение которого сервер клиентского доступа или почтовых ящиков должен подождать, пока агент вернется из события, прежде чем запишет в журнал событий.</span><span class="sxs-lookup"><span data-stu-id="9abef-105">The **agentExecution** element defines the time, in milliseconds, for the Client Access or Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span> 
  
- [<span data-ttu-id="9abef-106">configuration</span><span class="sxs-lookup"><span data-stu-id="9abef-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="9abef-107">текущего</span><span class="sxs-lookup"><span data-stu-id="9abef-107">monitoring</span></span>](monitoring.md)
- [<span data-ttu-id="9abef-108">ажентексекутион</span><span class="sxs-lookup"><span data-stu-id="9abef-108">agentExecution</span></span>](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

<span data-ttu-id="9abef-109">**Ажентексекутионтипе (complexType)**</span><span class="sxs-lookup"><span data-stu-id="9abef-109">**agentExecutionType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9abef-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9abef-110">Attributes and elements</span></span>

<span data-ttu-id="9abef-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9abef-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9abef-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9abef-112">Attributes</span></span>

|<span data-ttu-id="9abef-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="9abef-113">**Attribute**</span></span>|<span data-ttu-id="9abef-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9abef-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9abef-115">**тимелимитинмиллисекондс**</span><span class="sxs-lookup"><span data-stu-id="9abef-115">**timeLimitInMilliseconds**</span></span> <br/> |<span data-ttu-id="9abef-116">Положительное целое число, задающее время ожидания (в миллисекундах) ожидания агентом возврата из события до записи предупреждения в журнал событий.</span><span class="sxs-lookup"><span data-stu-id="9abef-116">A positive integer value that specifies the time, in milliseconds, for the server to wait for an agent to return from an event before it writes a warning to the event log.</span></span> <span data-ttu-id="9abef-117">Если это значение слишком мало, производительность может снизиться.</span><span class="sxs-lookup"><span data-stu-id="9abef-117">Performance can decrease if this value is too small.</span></span> <span data-ttu-id="9abef-118">Предлагаемое значение для этого атрибута — 300 000, равное 5 минутам.</span><span class="sxs-lookup"><span data-stu-id="9abef-118">The suggested value for this attribute is 300,000, which equates to 5 minutes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9abef-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9abef-119">Child elements</span></span>

<span data-ttu-id="9abef-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9abef-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9abef-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9abef-121">Parent elements</span></span>

|<span data-ttu-id="9abef-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9abef-122">**Element**</span></span>|<span data-ttu-id="9abef-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9abef-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9abef-124">текущего</span><span class="sxs-lookup"><span data-stu-id="9abef-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="9abef-125">Содержит сведения о конфигурации, определяющие, как и когда внешняя служба транспорта или служба транспорта наблюдает за установленными агентами.</span><span class="sxs-lookup"><span data-stu-id="9abef-125">Contains configuration information that defines how and when the Front End Transport service or the Transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="9abef-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9abef-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9abef-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="9abef-127">Namespace</span></span>  <br/> |<span data-ttu-id="9abef-128">В этом файле не определено пространство имен.</span><span class="sxs-lookup"><span data-stu-id="9abef-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="9abef-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9abef-129">Schema Name</span></span>  <br/> |<span data-ttu-id="9abef-130">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="9abef-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="9abef-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9abef-131">Validation File</span></span>  <br/> |<span data-ttu-id="9abef-132">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="9abef-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="9abef-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9abef-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="9abef-134">Неверно.</span><span class="sxs-lookup"><span data-stu-id="9abef-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9abef-135">См. также</span><span class="sxs-lookup"><span data-stu-id="9abef-135">See also</span></span>

- [<span data-ttu-id="9abef-136">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9abef-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

