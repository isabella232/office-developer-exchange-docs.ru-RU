---
title: транситионсграуп
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TransitionsGroup
api_type:
- schema
ms.assetid: 19d56080-546a-4d53-929e-363d56186759
description: Элемент Транситионсграуп представляет массив переходов часового пояса.
ms.openlocfilehash: e5991ad7f73a1694e0d4abadd8d252acc04970e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840238"
---
# <a name="transitionsgroup"></a><span data-ttu-id="f753c-103">транситионсграуп</span><span class="sxs-lookup"><span data-stu-id="f753c-103">TransitionsGroup</span></span>

<span data-ttu-id="f753c-104">Элемент **транситионсграуп** представляет массив переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f753c-104">The **TransitionsGroup** element represents an array of time zone transitions.</span></span> 
  
```xml
<TransitionsGroup Id="">
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</TransitionsGroup>
```

 <span data-ttu-id="f753c-105">**аррайофтранситионстипе**</span><span class="sxs-lookup"><span data-stu-id="f753c-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f753c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f753c-106">Attributes and elements</span></span>

<span data-ttu-id="f753c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f753c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f753c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f753c-108">Attributes</span></span>

|<span data-ttu-id="f753c-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f753c-109">**Attribute**</span></span>|<span data-ttu-id="f753c-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f753c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f753c-111">Id</span><span class="sxs-lookup"><span data-stu-id="f753c-111">Id</span></span>  <br/> |<span data-ttu-id="f753c-112">Строковое значение, представляющее уникальный идентификатор группы переходов.</span><span class="sxs-lookup"><span data-stu-id="f753c-112">A string value that represents the unique identifier of the transitions group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f753c-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f753c-113">Child elements</span></span>

|<span data-ttu-id="f753c-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f753c-114">**Element**</span></span>|<span data-ttu-id="f753c-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f753c-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f753c-116">абсолутедатетранситион</span><span class="sxs-lookup"><span data-stu-id="f753c-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="f753c-117">Представляет переход часового пояса, который выполняется в определенный день и в определенное время.</span><span class="sxs-lookup"><span data-stu-id="f753c-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="f753c-118">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="f753c-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="f753c-119">Представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="f753c-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="f753c-120">рекуррингдатетранситион</span><span class="sxs-lookup"><span data-stu-id="f753c-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="f753c-121">Представляет переход часового пояса, который выполняется в указанный день года.</span><span class="sxs-lookup"><span data-stu-id="f753c-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f753c-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f753c-122">Parent elements</span></span>

|<span data-ttu-id="f753c-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f753c-123">**Element**</span></span>|<span data-ttu-id="f753c-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f753c-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f753c-125">транситионсграупс</span><span class="sxs-lookup"><span data-stu-id="f753c-125">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="f753c-126">Представляет массив групп смены часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="f753c-126">Represents an array of time zone transition groups.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f753c-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="f753c-127">Remarks</span></span>

<span data-ttu-id="f753c-128">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f753c-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f753c-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f753c-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f753c-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f753c-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f753c-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f753c-131">Schema Name</span></span>  <br/> |<span data-ttu-id="f753c-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f753c-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="f753c-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f753c-133">Validation File</span></span>  <br/> |<span data-ttu-id="f753c-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f753c-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f753c-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f753c-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="f753c-136">False</span><span class="sxs-lookup"><span data-stu-id="f753c-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f753c-137">См. также</span><span class="sxs-lookup"><span data-stu-id="f753c-137">See also</span></span>



- [<span data-ttu-id="f753c-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f753c-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

