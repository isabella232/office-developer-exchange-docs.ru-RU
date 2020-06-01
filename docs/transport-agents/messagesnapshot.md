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
ms.openlocfilehash: 8a58444580c803efb7312df95d75d697bc42e8e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461844"
---
# <a name="messagesnapshot"></a><span data-ttu-id="016bd-103">мессажеснапшот</span><span class="sxs-lookup"><span data-stu-id="016bd-103">messageSnapshot</span></span>

<span data-ttu-id="016bd-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="016bd-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="016bd-105">Элемент **мессажеснапшот** содержит атрибут, указывающий, включена ли функция трассировки конвейера для сервера Exchange, на котором установлена роль сервера клиентского доступа или сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="016bd-105">The **messageSnapshot** element contains an attribute that specifies whether the pipeline tracing feature is enabled for the Exchange server that has the Client Access or the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="016bd-106">configuration</span><span class="sxs-lookup"><span data-stu-id="016bd-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="016bd-107">мексрунтиме</span><span class="sxs-lookup"><span data-stu-id="016bd-107">mexRuntime</span></span>](mexruntime.md) 
- [<span data-ttu-id="016bd-108">текущего</span><span class="sxs-lookup"><span data-stu-id="016bd-108">monitoring</span></span>](monitoring.md) 
- [<span data-ttu-id="016bd-109">мессажеснапшот</span><span class="sxs-lookup"><span data-stu-id="016bd-109">messageSnapshot</span></span>](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

<span data-ttu-id="016bd-110">**Мессажеснапшоттипе (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="016bd-110">**messageSnapshotType (Boolean)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="016bd-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="016bd-111">Attributes and elements</span></span>

<span data-ttu-id="016bd-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="016bd-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="016bd-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="016bd-113">Attributes</span></span>

|<span data-ttu-id="016bd-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="016bd-114">**Attribute**</span></span>|<span data-ttu-id="016bd-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="016bd-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="016bd-116">**enabled**</span><span class="sxs-lookup"><span data-stu-id="016bd-116">**enabled**</span></span> <br/> |<span data-ttu-id="016bd-117">Логическое значение, которое указывает, включена ли функция трассировки конвейера для клиентского доступа или сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="016bd-117">A Boolean value that indicates whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span> <span data-ttu-id="016bd-118">Значение **true** , если включена трассировка конвейера; в противном случае — значение **false** или элемент отсутствует.</span><span class="sxs-lookup"><span data-stu-id="016bd-118">The value is **true** if pipeline tracing is enabled; otherwise, the value is **false** or the element is not present.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="016bd-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="016bd-119">Child elements</span></span>

<span data-ttu-id="016bd-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="016bd-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="016bd-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="016bd-121">Parent elements</span></span>

|<span data-ttu-id="016bd-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="016bd-122">**Element**</span></span>|<span data-ttu-id="016bd-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="016bd-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="016bd-124">текущего</span><span class="sxs-lookup"><span data-stu-id="016bd-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="016bd-125">Содержит сведения о конфигурации, определяющие, как и когда служба транспорта наблюдает за установленными агентами.</span><span class="sxs-lookup"><span data-stu-id="016bd-125">Contains configuration information that defines how and when the transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="016bd-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="016bd-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="016bd-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="016bd-127">Namespace</span></span>  <br/> |<span data-ttu-id="016bd-128">В этом файле не определено пространство имен.</span><span class="sxs-lookup"><span data-stu-id="016bd-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="016bd-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="016bd-129">Schema Name</span></span>  <br/> |<span data-ttu-id="016bd-130">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="016bd-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="016bd-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="016bd-131">Validation File</span></span>  <br/> |<span data-ttu-id="016bd-132">Недоступно.</span><span class="sxs-lookup"><span data-stu-id="016bd-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="016bd-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="016bd-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="016bd-134">Неверно.</span><span class="sxs-lookup"><span data-stu-id="016bd-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="016bd-135">См. также</span><span class="sxs-lookup"><span data-stu-id="016bd-135">See also</span></span>

- [<span data-ttu-id="016bd-136">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="016bd-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

