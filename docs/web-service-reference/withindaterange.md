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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461851"
---
# <a name="withindaterange"></a><span data-ttu-id="0b2df-103">висиндатеранже</span><span class="sxs-lookup"><span data-stu-id="0b2df-103">WithinDateRange</span></span>

<span data-ttu-id="0b2df-104">Элемент **висиндатеранже** указывает диапазон дат, в рамках которого должны быть получены входящие сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="0b2df-104">The **WithinDateRange** element specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinDateRange>
     <StartDateTime/>
     <EndDateTime/>
</WithinDateRange>
```

 <span data-ttu-id="0b2df-105">**рулепредикатедатеранжетипе**</span><span class="sxs-lookup"><span data-stu-id="0b2df-105">**RulePredicateDateRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b2df-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0b2df-106">Attributes and elements</span></span>

<span data-ttu-id="0b2df-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0b2df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b2df-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0b2df-108">Attributes</span></span>

<span data-ttu-id="0b2df-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0b2df-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b2df-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0b2df-110">Child elements</span></span>

|<span data-ttu-id="0b2df-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0b2df-111">**Element**</span></span>|<span data-ttu-id="0b2df-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0b2df-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b2df-113">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="0b2df-113">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="0b2df-114">Задает период времени правила и указывает, что после этого значения будет выполнено условие правила.</span><span class="sxs-lookup"><span data-stu-id="0b2df-114">Specifies the rule time period and indicates that the rule condition is met after this value.</span></span>  <br/> |
|[<span data-ttu-id="0b2df-115">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="0b2df-115">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="0b2df-116">Задает период времени правила и указывает, что условие правила выполняется до этого значения.</span><span class="sxs-lookup"><span data-stu-id="0b2df-116">Specifies the rule time period and indicates that the rule condition is met before this value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b2df-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0b2df-117">Parent elements</span></span>

|<span data-ttu-id="0b2df-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0b2df-118">**Element**</span></span>|<span data-ttu-id="0b2df-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0b2df-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b2df-120">Условия</span><span class="sxs-lookup"><span data-stu-id="0b2df-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="0b2df-121">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="0b2df-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="0b2df-122">Исключения</span><span class="sxs-lookup"><span data-stu-id="0b2df-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="0b2df-123">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="0b2df-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0b2df-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0b2df-124">Text value</span></span>

<span data-ttu-id="0b2df-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="0b2df-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b2df-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="0b2df-126">Remarks</span></span>

<span data-ttu-id="0b2df-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b2df-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b2df-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0b2df-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b2df-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0b2df-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0b2df-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0b2df-130">Schema Name</span></span>  <br/> |<span data-ttu-id="0b2df-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0b2df-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0b2df-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0b2df-132">Validation File</span></span>  <br/> |<span data-ttu-id="0b2df-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0b2df-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0b2df-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0b2df-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b2df-135">True</span><span class="sxs-lookup"><span data-stu-id="0b2df-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b2df-136">См. также</span><span class="sxs-lookup"><span data-stu-id="0b2df-136">See also</span></span>



- [<span data-ttu-id="0b2df-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0b2df-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

