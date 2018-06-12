---
title: messageSnapshot
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
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 4b814def8eef8fb452d2e754c5f6787d644055f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761314"
---
# <a name="messagesnapshot"></a><span data-ttu-id="0ebf1-103">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="0ebf1-103">messageSnapshot</span></span>

<span data-ttu-id="0ebf1-104">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0ebf1-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="0ebf1-105">Элемент **messageSnapshot** содержит атрибут, который указывает, включена ли функция конвейерной трассировки для Exchange server с клиентского доступа или установлена роль сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="0ebf1-105">The **messageSnapshot** element contains an attribute that specifies whether the pipeline tracing feature is enabled for the Exchange server that has the Client Access or the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="0ebf1-106">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="0ebf1-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="0ebf1-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="0ebf1-107">mexRuntime</span></span>](mexruntime.md) 
- [<span data-ttu-id="0ebf1-108">мониторинг</span><span class="sxs-lookup"><span data-stu-id="0ebf1-108">monitoring</span></span>](monitoring.md) 
- [<span data-ttu-id="0ebf1-109">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="0ebf1-109">messageSnapshot</span></span>](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

<span data-ttu-id="0ebf1-110">**messageSnapshotType (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="0ebf1-110">**messageSnapshotType (Boolean)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0ebf1-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0ebf1-111">Attributes and elements</span></span>

<span data-ttu-id="0ebf1-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0ebf1-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ebf1-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0ebf1-113">Attributes</span></span>

|<span data-ttu-id="0ebf1-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0ebf1-114">**Attribute**</span></span>|<span data-ttu-id="0ebf1-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ebf1-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0ebf1-116">**включено**</span><span class="sxs-lookup"><span data-stu-id="0ebf1-116">**enabled**</span></span> <br/> |<span data-ttu-id="0ebf1-117">Логическое значение, указывающее, включена ли функция конвейерной трассировки для клиентского доступа и сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="0ebf1-117">A Boolean value that indicates whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span> <span data-ttu-id="0ebf1-118">Значение равно **true** , если включена конвейерной трассировки. в противном случае — значение равно **false** или элемент не существует.</span><span class="sxs-lookup"><span data-stu-id="0ebf1-118">The value is **true** if pipeline tracing is enabled; otherwise, the value is **false** or the element is not present.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0ebf1-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0ebf1-119">Child elements</span></span>

<span data-ttu-id="0ebf1-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="0ebf1-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0ebf1-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0ebf1-121">Parent elements</span></span>

|<span data-ttu-id="0ebf1-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0ebf1-122">**Element**</span></span>|<span data-ttu-id="0ebf1-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ebf1-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ebf1-124">мониторинг</span><span class="sxs-lookup"><span data-stu-id="0ebf1-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="0ebf1-125">Содержит сведения о конфигурации, который определяет, как и когда транспортная служба отслеживает агентов, которые устанавливаются.</span><span class="sxs-lookup"><span data-stu-id="0ebf1-125">Contains configuration information that defines how and when the transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="0ebf1-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0ebf1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ebf1-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0ebf1-127">Namespace</span></span>  <br/> |<span data-ttu-id="0ebf1-128">Этот файл не определяет пространство имен.</span><span class="sxs-lookup"><span data-stu-id="0ebf1-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="0ebf1-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0ebf1-129">Schema Name</span></span>  <br/> |<span data-ttu-id="0ebf1-130">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="0ebf1-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="0ebf1-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0ebf1-131">Validation File</span></span>  <br/> |<span data-ttu-id="0ebf1-132">Компонент недоступен.</span><span class="sxs-lookup"><span data-stu-id="0ebf1-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="0ebf1-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0ebf1-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ebf1-134">false</span><span class="sxs-lookup"><span data-stu-id="0ebf1-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ebf1-135">См. также</span><span class="sxs-lookup"><span data-stu-id="0ebf1-135">See also</span></span>

- [<span data-ttu-id="0ebf1-136">Элементы файла конфигурации агентов для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0ebf1-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)
