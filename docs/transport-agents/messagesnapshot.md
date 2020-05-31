---
title: мессажеснапшот
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- messageSnapshot
api_type:
- schema
ms.assetid: f157e44c-b950-463f-b086-31d5da94b7ff
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: 4b814def8eef8fb452d2e754c5f6787d644055f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761314"
---
# <a name="messagesnapshot"></a><span data-ttu-id="32611-103">мессажеснапшот</span><span class="sxs-lookup"><span data-stu-id="32611-103">messageSnapshot</span></span>

<span data-ttu-id="32611-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="32611-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="32611-105">Элемент **мессажеснапшот** содержит атрибут, указывающий, включена ли функция трассировки конвейера для сервера Exchange, на котором установлена роль сервера клиентского доступа или сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="32611-105">The **messageSnapshot** element contains an attribute that specifies whether the pipeline tracing feature is enabled for the Exchange server that has the Client Access or the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="32611-106">configuration</span><span class="sxs-lookup"><span data-stu-id="32611-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="32611-107">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="32611-107">mexRuntime</span></span>](mexruntime.md) 
- [<span data-ttu-id="32611-108">текущего</span><span class="sxs-lookup"><span data-stu-id="32611-108">monitoring</span></span>](monitoring.md) 
- [<span data-ttu-id="32611-109">мессажеснапшот</span><span class="sxs-lookup"><span data-stu-id="32611-109">messageSnapshot</span></span>](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

<span data-ttu-id="32611-110">**Мессажеснапшоттипе (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="32611-110">**messageSnapshotType (Boolean)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="32611-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="32611-111">Attributes and elements</span></span>

<span data-ttu-id="32611-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="32611-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32611-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="32611-113">Attributes</span></span>

|<span data-ttu-id="32611-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="32611-114">**Attribute**</span></span>|<span data-ttu-id="32611-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="32611-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32611-116">**enabled**</span><span class="sxs-lookup"><span data-stu-id="32611-116">**enabled**</span></span> <br/> |<span data-ttu-id="32611-117">Логическое значение, которое указывает, включена ли функция трассировки конвейера для клиентского доступа или сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="32611-117">A Boolean value that indicates whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span> <span data-ttu-id="32611-118">Значение **true** , если включена трассировка конвейера; в противном случае — значение **false** или элемент отсутствует.</span><span class="sxs-lookup"><span data-stu-id="32611-118">The value is **true** if pipeline tracing is enabled; otherwise, the value is **false** or the element is not present.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="32611-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="32611-119">Child elements</span></span>

<span data-ttu-id="32611-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="32611-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32611-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="32611-121">Parent elements</span></span>

|<span data-ttu-id="32611-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="32611-122">**Element**</span></span>|<span data-ttu-id="32611-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="32611-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32611-124">текущего</span><span class="sxs-lookup"><span data-stu-id="32611-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="32611-125">Содержит сведения о конфигурации, определяющие, как и когда служба транспорта наблюдает за установленными агентами.</span><span class="sxs-lookup"><span data-stu-id="32611-125">Contains configuration information that defines how and when the transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="32611-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="32611-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32611-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="32611-127">Namespace</span></span>  <br/> |<span data-ttu-id="32611-128">В этом файле не определено пространство имен.</span><span class="sxs-lookup"><span data-stu-id="32611-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="32611-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="32611-129">Schema Name</span></span>  <br/> |<span data-ttu-id="32611-130">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="32611-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="32611-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="32611-131">Validation File</span></span>  <br/> |<span data-ttu-id="32611-132">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="32611-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="32611-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="32611-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="32611-134">Неверно.</span><span class="sxs-lookup"><span data-stu-id="32611-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32611-135">См. также</span><span class="sxs-lookup"><span data-stu-id="32611-135">See also</span></span>

- [<span data-ttu-id="32611-136">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="32611-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

