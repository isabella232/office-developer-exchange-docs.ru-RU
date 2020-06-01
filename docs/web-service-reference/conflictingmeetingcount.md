---
title: конфликтингмитингкаунт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: Элемент Конфликтингмитингкаунт представляет количество собраний, которые конфликтуют с элементом календаря.
ms.openlocfilehash: d53245e1b5d1f0182b28b15bf55ba9742bbb2a07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463862"
---
# <a name="conflictingmeetingcount"></a><span data-ttu-id="53848-103">конфликтингмитингкаунт</span><span class="sxs-lookup"><span data-stu-id="53848-103">ConflictingMeetingCount</span></span>

<span data-ttu-id="53848-104">Элемент **конфликтингмитингкаунт** представляет количество собраний, которые конфликтуют с элементом календаря.</span><span class="sxs-lookup"><span data-stu-id="53848-104">The **ConflictingMeetingCount** element represents the number of meetings that conflict with the calendar item.</span></span> 
  
```xml
<ConflictingMeetingCount/>
```

 <span data-ttu-id="53848-105">**int**</span><span class="sxs-lookup"><span data-stu-id="53848-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53848-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="53848-106">Attributes and elements</span></span>

<span data-ttu-id="53848-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="53848-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53848-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="53848-108">Attributes</span></span>

<span data-ttu-id="53848-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="53848-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53848-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="53848-110">Child elements</span></span>

<span data-ttu-id="53848-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="53848-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="53848-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="53848-112">Parent elements</span></span>

|<span data-ttu-id="53848-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="53848-113">**Element**</span></span>|<span data-ttu-id="53848-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="53848-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53848-115">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="53848-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="53848-116">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="53848-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="53848-117">календаритем</span><span class="sxs-lookup"><span data-stu-id="53848-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="53848-118">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="53848-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="53848-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="53848-119">Text value</span></span>

<span data-ttu-id="53848-120">Текстовое значение представляет целое число.</span><span class="sxs-lookup"><span data-stu-id="53848-120">The text value represents an integer.</span></span> <span data-ttu-id="53848-121">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53848-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="53848-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="53848-122">Remarks</span></span>

<span data-ttu-id="53848-123">Элемент календаря считается конфликтующим, если он происходит, по крайней мере, частично, в то же время, что и другой элемент календаря в той же папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="53848-123">A calendar item is considered conflicting if it occurs, at least in part, at the same time as another calendar item in the same calendar folder.</span></span> <span data-ttu-id="53848-124">Если элемент календаря находится в папке "некалендарный", он сравнивается с элементами календаря в папке "Календарь" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="53848-124">If a calendar item is in a noncalendar folder, it is compared with calendar items in the default calendar folder.</span></span> <span data-ttu-id="53848-125">Приглашения на собрания сравниваются с элементами календаря в папке "Календарь" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="53848-125">Meeting requests are compared with calendar items in the default calendar folder.</span></span>
  
<span data-ttu-id="53848-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="53848-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53848-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="53848-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53848-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="53848-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="53848-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="53848-129">Schema name</span></span>  <br/> |<span data-ttu-id="53848-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="53848-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="53848-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="53848-131">Validation file</span></span>  <br/> |<span data-ttu-id="53848-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="53848-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="53848-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="53848-133">Can be empty</span></span>  <br/> |<span data-ttu-id="53848-134">False</span><span class="sxs-lookup"><span data-stu-id="53848-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="53848-135">См. также</span><span class="sxs-lookup"><span data-stu-id="53848-135">See also</span></span>



- [<span data-ttu-id="53848-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="53848-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

