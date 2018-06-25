---
title: Ресурсы
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Resources
api_type:
- schema
ms.assetid: a2133cf2-7c62-4f1c-b3aa-75f14d30dd74
description: Элемент Resources запланированного ресурс для собрания.
ms.openlocfilehash: 31f358414e53f55b983f7633fc9c67b0ce3ab645
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835166"
---
# <a name="resources"></a><span data-ttu-id="f553d-103">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="f553d-103">Resources</span></span>

<span data-ttu-id="f553d-104">Элемент **Resources** запланированного ресурс для собрания.</span><span class="sxs-lookup"><span data-stu-id="f553d-104">The **Resources** element represents a scheduled resource for a meeting.</span></span> 
  
```xml
<Resources>
   <Attendee/>
</Resources>
```

 <span data-ttu-id="f553d-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="f553d-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f553d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f553d-106">Attributes and elements</span></span>

<span data-ttu-id="f553d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f553d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f553d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f553d-108">Attributes</span></span>

<span data-ttu-id="f553d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f553d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f553d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f553d-110">Child elements</span></span>

|<span data-ttu-id="f553d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f553d-111">**Element**</span></span>|<span data-ttu-id="f553d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f553d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f553d-113">Attendee</span><span class="sxs-lookup"><span data-stu-id="f553d-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="f553d-114">Представляет участников и ресурсы, необходимые для собрания.</span><span class="sxs-lookup"><span data-stu-id="f553d-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f553d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f553d-115">Parent elements</span></span>

|<span data-ttu-id="f553d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f553d-116">**Element**</span></span>|<span data-ttu-id="f553d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f553d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f553d-118">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="f553d-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f553d-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="f553d-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f553d-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f553d-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f553d-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f553d-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f553d-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="f553d-122">Remarks</span></span>

<span data-ttu-id="f553d-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f553d-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f553d-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f553d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f553d-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f553d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f553d-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f553d-126">Schema name</span></span>  <br/> |<span data-ttu-id="f553d-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f553d-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="f553d-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f553d-128">Validation file</span></span>  <br/> |<span data-ttu-id="f553d-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f553d-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f553d-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f553d-130">Can be empty</span></span>  <br/> |<span data-ttu-id="f553d-131">False</span><span class="sxs-lookup"><span data-stu-id="f553d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f553d-132">См. также</span><span class="sxs-lookup"><span data-stu-id="f553d-132">See also</span></span>



- [<span data-ttu-id="f553d-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f553d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

