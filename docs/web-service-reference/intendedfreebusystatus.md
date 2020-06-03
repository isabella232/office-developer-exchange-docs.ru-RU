---
title: интендедфрибусистатус
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
description: Элемент Интендедфрибусистатус представляет состояние, назначенное элементу календаря, связанному с приглашением на собрание.
ms.openlocfilehash: c5502bcfb308aa2f02a9575ab43f80261b5fa4ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465620"
---
# <a name="intendedfreebusystatus"></a><span data-ttu-id="a700c-103">интендедфрибусистатус</span><span class="sxs-lookup"><span data-stu-id="a700c-103">IntendedFreeBusyStatus</span></span>

<span data-ttu-id="a700c-104">Элемент **интендедфрибусистатус** представляет состояние, назначенное элементу календаря, связанному с приглашением на собрание.</span><span class="sxs-lookup"><span data-stu-id="a700c-104">The **IntendedFreeBusyStatus** element represents the intended status for the calendar item that is associated with the meeting request.</span></span> 
  
```xml
<IntendedFreeBusyStatus/>
```

 <span data-ttu-id="a700c-105">**легацифрибуситипе**</span><span class="sxs-lookup"><span data-stu-id="a700c-105">**LegacyFreeBusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a700c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a700c-106">Attributes and elements</span></span>

<span data-ttu-id="a700c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a700c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a700c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a700c-108">Attributes</span></span>

<span data-ttu-id="a700c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a700c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a700c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a700c-110">Child elements</span></span>

<span data-ttu-id="a700c-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a700c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a700c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a700c-112">Parent elements</span></span>

|<span data-ttu-id="a700c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a700c-113">**Element**</span></span>|<span data-ttu-id="a700c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a700c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a700c-115">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="a700c-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a700c-116">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a700c-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a700c-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a700c-117">Text value</span></span>

<span data-ttu-id="a700c-118">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="a700c-118">A text value is required.</span></span> <span data-ttu-id="a700c-119">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a700c-119">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="a700c-120">Свободна</span><span class="sxs-lookup"><span data-stu-id="a700c-120">Free</span></span>
    
- <span data-ttu-id="a700c-121">Занят</span><span class="sxs-lookup"><span data-stu-id="a700c-121">Tentative</span></span>
    
- <span data-ttu-id="a700c-122">Занята</span><span class="sxs-lookup"><span data-stu-id="a700c-122">Busy</span></span>
    
- <span data-ttu-id="a700c-123">OOF</span><span class="sxs-lookup"><span data-stu-id="a700c-123">OOF</span></span>
    
- <span data-ttu-id="a700c-124">NoData</span><span class="sxs-lookup"><span data-stu-id="a700c-124">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="a700c-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="a700c-125">Remarks</span></span>

<span data-ttu-id="a700c-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a700c-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a700c-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a700c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a700c-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a700c-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a700c-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a700c-129">Schema Name</span></span>  <br/> |<span data-ttu-id="a700c-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a700c-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="a700c-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a700c-131">Validation File</span></span>  <br/> |<span data-ttu-id="a700c-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a700c-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a700c-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a700c-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="a700c-134">False</span><span class="sxs-lookup"><span data-stu-id="a700c-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a700c-135">См. также</span><span class="sxs-lookup"><span data-stu-id="a700c-135">See also</span></span>



- [<span data-ttu-id="a700c-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a700c-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

