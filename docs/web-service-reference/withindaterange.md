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
ms.openlocfilehash: ef5fb15b64ee4f7060f907818c4ebd4367ced5e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461851"
---
# <a name="withindaterange"></a><span data-ttu-id="dc5f6-103">висиндатеранже</span><span class="sxs-lookup"><span data-stu-id="dc5f6-103">WithinDateRange</span></span>

<span data-ttu-id="dc5f6-104">Элемент **висиндатеранже** указывает диапазон дат, в рамках которого должны быть получены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="dc5f6-104">The **WithinDateRange** element specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinDateRange>
     <StartDateTime/>
     <EndDateTime/>
</WithinDateRange>
```

 <span data-ttu-id="dc5f6-105">**рулепредикатедатеранжетипе**</span><span class="sxs-lookup"><span data-stu-id="dc5f6-105">**RulePredicateDateRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc5f6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dc5f6-106">Attributes and elements</span></span>

<span data-ttu-id="dc5f6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dc5f6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc5f6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dc5f6-108">Attributes</span></span>

<span data-ttu-id="dc5f6-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dc5f6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc5f6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dc5f6-110">Child elements</span></span>

|<span data-ttu-id="dc5f6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dc5f6-111">**Element**</span></span>|<span data-ttu-id="dc5f6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dc5f6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc5f6-113">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="dc5f6-113">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="dc5f6-114">Задает период времени правила и указывает, что после этого значения будет выполнено условие правила.</span><span class="sxs-lookup"><span data-stu-id="dc5f6-114">Specifies the rule time period and indicates that the rule condition is met after this value.</span></span>  <br/> |
|[<span data-ttu-id="dc5f6-115">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="dc5f6-115">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="dc5f6-116">Задает период времени правила и указывает, что условие правила выполняется до этого значения.</span><span class="sxs-lookup"><span data-stu-id="dc5f6-116">Specifies the rule time period and indicates that the rule condition is met before this value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc5f6-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dc5f6-117">Parent elements</span></span>

|<span data-ttu-id="dc5f6-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dc5f6-118">**Element**</span></span>|<span data-ttu-id="dc5f6-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dc5f6-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc5f6-120">Условия</span><span class="sxs-lookup"><span data-stu-id="dc5f6-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="dc5f6-121">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="dc5f6-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="dc5f6-122">Исключения</span><span class="sxs-lookup"><span data-stu-id="dc5f6-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="dc5f6-123">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="dc5f6-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dc5f6-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dc5f6-124">Text value</span></span>

<span data-ttu-id="dc5f6-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="dc5f6-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dc5f6-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="dc5f6-126">Remarks</span></span>

<span data-ttu-id="dc5f6-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dc5f6-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc5f6-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dc5f6-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc5f6-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dc5f6-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dc5f6-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dc5f6-130">Schema Name</span></span>  <br/> |<span data-ttu-id="dc5f6-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dc5f6-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dc5f6-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dc5f6-132">Validation File</span></span>  <br/> |<span data-ttu-id="dc5f6-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dc5f6-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc5f6-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dc5f6-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc5f6-135">True</span><span class="sxs-lookup"><span data-stu-id="dc5f6-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc5f6-136">См. также</span><span class="sxs-lookup"><span data-stu-id="dc5f6-136">See also</span></span>



- [<span data-ttu-id="dc5f6-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dc5f6-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

