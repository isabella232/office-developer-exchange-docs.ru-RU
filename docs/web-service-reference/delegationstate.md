---
title: DelegationState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegationState
api_type:
- schema
ms.assetid: 9dbb83ed-1ded-48f3-8e06-2489fc8b28d5
description: Элемент Делегатионстате представляет состояние делегированной задачи.
ms.openlocfilehash: b938b5a2240283c265006dd47cd6ff475ad80978
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457370"
---
# <a name="delegationstate"></a><span data-ttu-id="04d31-103">DelegationState</span><span class="sxs-lookup"><span data-stu-id="04d31-103">DelegationState</span></span>

<span data-ttu-id="04d31-104">Элемент **делегатионстате** представляет состояние делегированной задачи.</span><span class="sxs-lookup"><span data-stu-id="04d31-104">The **DelegationState** element represents the status of a delegated task.</span></span> 
  
```xml
<DelegationState/>
```

<span data-ttu-id="04d31-105">**таскделегатестатетипе**</span><span class="sxs-lookup"><span data-stu-id="04d31-105">**TaskDelegateStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="04d31-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="04d31-106">Attributes and elements</span></span>

<span data-ttu-id="04d31-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="04d31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04d31-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="04d31-108">Attributes</span></span>

<span data-ttu-id="04d31-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="04d31-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04d31-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="04d31-110">Child elements</span></span>

<span data-ttu-id="04d31-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="04d31-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04d31-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="04d31-112">Parent elements</span></span>

|<span data-ttu-id="04d31-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="04d31-113">**Element**</span></span>|<span data-ttu-id="04d31-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="04d31-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04d31-115">Задача</span><span class="sxs-lookup"><span data-stu-id="04d31-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="04d31-116">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="04d31-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04d31-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="04d31-117">Text value</span></span>

<span data-ttu-id="04d31-118">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04d31-118">This is a read-only property.</span></span> <span data-ttu-id="04d31-119">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="04d31-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="04d31-120">NoMatch</span><span class="sxs-lookup"><span data-stu-id="04d31-120">NoMatch</span></span>
    
- <span data-ttu-id="04d31-121">овннев</span><span class="sxs-lookup"><span data-stu-id="04d31-121">OwnNew</span></span>
    
- <span data-ttu-id="04d31-122">Он</span><span class="sxs-lookup"><span data-stu-id="04d31-122">Owned</span></span>
    
- <span data-ttu-id="04d31-123">Accepted</span><span class="sxs-lookup"><span data-stu-id="04d31-123">Accepted</span></span>
    
- <span data-ttu-id="04d31-124">Отклонено</span><span class="sxs-lookup"><span data-stu-id="04d31-124">Declined</span></span>
    
- <span data-ttu-id="04d31-125">Max</span><span class="sxs-lookup"><span data-stu-id="04d31-125">Max</span></span>
    
## <a name="remarks"></a><span data-ttu-id="04d31-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="04d31-126">Remarks</span></span>

<span data-ttu-id="04d31-127">Веб-службы Exchange в Microsoft Exchange Server 2007 не поддерживают назначения задач.</span><span class="sxs-lookup"><span data-stu-id="04d31-127">Exchange Web Services in Microsoft Exchange Server 2007 does not support task assignments.</span></span>
  
<span data-ttu-id="04d31-128">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Exchange 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="04d31-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04d31-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="04d31-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04d31-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="04d31-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04d31-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="04d31-131">Schema Name</span></span>  <br/> |<span data-ttu-id="04d31-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="04d31-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="04d31-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="04d31-133">Validation File</span></span>  <br/> |<span data-ttu-id="04d31-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="04d31-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04d31-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="04d31-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="04d31-136">False</span><span class="sxs-lookup"><span data-stu-id="04d31-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04d31-137">См. также</span><span class="sxs-lookup"><span data-stu-id="04d31-137">See also</span></span>

- [<span data-ttu-id="04d31-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="04d31-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

