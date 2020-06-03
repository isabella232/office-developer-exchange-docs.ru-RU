---
title: Когда
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- When
api_type:
- schema
ms.assetid: c7df1333-a33d-4cc6-a08a-34b68843f47d
description: Элемент When предоставляет сведения о том, когда встречается элемент "Календарь" или "собрание".
ms.openlocfilehash: 7c5f85184f966d909960bf1d79f5b8d33c67b51a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461858"
---
# <a name="when"></a><span data-ttu-id="94095-103">Когда</span><span class="sxs-lookup"><span data-stu-id="94095-103">When</span></span>

<span data-ttu-id="94095-104">Элемент **when** предоставляет сведения о том, когда встречается элемент "Календарь" или "собрание".</span><span class="sxs-lookup"><span data-stu-id="94095-104">The **When** element provides information about when a calendar or meeting item occurs.</span></span> 
  
```xml
<When/>
```

 <span data-ttu-id="94095-105">**String**</span><span class="sxs-lookup"><span data-stu-id="94095-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94095-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="94095-106">Attributes and elements</span></span>

<span data-ttu-id="94095-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="94095-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94095-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="94095-108">Attributes</span></span>

<span data-ttu-id="94095-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="94095-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94095-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="94095-110">Child elements</span></span>

<span data-ttu-id="94095-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="94095-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="94095-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="94095-112">Parent elements</span></span>

|<span data-ttu-id="94095-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="94095-113">**Element**</span></span>|<span data-ttu-id="94095-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="94095-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94095-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="94095-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="94095-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="94095-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="94095-117">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="94095-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="94095-118">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="94095-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="94095-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="94095-119">Text value</span></span>

<span data-ttu-id="94095-120">Текстовое значение — это строка, которая описывает, когда происходит элемент календаря.</span><span class="sxs-lookup"><span data-stu-id="94095-120">The text value is a string that describes when a calendar item occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="94095-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="94095-121">Remarks</span></span>

<span data-ttu-id="94095-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="94095-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94095-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="94095-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94095-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="94095-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94095-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="94095-125">Schema name</span></span>  <br/> |<span data-ttu-id="94095-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="94095-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="94095-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="94095-127">Validation file</span></span>  <br/> |<span data-ttu-id="94095-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="94095-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94095-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="94095-129">Can be empty</span></span>  <br/> |<span data-ttu-id="94095-130">False</span><span class="sxs-lookup"><span data-stu-id="94095-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94095-131">См. также</span><span class="sxs-lookup"><span data-stu-id="94095-131">See also</span></span>



- [<span data-ttu-id="94095-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="94095-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

