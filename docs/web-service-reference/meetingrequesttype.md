---
title: митингрекуесттипе
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
description: Элемент Митингрекуесттипе описывает тип приглашения на собрание.
ms.openlocfilehash: 7269587e2fa72aeb9070a7b53ee9215829729329
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834432"
---
# <a name="meetingrequesttype"></a><span data-ttu-id="95d1d-103">митингрекуесттипе</span><span class="sxs-lookup"><span data-stu-id="95d1d-103">MeetingRequestType</span></span>

<span data-ttu-id="95d1d-104">Элемент **митингрекуесттипе** описывает тип приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="95d1d-104">The **MeetingRequestType** element describes the type of the meeting request.</span></span> 
  
```xml
<MeetingRequestType/>
```

 <span data-ttu-id="95d1d-105">**митингрекуесттипетипе**</span><span class="sxs-lookup"><span data-stu-id="95d1d-105">**MeetingRequestTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95d1d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="95d1d-106">Attributes and elements</span></span>

<span data-ttu-id="95d1d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="95d1d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95d1d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="95d1d-108">Attributes</span></span>

<span data-ttu-id="95d1d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="95d1d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95d1d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="95d1d-110">Child elements</span></span>

<span data-ttu-id="95d1d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="95d1d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="95d1d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="95d1d-112">Parent elements</span></span>

|<span data-ttu-id="95d1d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="95d1d-113">**Element**</span></span>|<span data-ttu-id="95d1d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="95d1d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95d1d-115">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="95d1d-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="95d1d-116">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="95d1d-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="95d1d-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="95d1d-117">Text value</span></span>

<span data-ttu-id="95d1d-118">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="95d1d-118">A text value is required.</span></span> <span data-ttu-id="95d1d-119">В приведенной ниже таблице перечислены возможные текстовые значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="95d1d-119">The following table lists the possible text values for this element.</span></span>
  
|<span data-ttu-id="95d1d-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="95d1d-120">**Value**</span></span>|<span data-ttu-id="95d1d-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="95d1d-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="95d1d-122">фуллупдате</span><span class="sxs-lookup"><span data-stu-id="95d1d-122">FullUpdate</span></span>  <br/> |<span data-ttu-id="95d1d-123">Определяет приглашение на собрание как полное обновление существующего запроса.</span><span class="sxs-lookup"><span data-stu-id="95d1d-123">Identifies the meeting request as a full update to an existing request.</span></span> <span data-ttu-id="95d1d-124">Полное обновление обновляет время и Информационное содержимое.</span><span class="sxs-lookup"><span data-stu-id="95d1d-124">A full update has updated time and informational content.</span></span>  <br/> |
|<span data-ttu-id="95d1d-125">информатионалупдате</span><span class="sxs-lookup"><span data-stu-id="95d1d-125">InformationalUpdate</span></span>  <br/> |<span data-ttu-id="95d1d-126">Определяет приглашение на собрание, которое содержит только обновленный информационный контент.</span><span class="sxs-lookup"><span data-stu-id="95d1d-126">Identifies the meeting request as only containing updated informational content.</span></span>  <br/> |
|<span data-ttu-id="95d1d-127">NewMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="95d1d-127">NewMeetingRequest</span></span>  <br/> |<span data-ttu-id="95d1d-128">Идентифицирует приглашение на собрание в качестве нового приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="95d1d-128">Identifies the meeting request as a new meeting request.</span></span>  <br/> |
|<span data-ttu-id="95d1d-129">Нет</span><span class="sxs-lookup"><span data-stu-id="95d1d-129">None</span></span>  <br/> |<span data-ttu-id="95d1d-130">Указывает, что тип приглашения на собрание не определен.</span><span class="sxs-lookup"><span data-stu-id="95d1d-130">Indicates that the meeting request type is not defined.</span></span>  <br/> |
|<span data-ttu-id="95d1d-131">Прием</span><span class="sxs-lookup"><span data-stu-id="95d1d-131">Outdated</span></span>  <br/> |<span data-ttu-id="95d1d-132">Указывает, что приглашение на собрание считается устаревшим.</span><span class="sxs-lookup"><span data-stu-id="95d1d-132">Identifies the meeting request as outdated.</span></span>  <br/> |
|<span data-ttu-id="95d1d-133">принЦипалвантскопи</span><span class="sxs-lookup"><span data-stu-id="95d1d-133">PrincipalWantsCopy</span></span>  <br/> |<span data-ttu-id="95d1d-134">Указывает, что приглашение на собрание принадлежит участнику, который имеет переадресованные сообщения собраний представителю и имеет свои копии, помеченные как информационные.</span><span class="sxs-lookup"><span data-stu-id="95d1d-134">Indicates that the meeting request belongs to a principal who has forwarded meeting messages to a delegate and has his copies marked as informational.</span></span>  <br/> |
|<span data-ttu-id="95d1d-135">силентупдате</span><span class="sxs-lookup"><span data-stu-id="95d1d-135">SilentUpdate</span></span>  <br/> |<span data-ttu-id="95d1d-136">Определяет приглашение на собрание как неавтоматическое обновление существующего собрания.</span><span class="sxs-lookup"><span data-stu-id="95d1d-136">Identifies the meeting request as a silent update to an existing meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="95d1d-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="95d1d-137">Remarks</span></span>

<span data-ttu-id="95d1d-138">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="95d1d-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95d1d-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="95d1d-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95d1d-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="95d1d-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95d1d-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="95d1d-141">Schema Name</span></span>  <br/> |<span data-ttu-id="95d1d-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="95d1d-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="95d1d-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="95d1d-143">Validation File</span></span>  <br/> |<span data-ttu-id="95d1d-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="95d1d-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95d1d-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="95d1d-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="95d1d-146">False</span><span class="sxs-lookup"><span data-stu-id="95d1d-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95d1d-147">См. также</span><span class="sxs-lookup"><span data-stu-id="95d1d-147">See also</span></span>



- [<span data-ttu-id="95d1d-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="95d1d-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

