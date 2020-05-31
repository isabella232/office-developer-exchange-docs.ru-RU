---
title: висиндатеранже
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
description: Элемент Висиндатеранже указывает диапазон дат, в рамках которого должны быть получены входящие сообщения, чтобы применялось условие или исключение.
ms.openlocfilehash: d85ef91c581008c2aafb06b1900c4514aebacd65
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840513"
---
# <a name="withindaterange"></a><span data-ttu-id="28093-103">висиндатеранже</span><span class="sxs-lookup"><span data-stu-id="28093-103">WithinDateRange</span></span>

<span data-ttu-id="28093-104">Элемент **висиндатеранже** указывает диапазон дат, в рамках которого должны быть получены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="28093-104">The **WithinDateRange** element specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinDateRange>
     <StartDateTime/>
     <EndDateTime/>
</WithinDateRange>
```

 <span data-ttu-id="28093-105">**рулепредикатедатеранжетипе**</span><span class="sxs-lookup"><span data-stu-id="28093-105">**RulePredicateDateRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28093-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="28093-106">Attributes and elements</span></span>

<span data-ttu-id="28093-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="28093-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28093-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="28093-108">Attributes</span></span>

<span data-ttu-id="28093-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="28093-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28093-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="28093-110">Child elements</span></span>

|<span data-ttu-id="28093-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28093-111">**Element**</span></span>|<span data-ttu-id="28093-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28093-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28093-113">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="28093-113">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="28093-114">Задает период времени правила и указывает, что после этого значения будет выполнено условие правила.</span><span class="sxs-lookup"><span data-stu-id="28093-114">Specifies the rule time period and indicates that the rule condition is met after this value.</span></span>  <br/> |
|[<span data-ttu-id="28093-115">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="28093-115">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="28093-116">Задает период времени правила и указывает, что условие правила выполняется до этого значения.</span><span class="sxs-lookup"><span data-stu-id="28093-116">Specifies the rule time period and indicates that the rule condition is met before this value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28093-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="28093-117">Parent elements</span></span>

|<span data-ttu-id="28093-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28093-118">**Element**</span></span>|<span data-ttu-id="28093-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28093-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28093-120">Условия</span><span class="sxs-lookup"><span data-stu-id="28093-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="28093-121">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="28093-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="28093-122">Исключения</span><span class="sxs-lookup"><span data-stu-id="28093-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="28093-123">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="28093-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28093-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="28093-124">Text value</span></span>

<span data-ttu-id="28093-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="28093-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28093-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="28093-126">Remarks</span></span>

<span data-ttu-id="28093-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="28093-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28093-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="28093-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28093-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="28093-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28093-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="28093-130">Schema Name</span></span>  <br/> |<span data-ttu-id="28093-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="28093-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="28093-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="28093-132">Validation File</span></span>  <br/> |<span data-ttu-id="28093-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="28093-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28093-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="28093-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="28093-135">True</span><span class="sxs-lookup"><span data-stu-id="28093-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28093-136">См. также</span><span class="sxs-lookup"><span data-stu-id="28093-136">See also</span></span>



- [<span data-ttu-id="28093-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="28093-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

