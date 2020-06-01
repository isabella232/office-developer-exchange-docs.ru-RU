---
title: еарлиреженератион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- YearlyRegeneration
api_type:
- schema
ms.assetid: 23538bca-738e-4319-944e-f459ff8a7eba
description: Элемент Еарлиреженератион описывает частоту повторного создания задачи (в годах).
ms.openlocfilehash: 7a6796c433bc54d145d5a769e01f9bba46897735
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457881"
---
# <a name="yearlyregeneration"></a><span data-ttu-id="5e2e9-103">еарлиреженератион</span><span class="sxs-lookup"><span data-stu-id="5e2e9-103">YearlyRegeneration</span></span>

<span data-ttu-id="5e2e9-104">Элемент **еарлиреженератион** описывает частоту повторного создания задачи (в годах).</span><span class="sxs-lookup"><span data-stu-id="5e2e9-104">The **YearlyRegeneration** element describes the frequency, in years, in which a task is regenerated.</span></span> 
  
```xml
<YearlyRegeneratingPatternType>
   <Interval/>
</YearlyRegeneratingPatternType>
```

<span data-ttu-id="5e2e9-105">**еарлиреженератингпаттернтипе**</span><span class="sxs-lookup"><span data-stu-id="5e2e9-105">**YearlyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5e2e9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5e2e9-106">Attributes and elements</span></span>

<span data-ttu-id="5e2e9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5e2e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e2e9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5e2e9-108">Attributes</span></span>

<span data-ttu-id="5e2e9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5e2e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e2e9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5e2e9-110">Child elements</span></span>

|<span data-ttu-id="5e2e9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5e2e9-111">**Element**</span></span>|<span data-ttu-id="5e2e9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e2e9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e2e9-113">Interval</span><span class="sxs-lookup"><span data-stu-id="5e2e9-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="5e2e9-114">Определяет интервал (в годах), в течение которого новая задача воссоздается после завершения задачи.</span><span class="sxs-lookup"><span data-stu-id="5e2e9-114">Defines the interval, in years, during which a new task is regenerated after the completion of the task.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5e2e9-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5e2e9-115">Parent elements</span></span>

|<span data-ttu-id="5e2e9-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5e2e9-116">**Element**</span></span>|<span data-ttu-id="5e2e9-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e2e9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e2e9-118">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="5e2e9-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="5e2e9-119">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="5e2e9-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5e2e9-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="5e2e9-120">Remarks</span></span>

<span data-ttu-id="5e2e9-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5e2e9-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5e2e9-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5e2e9-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e2e9-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5e2e9-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5e2e9-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5e2e9-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5e2e9-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5e2e9-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="5e2e9-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5e2e9-126">Validation File</span></span>  <br/> |<span data-ttu-id="5e2e9-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5e2e9-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5e2e9-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5e2e9-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e2e9-129">False</span><span class="sxs-lookup"><span data-stu-id="5e2e9-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e2e9-130">См. также</span><span class="sxs-lookup"><span data-stu-id="5e2e9-130">See also</span></span>

- [<span data-ttu-id="5e2e9-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5e2e9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

