---
title: IsMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: 6ce22f17-7a31-46c4-b643-0894d087e852
description: Элемент IsMeeting указывает, будет ли элемент календаря собрания или встречи.
ms.openlocfilehash: bb1349a8690450882e6beac0ccd84a8d03272a7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834051"
---
# <a name="ismeeting"></a><span data-ttu-id="e2756-103">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="e2756-103">IsMeeting</span></span>

<span data-ttu-id="e2756-104">Элемент **IsMeeting** указывает, будет ли элемент календаря собрания или встречи.</span><span class="sxs-lookup"><span data-stu-id="e2756-104">The **IsMeeting** element indicates whether the calendar item is a meeting or an appointment.</span></span> 
  
```xml
<IsMeeting/>
```

 <span data-ttu-id="e2756-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e2756-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2756-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e2756-106">Attributes and elements</span></span>

<span data-ttu-id="e2756-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e2756-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2756-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e2756-108">Attributes</span></span>

<span data-ttu-id="e2756-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e2756-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2756-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e2756-110">Child elements</span></span>

<span data-ttu-id="e2756-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e2756-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e2756-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e2756-112">Parent elements</span></span>

|<span data-ttu-id="e2756-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e2756-113">**Element**</span></span>|<span data-ttu-id="e2756-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e2756-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2756-115">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="e2756-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e2756-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2756-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e2756-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e2756-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e2756-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2756-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e2756-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e2756-119">Text value</span></span>

<span data-ttu-id="e2756-120">Текстовое значение, представляющее логическое значение является обязательным, если данный элемент включен.</span><span class="sxs-lookup"><span data-stu-id="e2756-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="e2756-121">Значение **true** указывает на то, что элемент календаря собрания.</span><span class="sxs-lookup"><span data-stu-id="e2756-121">A value of **true** indicates that the calendar item is a meeting.</span></span> <span data-ttu-id="e2756-122">Значение **false** указывает на то, что элемент календаря встречи.</span><span class="sxs-lookup"><span data-stu-id="e2756-122">A value of **false** indicates that the calendar item is an appointment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e2756-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="e2756-123">Remarks</span></span>

<span data-ttu-id="e2756-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e2756-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2756-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e2756-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2756-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e2756-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2756-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e2756-127">Schema name</span></span>  <br/> |<span data-ttu-id="e2756-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e2756-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2756-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e2756-129">Validation file</span></span>  <br/> |<span data-ttu-id="e2756-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e2756-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2756-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e2756-131">Can be empty</span></span>  <br/> |<span data-ttu-id="e2756-132">False</span><span class="sxs-lookup"><span data-stu-id="e2756-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2756-133">См. также</span><span class="sxs-lookup"><span data-stu-id="e2756-133">See also</span></span>



- [<span data-ttu-id="e2756-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e2756-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

