---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: Элемент MeetingRequestType описывает тип запроса на проведение собрания.
ms.openlocfilehash: 7269587e2fa72aeb9070a7b53ee9215829729329
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834432"
---
# <a name="meetingrequesttype"></a><span data-ttu-id="1a2cc-103">MeetingRequestType</span><span class="sxs-lookup"><span data-stu-id="1a2cc-103">MeetingRequestType</span></span>

<span data-ttu-id="1a2cc-104">Элемент **MeetingRequestType** описывает тип запроса на проведение собрания.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-104">The **MeetingRequestType** element describes the type of the meeting request.</span></span> 
  
```xml
<MeetingRequestType/>
```

 <span data-ttu-id="1a2cc-105">**MeetingRequestTypeType**</span><span class="sxs-lookup"><span data-stu-id="1a2cc-105">**MeetingRequestTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a2cc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1a2cc-106">Attributes and elements</span></span>

<span data-ttu-id="1a2cc-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a2cc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1a2cc-108">Attributes</span></span>

<span data-ttu-id="1a2cc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a2cc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1a2cc-110">Child elements</span></span>

<span data-ttu-id="1a2cc-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a2cc-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1a2cc-112">Parent elements</span></span>

|<span data-ttu-id="1a2cc-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1a2cc-113">**Element**</span></span>|<span data-ttu-id="1a2cc-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a2cc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a2cc-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="1a2cc-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="1a2cc-116">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a2cc-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1a2cc-117">Text value</span></span>

<span data-ttu-id="1a2cc-118">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-118">A text value is required.</span></span> <span data-ttu-id="1a2cc-119">В следующей таблице перечислены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-119">The following table lists the possible text values for this element.</span></span>
  
|<span data-ttu-id="1a2cc-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="1a2cc-120">**Value**</span></span>|<span data-ttu-id="1a2cc-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a2cc-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a2cc-122">FullUpdate</span><span class="sxs-lookup"><span data-stu-id="1a2cc-122">FullUpdate</span></span>  <br/> |<span data-ttu-id="1a2cc-123">Определяет запрос на собрание как полное обновление для существующего запроса.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-123">Identifies the meeting request as a full update to an existing request.</span></span> <span data-ttu-id="1a2cc-124">Полное обновление обновил времени и информационного контента.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-124">A full update has updated time and informational content.</span></span>  <br/> |
|<span data-ttu-id="1a2cc-125">InformationalUpdate</span><span class="sxs-lookup"><span data-stu-id="1a2cc-125">InformationalUpdate</span></span>  <br/> |<span data-ttu-id="1a2cc-126">Определяет запрос на собрание, содержащее обновления информационного контента.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-126">Identifies the meeting request as only containing updated informational content.</span></span>  <br/> |
|<span data-ttu-id="1a2cc-127">NewMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="1a2cc-127">NewMeetingRequest</span></span>  <br/> |<span data-ttu-id="1a2cc-128">Указывает запрос на собрание в качестве нового приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-128">Identifies the meeting request as a new meeting request.</span></span>  <br/> |
|<span data-ttu-id="1a2cc-129">Нет</span><span class="sxs-lookup"><span data-stu-id="1a2cc-129">None</span></span>  <br/> |<span data-ttu-id="1a2cc-130">Указывает, что собрание тип не определен.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-130">Indicates that the meeting request type is not defined.</span></span>  <br/> |
|<span data-ttu-id="1a2cc-131">Устаревшие</span><span class="sxs-lookup"><span data-stu-id="1a2cc-131">Outdated</span></span>  <br/> |<span data-ttu-id="1a2cc-132">Определяет запрос на собрание считается устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-132">Identifies the meeting request as outdated.</span></span>  <br/> |
|<span data-ttu-id="1a2cc-133">PrincipalWantsCopy</span><span class="sxs-lookup"><span data-stu-id="1a2cc-133">PrincipalWantsCopy</span></span>  <br/> |<span data-ttu-id="1a2cc-134">Показывает, что запрос на собрание принадлежит участника, кто имеет свой копии, помеченные как информационные и перенаправление сообщений о собрании делегат.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-134">Indicates that the meeting request belongs to a principal who has forwarded meeting messages to a delegate and has his copies marked as informational.</span></span>  <br/> |
|<span data-ttu-id="1a2cc-135">SilentUpdate</span><span class="sxs-lookup"><span data-stu-id="1a2cc-135">SilentUpdate</span></span>  <br/> |<span data-ttu-id="1a2cc-136">Указывает запрос на собрание в качестве автоматической обновление для существующего собрания.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-136">Identifies the meeting request as a silent update to an existing meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1a2cc-137">Замечания</span><span class="sxs-lookup"><span data-stu-id="1a2cc-137">Remarks</span></span>

<span data-ttu-id="1a2cc-138">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1a2cc-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a2cc-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1a2cc-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a2cc-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1a2cc-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a2cc-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1a2cc-141">Schema Name</span></span>  <br/> |<span data-ttu-id="1a2cc-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1a2cc-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a2cc-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1a2cc-143">Validation File</span></span>  <br/> |<span data-ttu-id="1a2cc-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1a2cc-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a2cc-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1a2cc-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a2cc-146">False</span><span class="sxs-lookup"><span data-stu-id="1a2cc-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a2cc-147">См. также</span><span class="sxs-lookup"><span data-stu-id="1a2cc-147">See also</span></span>



- [<span data-ttu-id="1a2cc-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1a2cc-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

