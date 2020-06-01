---
title: исассигнментедитабле
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAssignmentEditable
api_type:
- schema
ms.assetid: 0ddf9181-f65e-4ad6-ad69-7b074ea0f2e7
description: Элемент Исассигнментедитабле представляет тип задачи.
ms.openlocfilehash: 5eb091b24e2c97f7aa6072044fed998b6c9c1651
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468056"
---
# <a name="isassignmenteditable"></a><span data-ttu-id="d1fd4-103">исассигнментедитабле</span><span class="sxs-lookup"><span data-stu-id="d1fd4-103">IsAssignmentEditable</span></span>

<span data-ttu-id="d1fd4-104">Элемент **исассигнментедитабле** представляет тип задачи.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-104">The **IsAssignmentEditable** element represents the task type.</span></span> 
  
```xml
<IsAssignmentEditable/>
```

 <span data-ttu-id="d1fd4-105">**положительн**</span><span class="sxs-lookup"><span data-stu-id="d1fd4-105">**integer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1fd4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d1fd4-106">Attributes and elements</span></span>

<span data-ttu-id="d1fd4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1fd4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d1fd4-108">Attributes</span></span>

<span data-ttu-id="d1fd4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1fd4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d1fd4-110">Child elements</span></span>

<span data-ttu-id="d1fd4-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1fd4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d1fd4-112">Parent elements</span></span>

|<span data-ttu-id="d1fd4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d1fd4-113">**Element**</span></span>|<span data-ttu-id="d1fd4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d1fd4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1fd4-115">Задача</span><span class="sxs-lookup"><span data-stu-id="d1fd4-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="d1fd4-116">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d1fd4-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d1fd4-117">Text value</span></span>

<span data-ttu-id="d1fd4-118">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-118">This property is read-only.</span></span> <span data-ttu-id="d1fd4-119">В приведенной ниже таблице перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="d1fd4-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d1fd4-120">**Value**</span></span>|<span data-ttu-id="d1fd4-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d1fd4-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d1fd4-122">нуль</span><span class="sxs-lookup"><span data-stu-id="d1fd4-122">0</span></span>  <br/> |<span data-ttu-id="d1fd4-123">Значение по умолчанию для всех элементов Task.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-123">The default for all task items.</span></span>  <br/> |
|<span data-ttu-id="d1fd4-124">1 </span><span class="sxs-lookup"><span data-stu-id="d1fd4-124">1</span></span>  <br/> |<span data-ttu-id="d1fd4-125">Запрос задачи.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-125">A task request.</span></span>  <br/> |
|<span data-ttu-id="d1fd4-126">2</span><span class="sxs-lookup"><span data-stu-id="d1fd4-126">2</span></span>  <br/> |<span data-ttu-id="d1fd4-127">Принятие задачи от получателя запроса задачи.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-127">A task acceptance from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="d1fd4-128">4</span><span class="sxs-lookup"><span data-stu-id="d1fd4-128">3</span></span>  <br/> |<span data-ttu-id="d1fd4-129">Отклонение задачи от получателя запроса задачи.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-129">A task declination from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="d1fd4-130">4 </span><span class="sxs-lookup"><span data-stu-id="d1fd4-130">4</span></span>  <br/> |<span data-ttu-id="d1fd4-131">Обновление запроса на предыдущую задачу.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-131">An update to a previous task request.</span></span>  <br/> |
|<span data-ttu-id="d1fd4-132">5 </span><span class="sxs-lookup"><span data-stu-id="d1fd4-132">5</span></span>  <br/> |<span data-ttu-id="d1fd4-133">Не используется.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-133">Not used.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d1fd4-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="d1fd4-134">Remarks</span></span>

<span data-ttu-id="d1fd4-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d1fd4-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1fd4-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d1fd4-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1fd4-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d1fd4-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1fd4-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d1fd4-138">Schema Name</span></span>  <br/> |<span data-ttu-id="d1fd4-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d1fd4-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="d1fd4-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d1fd4-140">Validation File</span></span>  <br/> |<span data-ttu-id="d1fd4-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d1fd4-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1fd4-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d1fd4-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1fd4-143">False</span><span class="sxs-lookup"><span data-stu-id="d1fd4-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1fd4-144">См. также</span><span class="sxs-lookup"><span data-stu-id="d1fd4-144">See also</span></span>



- [<span data-ttu-id="d1fd4-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d1fd4-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

