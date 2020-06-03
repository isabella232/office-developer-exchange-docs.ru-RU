---
title: Себя (Реминдерактионтипе)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: Элемент действия указывает действие, выполняемое с напоминанием.
ms.openlocfilehash: 5c62b2dd945b23a5ff2bb824385c45dbc617a5a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465060"
---
# <a name="actiontype-reminderactiontype"></a><span data-ttu-id="3451d-103">Себя (Реминдерактионтипе)</span><span class="sxs-lookup"><span data-stu-id="3451d-103">ActionType (ReminderActionType)</span></span>

<span data-ttu-id="3451d-104">Элемент **действия** указывает действие, выполняемое с напоминанием.</span><span class="sxs-lookup"><span data-stu-id="3451d-104">The **ActionType** element specifies the action to take on the reminder.</span></span> 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 <span data-ttu-id="3451d-105">**реминдерактионтипе**</span><span class="sxs-lookup"><span data-stu-id="3451d-105">**ReminderActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3451d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3451d-106">Attributes and elements</span></span>

<span data-ttu-id="3451d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3451d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3451d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3451d-108">Attributes</span></span>

<span data-ttu-id="3451d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3451d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3451d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3451d-110">Child elements</span></span>

<span data-ttu-id="3451d-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3451d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3451d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3451d-112">Parent elements</span></span>

[<span data-ttu-id="3451d-113">реминдеритемактион</span><span class="sxs-lookup"><span data-stu-id="3451d-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="3451d-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3451d-114">Text value</span></span>

<span data-ttu-id="3451d-115">Текстовое **значение элемента действия** указывает действие, выполняемое с напоминанием.</span><span class="sxs-lookup"><span data-stu-id="3451d-115">The text value of the **ActionType** element specifies the action to take on the reminder.</span></span> <span data-ttu-id="3451d-116">Текстовое значение **отклонения** указывает, что напоминание должно быть закрыто.</span><span class="sxs-lookup"><span data-stu-id="3451d-116">The text value of **Dismiss** indicates the reminder should be dismissed.</span></span> <span data-ttu-id="3451d-117">Текстовое значение **откладывания** указывает на то, что напоминание должно быть задержано до момента времени, указанного в элементе [невреминдертиме](newremindertime.md) .</span><span class="sxs-lookup"><span data-stu-id="3451d-117">The text value of **Snooze** indicates that the reminder should be delayed until the time specified by the [NewReminderTime](newremindertime.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3451d-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="3451d-118">Remarks</span></span>

<span data-ttu-id="3451d-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3451d-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3451d-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3451d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3451d-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3451d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3451d-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3451d-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3451d-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3451d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="3451d-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3451d-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="3451d-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3451d-125">Validation File</span></span>  <br/> |<span data-ttu-id="3451d-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3451d-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3451d-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3451d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="3451d-128">False</span><span class="sxs-lookup"><span data-stu-id="3451d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3451d-129">См. также</span><span class="sxs-lookup"><span data-stu-id="3451d-129">See also</span></span>

- [<span data-ttu-id="3451d-130">реминдеритемактион</span><span class="sxs-lookup"><span data-stu-id="3451d-130">ReminderItemAction</span></span>](reminderitemaction.md)
- [<span data-ttu-id="3451d-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3451d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

