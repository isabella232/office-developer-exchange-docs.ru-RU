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
ms.openlocfilehash: 9f08dec048d410dadab9580e7886b2499d943176
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467419"
---
# <a name="transitionsgroup"></a><span data-ttu-id="62991-103">транситионсграуп</span><span class="sxs-lookup"><span data-stu-id="62991-103">TransitionsGroup</span></span>

<span data-ttu-id="62991-104">Элемент **транситионсграуп** представляет массив переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="62991-104">The **TransitionsGroup** element represents an array of time zone transitions.</span></span> 
  
```xml
<TransitionsGroup Id="">
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</TransitionsGroup>
```

 <span data-ttu-id="62991-105">**аррайофтранситионстипе**</span><span class="sxs-lookup"><span data-stu-id="62991-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="62991-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="62991-106">Attributes and elements</span></span>

<span data-ttu-id="62991-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="62991-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62991-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="62991-108">Attributes</span></span>

|<span data-ttu-id="62991-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="62991-109">**Attribute**</span></span>|<span data-ttu-id="62991-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62991-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="62991-111">Id</span><span class="sxs-lookup"><span data-stu-id="62991-111">Id</span></span>  <br/> |<span data-ttu-id="62991-112">Строковое значение, представляющее уникальный идентификатор группы переходов.</span><span class="sxs-lookup"><span data-stu-id="62991-112">A string value that represents the unique identifier of the transitions group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="62991-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="62991-113">Child elements</span></span>

|<span data-ttu-id="62991-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="62991-114">**Element**</span></span>|<span data-ttu-id="62991-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62991-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62991-116">абсолутедатетранситион</span><span class="sxs-lookup"><span data-stu-id="62991-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="62991-117">Представляет переход часового пояса, который выполняется в определенный день и в определенное время.</span><span class="sxs-lookup"><span data-stu-id="62991-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="62991-118">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="62991-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="62991-119">Представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="62991-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="62991-120">рекуррингдатетранситион</span><span class="sxs-lookup"><span data-stu-id="62991-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="62991-121">Представляет переход часового пояса, который выполняется в указанный день года.</span><span class="sxs-lookup"><span data-stu-id="62991-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="62991-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="62991-122">Parent elements</span></span>

|<span data-ttu-id="62991-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="62991-123">**Element**</span></span>|<span data-ttu-id="62991-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62991-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62991-125">транситионсграупс</span><span class="sxs-lookup"><span data-stu-id="62991-125">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="62991-126">Представляет массив групп смены часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="62991-126">Represents an array of time zone transition groups.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="62991-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="62991-127">Remarks</span></span>

<span data-ttu-id="62991-128">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="62991-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="62991-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="62991-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="62991-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="62991-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="62991-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="62991-131">Schema Name</span></span>  <br/> |<span data-ttu-id="62991-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="62991-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="62991-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="62991-133">Validation File</span></span>  <br/> |<span data-ttu-id="62991-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="62991-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="62991-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="62991-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="62991-136">False</span><span class="sxs-lookup"><span data-stu-id="62991-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="62991-137">См. также</span><span class="sxs-lookup"><span data-stu-id="62991-137">See also</span></span>



- [<span data-ttu-id="62991-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="62991-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

