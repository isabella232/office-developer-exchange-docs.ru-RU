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
ms.openlocfilehash: 91922c4d6abd4d88ac9e36dd3d4c0224fc1ee716
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833992"
---
# <a name="isassignmenteditable"></a><span data-ttu-id="57362-103">исассигнментедитабле</span><span class="sxs-lookup"><span data-stu-id="57362-103">IsAssignmentEditable</span></span>

<span data-ttu-id="57362-104">Элемент **исассигнментедитабле** представляет тип задачи.</span><span class="sxs-lookup"><span data-stu-id="57362-104">The **IsAssignmentEditable** element represents the task type.</span></span> 
  
```xml
<IsAssignmentEditable/>
```

 <span data-ttu-id="57362-105">**положительн**</span><span class="sxs-lookup"><span data-stu-id="57362-105">**integer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57362-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="57362-106">Attributes and elements</span></span>

<span data-ttu-id="57362-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="57362-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57362-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="57362-108">Attributes</span></span>

<span data-ttu-id="57362-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="57362-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57362-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="57362-110">Child elements</span></span>

<span data-ttu-id="57362-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="57362-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57362-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="57362-112">Parent elements</span></span>

|<span data-ttu-id="57362-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57362-113">**Element**</span></span>|<span data-ttu-id="57362-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57362-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57362-115">Задача</span><span class="sxs-lookup"><span data-stu-id="57362-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="57362-116">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="57362-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57362-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="57362-117">Text value</span></span>

<span data-ttu-id="57362-118">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57362-118">This property is read-only.</span></span> <span data-ttu-id="57362-119">В приведенной ниже таблице перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="57362-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="57362-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="57362-120">**Value**</span></span>|<span data-ttu-id="57362-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57362-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="57362-122">нуль</span><span class="sxs-lookup"><span data-stu-id="57362-122">0</span></span>  <br/> |<span data-ttu-id="57362-123">Значение по умолчанию для всех элементов Task.</span><span class="sxs-lookup"><span data-stu-id="57362-123">The default for all task items.</span></span>  <br/> |
|<span data-ttu-id="57362-124">1,1</span><span class="sxs-lookup"><span data-stu-id="57362-124">1</span></span>  <br/> |<span data-ttu-id="57362-125">Запрос задачи.</span><span class="sxs-lookup"><span data-stu-id="57362-125">A task request.</span></span>  <br/> |
|<span data-ttu-id="57362-126">2</span><span class="sxs-lookup"><span data-stu-id="57362-126">2</span></span>  <br/> |<span data-ttu-id="57362-127">Принятие задачи от получателя запроса задачи.</span><span class="sxs-lookup"><span data-stu-id="57362-127">A task acceptance from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="57362-128">4</span><span class="sxs-lookup"><span data-stu-id="57362-128">3</span></span>  <br/> |<span data-ttu-id="57362-129">Отклонение задачи от получателя запроса задачи.</span><span class="sxs-lookup"><span data-stu-id="57362-129">A task declination from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="57362-130">4 </span><span class="sxs-lookup"><span data-stu-id="57362-130">4</span></span>  <br/> |<span data-ttu-id="57362-131">Обновление запроса на предыдущую задачу.</span><span class="sxs-lookup"><span data-stu-id="57362-131">An update to a previous task request.</span></span>  <br/> |
|<span data-ttu-id="57362-132">5 </span><span class="sxs-lookup"><span data-stu-id="57362-132">5</span></span>  <br/> |<span data-ttu-id="57362-133">Не используется.</span><span class="sxs-lookup"><span data-stu-id="57362-133">Not used.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="57362-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="57362-134">Remarks</span></span>

<span data-ttu-id="57362-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="57362-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57362-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="57362-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57362-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="57362-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57362-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="57362-138">Schema Name</span></span>  <br/> |<span data-ttu-id="57362-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="57362-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="57362-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="57362-140">Validation File</span></span>  <br/> |<span data-ttu-id="57362-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="57362-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57362-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="57362-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="57362-143">False</span><span class="sxs-lookup"><span data-stu-id="57362-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57362-144">См. также</span><span class="sxs-lookup"><span data-stu-id="57362-144">See also</span></span>



- [<span data-ttu-id="57362-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="57362-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

