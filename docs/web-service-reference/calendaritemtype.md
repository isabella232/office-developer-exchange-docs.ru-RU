---
title: календаритемтипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItemType
api_type:
- schema
ms.assetid: 1feb0788-adf7-4a7c-830c-005214ad930f
description: Элемент Календаритемтипе представляет тип элемента календаря.
ms.openlocfilehash: 05e93b6db3ae574c03f6e43c5ebec2288edec3e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527196"
---
# <a name="calendaritemtype"></a><span data-ttu-id="33929-103">календаритемтипе</span><span class="sxs-lookup"><span data-stu-id="33929-103">CalendarItemType</span></span>

<span data-ttu-id="33929-104">Элемент **календаритемтипе** представляет тип элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="33929-104">The **CalendarItemType** element represents the type of a calendar item.</span></span> 
  
```xml
<CalendarItemType/>
```

 <span data-ttu-id="33929-105">**календаритемтипетипе**</span><span class="sxs-lookup"><span data-stu-id="33929-105">**CalendarItemTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33929-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="33929-106">Attributes and elements</span></span>

<span data-ttu-id="33929-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="33929-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33929-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="33929-108">Attributes</span></span>

<span data-ttu-id="33929-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33929-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33929-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="33929-110">Child elements</span></span>

<span data-ttu-id="33929-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33929-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33929-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="33929-112">Parent elements</span></span>

|<span data-ttu-id="33929-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33929-113">**Element**</span></span>|<span data-ttu-id="33929-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33929-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33929-115">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="33929-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="33929-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="33929-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="33929-117">календаритем</span><span class="sxs-lookup"><span data-stu-id="33929-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="33929-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="33929-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33929-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="33929-119">Text value</span></span>

<span data-ttu-id="33929-120">При использовании этого элемента необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="33929-120">A text value is required if this element is used.</span></span> <span data-ttu-id="33929-121">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="33929-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="33929-122">**Один** Элемент не связан с повторяющимся элементом календаря.</span><span class="sxs-lookup"><span data-stu-id="33929-122">**Single** The item is not associated with a recurring calendar item.</span></span> 
    
- <span data-ttu-id="33929-123">**Экземпляр** Элемент является экземпляром повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="33929-123">**Occurrence** The item is an occurrence of a recurring calendar item.</span></span> 
    
- <span data-ttu-id="33929-124">**Exception (исключение** ) Элемент является исключением повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="33929-124">**Exception** The item is an exception to a recurring calendar item.</span></span> 
    
- <span data-ttu-id="33929-125">**Рекуррингмастер** Элемент является главным для набора повторяющихся элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="33929-125">**RecurringMaster** The item is master for a set of recurring calendar items.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="33929-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="33929-126">Remarks</span></span>

<span data-ttu-id="33929-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="33929-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33929-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="33929-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33929-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="33929-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33929-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="33929-130">Schema name</span></span>  <br/> |<span data-ttu-id="33929-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="33929-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="33929-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="33929-132">Validation file</span></span>  <br/> |<span data-ttu-id="33929-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="33929-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="33929-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="33929-134">Can be empty</span></span>  <br/> |<span data-ttu-id="33929-135">False</span><span class="sxs-lookup"><span data-stu-id="33929-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33929-136">См. также</span><span class="sxs-lookup"><span data-stu-id="33929-136">See also</span></span>



- [<span data-ttu-id="33929-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="33929-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

