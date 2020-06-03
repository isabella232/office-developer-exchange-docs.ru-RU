---
title: Month (переход часового пояса)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: 5e6aac75-366d-43d0-8ccb-956285474662
description: Элемент month представляет месяц, в котором происходит переход часового пояса.
ms.openlocfilehash: 1fa32ea355cc3fe826f9c34b2fd147a0d8201673
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467741"
---
# <a name="month-time-zone-transition"></a><span data-ttu-id="a8ae3-103">Month (переход часового пояса)</span><span class="sxs-lookup"><span data-stu-id="a8ae3-103">Month (Time Zone Transition)</span></span>

<span data-ttu-id="a8ae3-104">Элемент **Month** представляет месяц, в котором происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a8ae3-104">The **Month** element represents the month in which the time zone transition occurs.</span></span> 
  
```xml
<Month/>
```

 <span data-ttu-id="a8ae3-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a8ae3-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8ae3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a8ae3-106">Attributes and elements</span></span>

<span data-ttu-id="a8ae3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a8ae3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8ae3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a8ae3-108">Attributes</span></span>

<span data-ttu-id="a8ae3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a8ae3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8ae3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a8ae3-110">Child elements</span></span>

<span data-ttu-id="a8ae3-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a8ae3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8ae3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a8ae3-112">Parent elements</span></span>

|<span data-ttu-id="a8ae3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a8ae3-113">**Element**</span></span>|<span data-ttu-id="a8ae3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a8ae3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8ae3-115">рекуррингдатетранситион</span><span class="sxs-lookup"><span data-stu-id="a8ae3-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="a8ae3-116">Представляет переход часового пояса, который выполняется в определенный день каждого года.</span><span class="sxs-lookup"><span data-stu-id="a8ae3-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="a8ae3-117">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="a8ae3-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="a8ae3-118">Представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="a8ae3-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8ae3-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a8ae3-119">Text value</span></span>

<span data-ttu-id="a8ae3-120">Текстовое значение — это целое число, представляющее месяц, в котором происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a8ae3-120">The text value is an integer that represents the month in which the time zone transition occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8ae3-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="a8ae3-121">Remarks</span></span>

<span data-ttu-id="a8ae3-122">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a8ae3-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8ae3-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a8ae3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8ae3-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a8ae3-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8ae3-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a8ae3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a8ae3-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a8ae3-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8ae3-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a8ae3-127">Validation File</span></span>  <br/> |<span data-ttu-id="a8ae3-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a8ae3-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8ae3-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a8ae3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8ae3-130">False</span><span class="sxs-lookup"><span data-stu-id="a8ae3-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8ae3-131">См. также</span><span class="sxs-lookup"><span data-stu-id="a8ae3-131">See also</span></span>



- [<span data-ttu-id="a8ae3-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a8ae3-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

