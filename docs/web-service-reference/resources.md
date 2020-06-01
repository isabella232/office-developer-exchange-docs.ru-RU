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
description: Элемент Resources представляет запланированный ресурс для собрания.
ms.openlocfilehash: 67b4ed93a67a48945845887aa2d08b5bfe0102d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455592"
---
# <a name="resources"></a><span data-ttu-id="ab79c-103">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="ab79c-103">Resources</span></span>

<span data-ttu-id="ab79c-104">Элемент **Resources** представляет запланированный ресурс для собрания.</span><span class="sxs-lookup"><span data-stu-id="ab79c-104">The **Resources** element represents a scheduled resource for a meeting.</span></span> 
  
```xml
<Resources>
   <Attendee/>
</Resources>
```

 <span data-ttu-id="ab79c-105">**нонемптяррайофаттендистипе**</span><span class="sxs-lookup"><span data-stu-id="ab79c-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab79c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ab79c-106">Attributes and elements</span></span>

<span data-ttu-id="ab79c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ab79c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab79c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ab79c-108">Attributes</span></span>

<span data-ttu-id="ab79c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ab79c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ab79c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ab79c-110">Child elements</span></span>

|<span data-ttu-id="ab79c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ab79c-111">**Element**</span></span>|<span data-ttu-id="ab79c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ab79c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ab79c-113">Участник</span><span class="sxs-lookup"><span data-stu-id="ab79c-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="ab79c-114">Представляет участников и ресурсы собрания.</span><span class="sxs-lookup"><span data-stu-id="ab79c-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ab79c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ab79c-115">Parent elements</span></span>

|<span data-ttu-id="ab79c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ab79c-116">**Element**</span></span>|<span data-ttu-id="ab79c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ab79c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ab79c-118">календаритем</span><span class="sxs-lookup"><span data-stu-id="ab79c-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ab79c-119">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab79c-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ab79c-120">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="ab79c-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ab79c-121">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab79c-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ab79c-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="ab79c-122">Remarks</span></span>

<span data-ttu-id="ab79c-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ab79c-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab79c-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ab79c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab79c-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ab79c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ab79c-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ab79c-126">Schema name</span></span>  <br/> |<span data-ttu-id="ab79c-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ab79c-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="ab79c-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ab79c-128">Validation file</span></span>  <br/> |<span data-ttu-id="ab79c-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ab79c-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ab79c-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ab79c-130">Can be empty</span></span>  <br/> |<span data-ttu-id="ab79c-131">False</span><span class="sxs-lookup"><span data-stu-id="ab79c-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ab79c-132">См. также</span><span class="sxs-lookup"><span data-stu-id="ab79c-132">See also</span></span>



- [<span data-ttu-id="ab79c-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ab79c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

