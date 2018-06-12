---
title: HasBeenProcessed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasBeenProcessed
api_type:
- schema
ms.assetid: 46d4af8e-0f11-4a74-9365-1d983731fed8
description: Элемент HasBeenProcessed указывает ли сообщение собрания элемент обработки.
ms.openlocfilehash: cccd3b2258490fcbe902bcd391f25b0be2fe7c26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833796"
---
# <a name="hasbeenprocessed"></a><span data-ttu-id="e57e4-103">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="e57e4-103">HasBeenProcessed</span></span>

<span data-ttu-id="e57e4-104">Элемент **HasBeenProcessed** указывает ли сообщение собрания элемент обработки.</span><span class="sxs-lookup"><span data-stu-id="e57e4-104">The **HasBeenProcessed** element indicates whether a meeting message item has been processed.</span></span> 
  
```xml
<HasBeenProcessed/>
```

 <span data-ttu-id="e57e4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e57e4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e57e4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e57e4-106">Attributes and elements</span></span>

<span data-ttu-id="e57e4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e57e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e57e4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e57e4-108">Attributes</span></span>

<span data-ttu-id="e57e4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e57e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e57e4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e57e4-110">Child elements</span></span>

<span data-ttu-id="e57e4-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e57e4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e57e4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e57e4-112">Parent elements</span></span>

|<span data-ttu-id="e57e4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e57e4-113">**Element**</span></span>|<span data-ttu-id="e57e4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e57e4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e57e4-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e57e4-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e57e4-116">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e57e4-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e57e4-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e57e4-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e57e4-118">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e57e4-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e57e4-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e57e4-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e57e4-120">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e57e4-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e57e4-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e57e4-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e57e4-122">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e57e4-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e57e4-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e57e4-123">Text value</span></span>

<span data-ttu-id="e57e4-124">Текстовое значение **true,** указывает, что сообщение собрание было обработано.</span><span class="sxs-lookup"><span data-stu-id="e57e4-124">A text value of **true** indicates that the meeting message has been processed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e57e4-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="e57e4-125">Remarks</span></span>

<span data-ttu-id="e57e4-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e57e4-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e57e4-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e57e4-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e57e4-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e57e4-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e57e4-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e57e4-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e57e4-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e57e4-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="e57e4-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e57e4-131">Validation File</span></span>  <br/> |<span data-ttu-id="e57e4-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e57e4-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e57e4-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e57e4-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="e57e4-134">False</span><span class="sxs-lookup"><span data-stu-id="e57e4-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e57e4-135">См. также</span><span class="sxs-lookup"><span data-stu-id="e57e4-135">See also</span></span>



- [<span data-ttu-id="e57e4-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e57e4-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

