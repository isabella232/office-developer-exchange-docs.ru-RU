---
title: ItemClasses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemClasses
api_type:
- schema
ms.assetid: f95430cc-2860-47c1-af2d-8c4156c9b281
description: Элемент ItemClasses представляет классов элементов, которые необходимо ставится отметка для входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 70a4823f9017ba8c6f894394d5907f1adeb80167
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834148"
---
# <a name="itemclasses"></a><span data-ttu-id="df808-103">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="df808-103">ItemClasses</span></span>

<span data-ttu-id="df808-104">Элемент **ItemClasses** представляет классов элементов, которые необходимо ставится отметка для входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="df808-104">The **ItemClasses** element represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="df808-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="df808-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df808-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="df808-106">Attributes and elements</span></span>

<span data-ttu-id="df808-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="df808-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df808-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="df808-108">Attributes</span></span>

<span data-ttu-id="df808-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="df808-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df808-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="df808-110">Child elements</span></span>

|<span data-ttu-id="df808-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="df808-111">**Element**</span></span>|<span data-ttu-id="df808-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="df808-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df808-113">Строка</span><span class="sxs-lookup"><span data-stu-id="df808-113">String</span></span>](string.md) <br/> |<span data-ttu-id="df808-114">Представляет один элемент класса.</span><span class="sxs-lookup"><span data-stu-id="df808-114">Represents a single item class.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="df808-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="df808-115">Parent elements</span></span>

|<span data-ttu-id="df808-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="df808-116">**Element**</span></span>|<span data-ttu-id="df808-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="df808-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df808-118">Условия</span><span class="sxs-lookup"><span data-stu-id="df808-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="df808-119">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="df808-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="df808-120">Исключения</span><span class="sxs-lookup"><span data-stu-id="df808-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="df808-121">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="df808-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="df808-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="df808-122">Text value</span></span>

<span data-ttu-id="df808-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="df808-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="df808-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="df808-124">Remarks</span></span>

<span data-ttu-id="df808-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="df808-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="df808-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="df808-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df808-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="df808-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="df808-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="df808-128">Schema name</span></span>  <br/> |<span data-ttu-id="df808-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="df808-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="df808-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="df808-130">Validation file</span></span>  <br/> |<span data-ttu-id="df808-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="df808-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="df808-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="df808-132">Can be empty</span></span>  <br/> |<span data-ttu-id="df808-133">False</span><span class="sxs-lookup"><span data-stu-id="df808-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="df808-134">См. также</span><span class="sxs-lookup"><span data-stu-id="df808-134">See also</span></span>



- [<span data-ttu-id="df808-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="df808-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

