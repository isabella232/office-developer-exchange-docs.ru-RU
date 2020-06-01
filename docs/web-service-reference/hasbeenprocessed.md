---
title: хасбинпроцессед
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
description: Элемент Хасбинпроцессед указывает, был ли обработан элемент сообщения о собрании.
ms.openlocfilehash: 7251ca86e07a0b72c186c65094b6469331dfd12e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462895"
---
# <a name="hasbeenprocessed"></a><span data-ttu-id="5df3a-103">хасбинпроцессед</span><span class="sxs-lookup"><span data-stu-id="5df3a-103">HasBeenProcessed</span></span>

<span data-ttu-id="5df3a-104">Элемент **хасбинпроцессед** указывает, был ли обработан элемент сообщения о собрании.</span><span class="sxs-lookup"><span data-stu-id="5df3a-104">The **HasBeenProcessed** element indicates whether a meeting message item has been processed.</span></span> 
  
```xml
<HasBeenProcessed/>
```

 <span data-ttu-id="5df3a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5df3a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5df3a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5df3a-106">Attributes and elements</span></span>

<span data-ttu-id="5df3a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5df3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5df3a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5df3a-108">Attributes</span></span>

<span data-ttu-id="5df3a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5df3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5df3a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5df3a-110">Child elements</span></span>

<span data-ttu-id="5df3a-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5df3a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5df3a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5df3a-112">Parent elements</span></span>

|<span data-ttu-id="5df3a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5df3a-113">**Element**</span></span>|<span data-ttu-id="5df3a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5df3a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5df3a-115">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="5df3a-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="5df3a-116">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5df3a-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5df3a-117">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="5df3a-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="5df3a-118">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5df3a-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5df3a-119">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="5df3a-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5df3a-120">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5df3a-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5df3a-121">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="5df3a-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="5df3a-122">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5df3a-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5df3a-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5df3a-123">Text value</span></span>

<span data-ttu-id="5df3a-124">Текстовое значение **true** указывает, что сообщение о собрании было обработано.</span><span class="sxs-lookup"><span data-stu-id="5df3a-124">A text value of **true** indicates that the meeting message has been processed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5df3a-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="5df3a-125">Remarks</span></span>

<span data-ttu-id="5df3a-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5df3a-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5df3a-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5df3a-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5df3a-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5df3a-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5df3a-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5df3a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="5df3a-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5df3a-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="5df3a-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5df3a-131">Validation File</span></span>  <br/> |<span data-ttu-id="5df3a-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5df3a-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5df3a-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5df3a-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="5df3a-134">False</span><span class="sxs-lookup"><span data-stu-id="5df3a-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5df3a-135">См. также</span><span class="sxs-lookup"><span data-stu-id="5df3a-135">See also</span></span>



- [<span data-ttu-id="5df3a-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5df3a-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

