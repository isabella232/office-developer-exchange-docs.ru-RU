---
title: IsOutOfDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOutOfDate
api_type:
- schema
ms.assetid: 2b6005a6-56a9-4848-b998-32908c13e2e2
description: Элемент IsOutOfDate указывает, является ли сообщения о собрании, собрание, ответа или отмены устаревшей.
ms.openlocfilehash: 0a6b2670cc3eb260002821bab31d652177902de1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834110"
---
# <a name="isoutofdate"></a><span data-ttu-id="bd8dd-103">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="bd8dd-103">IsOutOfDate</span></span>

<span data-ttu-id="bd8dd-104">Элемент **IsOutOfDate** указывает, является ли сообщения о собрании, собрание, ответа или отмены устаревшей.</span><span class="sxs-lookup"><span data-stu-id="bd8dd-104">The **IsOutOfDate** element indicates whether a meeting message, request, response, or cancellation is out-of-date.</span></span> 
  
```xml
<IsOutOfDate/>
```

 <span data-ttu-id="bd8dd-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="bd8dd-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd8dd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bd8dd-106">Attributes and elements</span></span>

<span data-ttu-id="bd8dd-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bd8dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd8dd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bd8dd-108">Attributes</span></span>

<span data-ttu-id="bd8dd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd8dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd8dd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bd8dd-110">Child elements</span></span>

<span data-ttu-id="bd8dd-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd8dd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bd8dd-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bd8dd-112">Parent elements</span></span>

|<span data-ttu-id="bd8dd-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd8dd-113">**Element**</span></span>|<span data-ttu-id="bd8dd-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd8dd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd8dd-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="bd8dd-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="bd8dd-116">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd8dd-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bd8dd-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="bd8dd-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="bd8dd-118">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd8dd-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bd8dd-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="bd8dd-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="bd8dd-120">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd8dd-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bd8dd-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="bd8dd-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="bd8dd-122">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd8dd-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd8dd-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bd8dd-123">Text value</span></span>

<span data-ttu-id="bd8dd-124">Текстовое значение **true,** указывает, что элемент собрания является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="bd8dd-124">A text value of **true** indicates that the meeting item is out-of-date.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bd8dd-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="bd8dd-125">Remarks</span></span>

<span data-ttu-id="bd8dd-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bd8dd-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd8dd-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bd8dd-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd8dd-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bd8dd-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd8dd-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bd8dd-129">Schema Name</span></span>  <br/> |<span data-ttu-id="bd8dd-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bd8dd-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd8dd-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bd8dd-131">Validation File</span></span>  <br/> |<span data-ttu-id="bd8dd-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bd8dd-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd8dd-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bd8dd-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd8dd-134">False</span><span class="sxs-lookup"><span data-stu-id="bd8dd-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd8dd-135">См. также</span><span class="sxs-lookup"><span data-stu-id="bd8dd-135">See also</span></span>



- [<span data-ttu-id="bd8dd-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bd8dd-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

