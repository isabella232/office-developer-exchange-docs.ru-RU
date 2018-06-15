---
title: IsDelegated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsDelegated
api_type:
- schema
ms.assetid: c12907db-be80-4924-9469-8e58612cf42c
description: Элемент IsDelegated указывает, обработано ли собрания с помощью учетной записи, имеющей права доступа делегата.
ms.openlocfilehash: a6f42a57b2d0fdb760e4c36d3211ba57289a3c7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2018
ms.locfileid: "19834005"
---
# <a name="isdelegated"></a><span data-ttu-id="b5908-103">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="b5908-103">IsDelegated</span></span>

<span data-ttu-id="b5908-104">Элемент **IsDelegated** указывает, обработано ли собрания с помощью учетной записи, имеющей права доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="b5908-104">The **IsDelegated** element indicates whether a meeting was handled by an account that has delegate access.</span></span> 
  
```xml
<IsDelegated/>
```

 <span data-ttu-id="b5908-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b5908-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5908-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b5908-106">Attributes and elements</span></span>

<span data-ttu-id="b5908-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b5908-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5908-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b5908-108">Attributes</span></span>

<span data-ttu-id="b5908-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5908-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5908-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b5908-110">Child elements</span></span>

<span data-ttu-id="b5908-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5908-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5908-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b5908-112">Parent elements</span></span>

|<span data-ttu-id="b5908-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b5908-113">**Element**</span></span>|<span data-ttu-id="b5908-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b5908-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5908-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b5908-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b5908-116">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5908-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b5908-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b5908-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b5908-118">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5908-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b5908-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b5908-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b5908-120">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5908-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b5908-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b5908-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b5908-122">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5908-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b5908-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b5908-123">Text value</span></span>

<span data-ttu-id="b5908-124">Текстовое значение **true,** указывает, что приглашение на собрание было обработано под учетной записью, имеющей права доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="b5908-124">A text value of **true** indicates that the meeting was handled by an account that has delegate access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b5908-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="b5908-125">Remarks</span></span>

<span data-ttu-id="b5908-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b5908-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5908-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b5908-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5908-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b5908-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5908-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b5908-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b5908-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b5908-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5908-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b5908-131">Validation File</span></span>  <br/> |<span data-ttu-id="b5908-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b5908-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5908-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b5908-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="b5908-134">False</span><span class="sxs-lookup"><span data-stu-id="b5908-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5908-135">См. также</span><span class="sxs-lookup"><span data-stu-id="b5908-135">See also</span></span>



- [<span data-ttu-id="b5908-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b5908-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

