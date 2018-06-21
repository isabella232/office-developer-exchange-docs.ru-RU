---
title: Priority
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Priority
api_type:
- schema
ms.assetid: e1adb8b9-e3d5-469a-b188-822733d2503e
description: Элемент приоритет указывает порядок, в котором будет выполняться правило.
ms.openlocfilehash: 49e9bda063d8766ff49c8a2e9574c986bcfdbeb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/21/2018
ms.locfileid: "19834888"
---
# <a name="priority"></a><span data-ttu-id="372fd-103">Priority</span><span class="sxs-lookup"><span data-stu-id="372fd-103">Priority</span></span>

<span data-ttu-id="372fd-104">Элемент **приоритет** указывает порядок, в котором будет выполняться правило.</span><span class="sxs-lookup"><span data-stu-id="372fd-104">The **Priority** element indicates the order in which a rule is to be run.</span></span> 
  
```XML
<Priority/>
```

 <span data-ttu-id="372fd-105">**int**</span><span class="sxs-lookup"><span data-stu-id="372fd-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="372fd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="372fd-106">Attributes and elements</span></span>

<span data-ttu-id="372fd-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="372fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="372fd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="372fd-108">Attributes</span></span>

<span data-ttu-id="372fd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="372fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="372fd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="372fd-110">Child elements</span></span>

<span data-ttu-id="372fd-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="372fd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="372fd-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="372fd-112">Parent elements</span></span>

|<span data-ttu-id="372fd-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="372fd-113">**Element**</span></span>|<span data-ttu-id="372fd-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="372fd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="372fd-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="372fd-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="372fd-116">Представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="372fd-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="372fd-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="372fd-117">Text value</span></span>

<span data-ttu-id="372fd-118">Текстовое значение для элемента **приоритет** — целое число, указывающее порядок выполнения, в котором должна запускаться правило.</span><span class="sxs-lookup"><span data-stu-id="372fd-118">The text value for the **Priority** element is an integer that indicates the execution order in which a rule should be run.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="372fd-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="372fd-119">Remarks</span></span>

<span data-ttu-id="372fd-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="372fd-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="372fd-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="372fd-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="372fd-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="372fd-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="372fd-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="372fd-123">Schema Name</span></span>  <br/> |<span data-ttu-id="372fd-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="372fd-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="372fd-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="372fd-125">Validation File</span></span>  <br/> |<span data-ttu-id="372fd-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="372fd-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="372fd-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="372fd-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="372fd-128">False</span><span class="sxs-lookup"><span data-stu-id="372fd-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="372fd-129">См. также</span><span class="sxs-lookup"><span data-stu-id="372fd-129">See also</span></span>



- [<span data-ttu-id="372fd-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="372fd-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

