---
title: флагжедфорактион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlaggedForAction
api_type:
- schema
ms.assetid: 6a08c48a-7b32-4754-8940-adbda55e8133
description: Элемент Флагжедфорактион указывает флаг для значения действия, который должен отображаться в входящих сообщениях, чтобы применить условие или исключение.
ms.openlocfilehash: f996dc4bcf30db32e1d73fb302ab137f0a6ad4d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466243"
---
# <a name="flaggedforaction"></a><span data-ttu-id="07b6d-103">флагжедфорактион</span><span class="sxs-lookup"><span data-stu-id="07b6d-103">FlaggedForAction</span></span>

<span data-ttu-id="07b6d-104">Элемент **флагжедфорактион** указывает флаг для значения действия, который должен отображаться в входящих сообщениях, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="07b6d-104">The **FlaggedForAction** element specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<FlaggedForAction/>
```

 <span data-ttu-id="07b6d-105">**флагжедфорактионтипе**</span><span class="sxs-lookup"><span data-stu-id="07b6d-105">**FlaggedForActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07b6d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="07b6d-106">Attributes and elements</span></span>

<span data-ttu-id="07b6d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="07b6d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07b6d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="07b6d-108">Attributes</span></span>

<span data-ttu-id="07b6d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="07b6d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07b6d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="07b6d-110">Child elements</span></span>

<span data-ttu-id="07b6d-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="07b6d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="07b6d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="07b6d-112">Parent elements</span></span>

|<span data-ttu-id="07b6d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="07b6d-113">**Element**</span></span>|<span data-ttu-id="07b6d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07b6d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07b6d-115">Условия</span><span class="sxs-lookup"><span data-stu-id="07b6d-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="07b6d-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="07b6d-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="07b6d-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="07b6d-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="07b6d-118">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="07b6d-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="07b6d-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="07b6d-119">Text value</span></span>

<span data-ttu-id="07b6d-120">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="07b6d-120">A text value is required.</span></span> <span data-ttu-id="07b6d-121">Ниже приведены возможные текстовые значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="07b6d-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="07b6d-122">Любые</span><span class="sxs-lookup"><span data-stu-id="07b6d-122">Any</span></span>
    
- <span data-ttu-id="07b6d-123">Звонок</span><span class="sxs-lookup"><span data-stu-id="07b6d-123">Call</span></span>
    
- <span data-ttu-id="07b6d-124">донотфорвард</span><span class="sxs-lookup"><span data-stu-id="07b6d-124">DoNotForward</span></span>
    
- <span data-ttu-id="07b6d-125">Следующего</span><span class="sxs-lookup"><span data-stu-id="07b6d-125">FollowUp</span></span>
    
- <span data-ttu-id="07b6d-126">СВЕДЕНИЮ</span><span class="sxs-lookup"><span data-stu-id="07b6d-126">FYI</span></span>
    
- <span data-ttu-id="07b6d-127">Перенаправление</span><span class="sxs-lookup"><span data-stu-id="07b6d-127">Forward</span></span>
    
- <span data-ttu-id="07b6d-128">нореспонсенецессари</span><span class="sxs-lookup"><span data-stu-id="07b6d-128">NoResponseNecessary</span></span>
    
- <span data-ttu-id="07b6d-129">Чтение</span><span class="sxs-lookup"><span data-stu-id="07b6d-129">Read</span></span>
    
- <span data-ttu-id="07b6d-130">Ответить</span><span class="sxs-lookup"><span data-stu-id="07b6d-130">Reply</span></span>
    
- <span data-ttu-id="07b6d-131">реплитоалл</span><span class="sxs-lookup"><span data-stu-id="07b6d-131">ReplyToAll</span></span>
    
- <span data-ttu-id="07b6d-132">Проверка</span><span class="sxs-lookup"><span data-stu-id="07b6d-132">Review</span></span>
    
## <a name="remarks"></a><span data-ttu-id="07b6d-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="07b6d-133">Remarks</span></span>

<span data-ttu-id="07b6d-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="07b6d-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07b6d-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="07b6d-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07b6d-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="07b6d-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="07b6d-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="07b6d-137">Schema Name</span></span>  <br/> |<span data-ttu-id="07b6d-138">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="07b6d-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="07b6d-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="07b6d-139">Validation File</span></span>  <br/> |<span data-ttu-id="07b6d-140">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="07b6d-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="07b6d-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="07b6d-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="07b6d-142">True</span><span class="sxs-lookup"><span data-stu-id="07b6d-142">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07b6d-143">См. также</span><span class="sxs-lookup"><span data-stu-id="07b6d-143">See also</span></span>



- [<span data-ttu-id="07b6d-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="07b6d-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

