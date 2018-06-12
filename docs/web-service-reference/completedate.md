---
title: CompleteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: Элемент CompleteDate представляет дату, на котором был выполнен элемента.
ms.openlocfilehash: 00a1ec25be737ec0a5cc874063e1bce19a96cee0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761693"
---
# <a name="completedate"></a><span data-ttu-id="a37a9-103">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="a37a9-103">CompleteDate</span></span>

<span data-ttu-id="a37a9-104">Элемент **CompleteDate** представляет дату, на котором был выполнен элемента.</span><span class="sxs-lookup"><span data-stu-id="a37a9-104">The **CompleteDate** element represents the date on which an item was completed.</span></span> 
  
```xml
<CompleteDate/>
```

 <span data-ttu-id="a37a9-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="a37a9-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a37a9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a37a9-106">Attributes and elements</span></span>

<span data-ttu-id="a37a9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a37a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a37a9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a37a9-108">Attributes</span></span>

<span data-ttu-id="a37a9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a37a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a37a9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a37a9-110">Child elements</span></span>

<span data-ttu-id="a37a9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a37a9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a37a9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a37a9-112">Parent elements</span></span>

|<span data-ttu-id="a37a9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a37a9-113">**Element**</span></span>|<span data-ttu-id="a37a9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a37a9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a37a9-115">Задача</span><span class="sxs-lookup"><span data-stu-id="a37a9-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="a37a9-116">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a37a9-116">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a37a9-117">Флаг</span><span class="sxs-lookup"><span data-stu-id="a37a9-117">Flag</span></span>](flag.md) <br/> |<span data-ttu-id="a37a9-118">Задает флаг для элемента почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a37a9-118">Specifies a flag on a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a37a9-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a37a9-119">Text value</span></span>

<span data-ttu-id="a37a9-120">Текстовое значение, которое представляет дату и время является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="a37a9-120">A text value that represents the date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a37a9-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="a37a9-121">Remarks</span></span>

<span data-ttu-id="a37a9-122">Установка **CompleteDate** имеет тот же эффект, что и установка [PercentComplete](percentcomplete.md) [состояние](status.md) значение **завершено**или 100.</span><span class="sxs-lookup"><span data-stu-id="a37a9-122">Setting **CompleteDate** has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or [Status](status.md) to **Completed**.</span></span> <span data-ttu-id="a37a9-123">В запросе, что наборов по крайней мере два из этих свойств, последнего обработанного свойство определяет значение, заданное для этих элементов.</span><span class="sxs-lookup"><span data-stu-id="a37a9-123">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="a37a9-124">Например [PercentComplete](percentcomplete.md) равно 100, **CompleteDate** — 1 января 2007 г и имеет [состояние](status.md) **NotStarted**и свойства, передаваемых в указанном порядке, влияние нужно задать [состояние](status.md) задачи для **NotStarted **, [CompleteDate](completedate.md) **значение null**, а [PercentComplete](percentcomplete.md) 0.</span><span class="sxs-lookup"><span data-stu-id="a37a9-124">For example, if [PercentComplete](percentcomplete.md) is 100, **CompleteDate** is January 1, 2007, and [Status](status.md) is **NotStarted**, and the properties are streamed in that order, the effect will be to set the [Status](status.md) of the task to **NotStarted**, the [CompleteDate](completedate.md) to **null**, and [PercentComplete](percentcomplete.md) to 0.</span></span> 
  
<span data-ttu-id="a37a9-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a37a9-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a37a9-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a37a9-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a37a9-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a37a9-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a37a9-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a37a9-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a37a9-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a37a9-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="a37a9-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a37a9-130">Validation File</span></span>  <br/> |<span data-ttu-id="a37a9-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a37a9-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a37a9-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a37a9-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a37a9-133">False</span><span class="sxs-lookup"><span data-stu-id="a37a9-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a37a9-134">См. также</span><span class="sxs-lookup"><span data-stu-id="a37a9-134">See also</span></span>



- [<span data-ttu-id="a37a9-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a37a9-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a37a9-136">Создание задач</span><span class="sxs-lookup"><span data-stu-id="a37a9-136">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="a37a9-137">Удаление задачи</span><span class="sxs-lookup"><span data-stu-id="a37a9-137">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

