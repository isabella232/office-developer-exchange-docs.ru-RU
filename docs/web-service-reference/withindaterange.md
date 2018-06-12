---
title: WithinDateRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WithinDateRange
api_type:
- schema
ms.assetid: 226aeb15-016f-45ca-992a-c137ba09ca08
description: Элемент WithinDateRange указывает диапазон дат, в течение которого нужно были получены в порядке для условие или исключение для применения входящих сообщений.
ms.openlocfilehash: d85ef91c581008c2aafb06b1900c4514aebacd65
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840513"
---
# <a name="withindaterange"></a><span data-ttu-id="5564d-103">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="5564d-103">WithinDateRange</span></span>

<span data-ttu-id="5564d-104">Элемент **WithinDateRange** указывает диапазон дат, в течение которого нужно были получены в порядке для условие или исключение для применения входящих сообщений.</span><span class="sxs-lookup"><span data-stu-id="5564d-104">The **WithinDateRange** element specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinDateRange>
     <StartDateTime/>
     <EndDateTime/>
</WithinDateRange>
```

 <span data-ttu-id="5564d-105">**RulePredicateDateRangeType**</span><span class="sxs-lookup"><span data-stu-id="5564d-105">**RulePredicateDateRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5564d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5564d-106">Attributes and elements</span></span>

<span data-ttu-id="5564d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5564d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5564d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5564d-108">Attributes</span></span>

<span data-ttu-id="5564d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5564d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5564d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5564d-110">Child elements</span></span>

|<span data-ttu-id="5564d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5564d-111">**Element**</span></span>|<span data-ttu-id="5564d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5564d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5564d-113">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="5564d-113">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="5564d-114">Задает правило, которое периода времени и указывает, что правило условие выполняется после это значение.</span><span class="sxs-lookup"><span data-stu-id="5564d-114">Specifies the rule time period and indicates that the rule condition is met after this value.</span></span>  <br/> |
|[<span data-ttu-id="5564d-115">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="5564d-115">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="5564d-116">Задает правило, которое периода времени и указывает, что правило условие выполняется, прежде чем это значение.</span><span class="sxs-lookup"><span data-stu-id="5564d-116">Specifies the rule time period and indicates that the rule condition is met before this value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5564d-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5564d-117">Parent elements</span></span>

|<span data-ttu-id="5564d-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5564d-118">**Element**</span></span>|<span data-ttu-id="5564d-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5564d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5564d-120">Условия</span><span class="sxs-lookup"><span data-stu-id="5564d-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="5564d-121">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="5564d-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="5564d-122">Исключения</span><span class="sxs-lookup"><span data-stu-id="5564d-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="5564d-123">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="5564d-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5564d-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5564d-124">Text value</span></span>

<span data-ttu-id="5564d-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="5564d-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5564d-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="5564d-126">Remarks</span></span>

<span data-ttu-id="5564d-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5564d-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5564d-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5564d-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5564d-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5564d-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5564d-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5564d-130">Schema Name</span></span>  <br/> |<span data-ttu-id="5564d-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5564d-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5564d-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5564d-132">Validation File</span></span>  <br/> |<span data-ttu-id="5564d-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5564d-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5564d-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5564d-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="5564d-135">True</span><span class="sxs-lookup"><span data-stu-id="5564d-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5564d-136">См. также</span><span class="sxs-lookup"><span data-stu-id="5564d-136">See also</span></span>



- [<span data-ttu-id="5564d-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5564d-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

