---
title: абсолутедатетранситион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteDateTransition
api_type:
- schema
ms.assetid: 8f5731eb-bed0-45bf-ba89-4aaf20c34a39
description: Элемент Абсолутедатетранситион представляет переход часового пояса, который выполняется в определенный день и в определенное время.
ms.openlocfilehash: 514464f69c3be5496aedbe184848ef9ed9f296b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461725"
---
# <a name="absolutedatetransition"></a><span data-ttu-id="6c908-103">абсолутедатетранситион</span><span class="sxs-lookup"><span data-stu-id="6c908-103">AbsoluteDateTransition</span></span>

<span data-ttu-id="6c908-104">Элемент **абсолутедатетранситион** представляет переход часового пояса, который выполняется в определенный день и в определенное время.</span><span class="sxs-lookup"><span data-stu-id="6c908-104">The **AbsoluteDateTransition** element represents a time zone transition that occurs on a specific date and at a specific time.</span></span> 
  
```xml
<AbsoluteDateTransition>
   <To/>
   <DateTime/>
</AbsoluteDateTransition>
```

<span data-ttu-id="6c908-105">**абсолутедатетранситионтипе**</span><span class="sxs-lookup"><span data-stu-id="6c908-105">**AbsoluteDateTransitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6c908-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6c908-106">Attributes and elements</span></span>

<span data-ttu-id="6c908-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6c908-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c908-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6c908-108">Attributes</span></span>

<span data-ttu-id="6c908-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6c908-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c908-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6c908-110">Child elements</span></span>

|<span data-ttu-id="6c908-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6c908-111">**Element**</span></span>|<span data-ttu-id="6c908-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6c908-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c908-113">To</span><span class="sxs-lookup"><span data-stu-id="6c908-113">To</span></span>](to.md) <br/> |<span data-ttu-id="6c908-114">Указывает [период](period.md) или [транситионсграуп](transitionsgroup.md) , который является целевым объектом перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="6c908-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="6c908-115">DateTime</span><span class="sxs-lookup"><span data-stu-id="6c908-115">DateTime</span></span>](datetime.md) <br/> |<span data-ttu-id="6c908-116">Представляет дату и время, когда происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="6c908-116">Represents the date and time at which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6c908-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6c908-117">Parent elements</span></span>

|<span data-ttu-id="6c908-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6c908-118">**Element**</span></span>|<span data-ttu-id="6c908-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6c908-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c908-120">Выполняет</span><span class="sxs-lookup"><span data-stu-id="6c908-120">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="6c908-121">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="6c908-121">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="6c908-122">транситионсграуп</span><span class="sxs-lookup"><span data-stu-id="6c908-122">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="6c908-123">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="6c908-123">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6c908-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="6c908-124">Remarks</span></span>

<span data-ttu-id="6c908-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6c908-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c908-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6c908-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c908-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6c908-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c908-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6c908-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6c908-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6c908-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c908-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6c908-130">Validation File</span></span>  <br/> |<span data-ttu-id="6c908-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6c908-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c908-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6c908-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c908-133">False</span><span class="sxs-lookup"><span data-stu-id="6c908-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c908-134">См. также</span><span class="sxs-lookup"><span data-stu-id="6c908-134">See also</span></span>

- [<span data-ttu-id="6c908-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6c908-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

