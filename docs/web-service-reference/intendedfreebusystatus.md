---
title: IntendedFreeBusyStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IntendedFreeBusyStatus
api_type:
- schema
ms.assetid: 0e0fa898-69a4-4c57-8bb2-52f716b5b478
description: Элемент IntendedFreeBusyStatus представляет предполагаемая состояния для элемента календаря, который связан с приглашения на собрание.
ms.openlocfilehash: 3254becf8c6885f7d6dc401ecf31da149e7de2d4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833945"
---
# <a name="intendedfreebusystatus"></a><span data-ttu-id="2463c-103">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="2463c-103">IntendedFreeBusyStatus</span></span>

<span data-ttu-id="2463c-104">Элемент **IntendedFreeBusyStatus** представляет предполагаемая состояния для элемента календаря, который связан с приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="2463c-104">The **IntendedFreeBusyStatus** element represents the intended status for the calendar item that is associated with the meeting request.</span></span> 
  
```xml
<IntendedFreeBusyStatus/>
```

 <span data-ttu-id="2463c-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="2463c-105">**LegacyFreeBusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2463c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2463c-106">Attributes and elements</span></span>

<span data-ttu-id="2463c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2463c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2463c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2463c-108">Attributes</span></span>

<span data-ttu-id="2463c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2463c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2463c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2463c-110">Child elements</span></span>

<span data-ttu-id="2463c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2463c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2463c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2463c-112">Parent elements</span></span>

|<span data-ttu-id="2463c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2463c-113">**Element**</span></span>|<span data-ttu-id="2463c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2463c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2463c-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2463c-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2463c-116">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2463c-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2463c-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2463c-117">Text value</span></span>

<span data-ttu-id="2463c-118">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="2463c-118">A text value is required.</span></span> <span data-ttu-id="2463c-119">Ниже приведены возможные значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="2463c-119">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="2463c-120">Свободна</span><span class="sxs-lookup"><span data-stu-id="2463c-120">Free</span></span>
    
- <span data-ttu-id="2463c-121">Под вопросом</span><span class="sxs-lookup"><span data-stu-id="2463c-121">Tentative</span></span>
    
- <span data-ttu-id="2463c-122">Занята</span><span class="sxs-lookup"><span data-stu-id="2463c-122">Busy</span></span>
    
- <span data-ttu-id="2463c-123">ОБ ОТСУТСТВИИ НА РАБОТЕ</span><span class="sxs-lookup"><span data-stu-id="2463c-123">OOF</span></span>
    
- <span data-ttu-id="2463c-124">NoData</span><span class="sxs-lookup"><span data-stu-id="2463c-124">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="2463c-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="2463c-125">Remarks</span></span>

<span data-ttu-id="2463c-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2463c-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2463c-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2463c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2463c-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2463c-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2463c-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2463c-129">Schema Name</span></span>  <br/> |<span data-ttu-id="2463c-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2463c-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="2463c-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2463c-131">Validation File</span></span>  <br/> |<span data-ttu-id="2463c-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2463c-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2463c-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2463c-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="2463c-134">False</span><span class="sxs-lookup"><span data-stu-id="2463c-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2463c-135">См. также</span><span class="sxs-lookup"><span data-stu-id="2463c-135">See also</span></span>



- [<span data-ttu-id="2463c-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2463c-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

