---
title: монслиреженератион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MonthlyRegeneration
api_type:
- schema
ms.assetid: 9a52ca97-a663-41fe-b61a-61d8c53833ca
description: Элемент Монслиреженератион описывает частоту повторного создания задачи в месяцах.
ms.openlocfilehash: c941bc2606790646d2797df27c854996901c0bc6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462740"
---
# <a name="monthlyregeneration"></a><span data-ttu-id="f50a3-103">монслиреженератион</span><span class="sxs-lookup"><span data-stu-id="f50a3-103">MonthlyRegeneration</span></span>

<span data-ttu-id="f50a3-104">Элемент **монслиреженератион** описывает частоту повторного создания задачи в месяцах.</span><span class="sxs-lookup"><span data-stu-id="f50a3-104">The **MonthlyRegeneration** element describes the frequency, in months, of which task is regenerated.</span></span> 
  
```xml
<MonthlyRegeneration>
   <Interval/>
</MonthlyRegeneration>
```

 <span data-ttu-id="f50a3-105">**монслиреженератингпаттернтипе**</span><span class="sxs-lookup"><span data-stu-id="f50a3-105">**MonthlyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f50a3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f50a3-106">Attributes and elements</span></span>

<span data-ttu-id="f50a3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f50a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f50a3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f50a3-108">Attributes</span></span>

<span data-ttu-id="f50a3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f50a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f50a3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f50a3-110">Child elements</span></span>

|<span data-ttu-id="f50a3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f50a3-111">**Element**</span></span>|<span data-ttu-id="f50a3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f50a3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f50a3-113">Interval</span><span class="sxs-lookup"><span data-stu-id="f50a3-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="f50a3-114">Определяет интервал (в месяцах) между двумя последовательными повторяющимися элементами.</span><span class="sxs-lookup"><span data-stu-id="f50a3-114">Defines the interval, in months, between two consecutive recurring items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f50a3-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f50a3-115">Parent elements</span></span>

|<span data-ttu-id="f50a3-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f50a3-116">**Element**</span></span>|<span data-ttu-id="f50a3-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f50a3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f50a3-118">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="f50a3-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="f50a3-119">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="f50a3-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f50a3-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="f50a3-120">Remarks</span></span>

<span data-ttu-id="f50a3-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f50a3-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f50a3-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f50a3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f50a3-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f50a3-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f50a3-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f50a3-124">Schema name</span></span>  <br/> |<span data-ttu-id="f50a3-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f50a3-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="f50a3-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f50a3-126">Validation file</span></span>  <br/> |<span data-ttu-id="f50a3-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f50a3-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f50a3-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f50a3-128">Can be empty</span></span>  <br/> |<span data-ttu-id="f50a3-129">False</span><span class="sxs-lookup"><span data-stu-id="f50a3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f50a3-130">См. также</span><span class="sxs-lookup"><span data-stu-id="f50a3-130">See also</span></span>



- [<span data-ttu-id="f50a3-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f50a3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

