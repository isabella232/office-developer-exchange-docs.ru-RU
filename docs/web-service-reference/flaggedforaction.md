---
title: FlaggedForAction
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
description: Элемент FlaggedForAction указывает флаг, для которого действию задано значение, которое должно отображаться для входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 5b6e714512edcf12ded2c04f414d047b8622d305
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762613"
---
# <a name="flaggedforaction"></a><span data-ttu-id="f1bc5-103">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="f1bc5-103">FlaggedForAction</span></span>

<span data-ttu-id="f1bc5-104">Элемент **FlaggedForAction** указывает флаг, для которого действию задано значение, которое должно отображаться для входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="f1bc5-104">The **FlaggedForAction** element specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<FlaggedForAction/>
```

 <span data-ttu-id="f1bc5-105">**FlaggedForActionType**</span><span class="sxs-lookup"><span data-stu-id="f1bc5-105">**FlaggedForActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1bc5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f1bc5-106">Attributes and elements</span></span>

<span data-ttu-id="f1bc5-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f1bc5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1bc5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f1bc5-108">Attributes</span></span>

<span data-ttu-id="f1bc5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1bc5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1bc5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f1bc5-110">Child elements</span></span>

<span data-ttu-id="f1bc5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1bc5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f1bc5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f1bc5-112">Parent elements</span></span>

|<span data-ttu-id="f1bc5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1bc5-113">**Element**</span></span>|<span data-ttu-id="f1bc5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1bc5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1bc5-115">Условия</span><span class="sxs-lookup"><span data-stu-id="f1bc5-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="f1bc5-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="f1bc5-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="f1bc5-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="f1bc5-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="f1bc5-118">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="f1bc5-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f1bc5-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f1bc5-119">Text value</span></span>

<span data-ttu-id="f1bc5-120">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="f1bc5-120">A text value is required.</span></span> <span data-ttu-id="f1bc5-121">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="f1bc5-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="f1bc5-122">Любой</span><span class="sxs-lookup"><span data-stu-id="f1bc5-122">Any</span></span>
    
- <span data-ttu-id="f1bc5-123">Звонок</span><span class="sxs-lookup"><span data-stu-id="f1bc5-123">Call</span></span>
    
- <span data-ttu-id="f1bc5-124">DoNotForward</span><span class="sxs-lookup"><span data-stu-id="f1bc5-124">DoNotForward</span></span>
    
- <span data-ttu-id="f1bc5-125">Последующего действия</span><span class="sxs-lookup"><span data-stu-id="f1bc5-125">FollowUp</span></span>
    
- <span data-ttu-id="f1bc5-126">FYI</span><span class="sxs-lookup"><span data-stu-id="f1bc5-126">FYI</span></span>
    
- <span data-ttu-id="f1bc5-127">Переслать</span><span class="sxs-lookup"><span data-stu-id="f1bc5-127">Forward</span></span>
    
- <span data-ttu-id="f1bc5-128">NoResponseNecessary</span><span class="sxs-lookup"><span data-stu-id="f1bc5-128">NoResponseNecessary</span></span>
    
- <span data-ttu-id="f1bc5-129">Чтение</span><span class="sxs-lookup"><span data-stu-id="f1bc5-129">Read</span></span>
    
- <span data-ttu-id="f1bc5-130">Ответить</span><span class="sxs-lookup"><span data-stu-id="f1bc5-130">Reply</span></span>
    
- <span data-ttu-id="f1bc5-131">ReplyToAll</span><span class="sxs-lookup"><span data-stu-id="f1bc5-131">ReplyToAll</span></span>
    
- <span data-ttu-id="f1bc5-132">Просмотр</span><span class="sxs-lookup"><span data-stu-id="f1bc5-132">Review</span></span>
    
## <a name="remarks"></a><span data-ttu-id="f1bc5-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="f1bc5-133">Remarks</span></span>

<span data-ttu-id="f1bc5-134">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1bc5-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1bc5-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f1bc5-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1bc5-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f1bc5-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f1bc5-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f1bc5-137">Schema Name</span></span>  <br/> |<span data-ttu-id="f1bc5-138">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f1bc5-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f1bc5-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f1bc5-139">Validation File</span></span>  <br/> |<span data-ttu-id="f1bc5-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f1bc5-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f1bc5-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f1bc5-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1bc5-142">True</span><span class="sxs-lookup"><span data-stu-id="f1bc5-142">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1bc5-143">См. также</span><span class="sxs-lookup"><span data-stu-id="f1bc5-143">See also</span></span>



- [<span data-ttu-id="f1bc5-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f1bc5-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

