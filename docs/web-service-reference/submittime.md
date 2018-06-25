---
title: SubmitTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubmitTime
api_type:
- schema
ms.assetid: 97e4b71e-f45c-4bdb-80f9-805934916c0f
description: Элемент SubmitTime представляет время, когда сообщение было отправлено на сервер.
ms.openlocfilehash: 3f19e2ac14b412ef8d1ab59eb069f0223cf782ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835617"
---
# <a name="submittime"></a><span data-ttu-id="b5806-103">SubmitTime</span><span class="sxs-lookup"><span data-stu-id="b5806-103">SubmitTime</span></span>

<span data-ttu-id="b5806-104">Элемент **SubmitTime** представляет время, когда сообщение было отправлено на сервер.</span><span class="sxs-lookup"><span data-stu-id="b5806-104">The **SubmitTime** element represents the time at which the message was sent to the server.</span></span> 
  
```XML
<SubmitTime/>
```

 <span data-ttu-id="b5806-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="b5806-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5806-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b5806-106">Attributes and elements</span></span>

<span data-ttu-id="b5806-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b5806-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5806-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b5806-108">Attributes</span></span>

<span data-ttu-id="b5806-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5806-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5806-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b5806-110">Child elements</span></span>

<span data-ttu-id="b5806-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5806-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5806-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b5806-112">Parent elements</span></span>

|<span data-ttu-id="b5806-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b5806-113">**Element**</span></span>|<span data-ttu-id="b5806-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b5806-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5806-115">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b5806-115">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="b5806-116">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b5806-116">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b5806-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b5806-117">Text value</span></span>

<span data-ttu-id="b5806-118">Текстовое значение, представляющее даты/времени является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="b5806-118">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b5806-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="b5806-119">Remarks</span></span>

<span data-ttu-id="b5806-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5806-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5806-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b5806-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5806-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b5806-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5806-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b5806-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b5806-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b5806-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5806-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b5806-125">Validation File</span></span>  <br/> |<span data-ttu-id="b5806-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b5806-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5806-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b5806-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b5806-128">False</span><span class="sxs-lookup"><span data-stu-id="b5806-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5806-129">См. также</span><span class="sxs-lookup"><span data-stu-id="b5806-129">See also</span></span>



[<span data-ttu-id="b5806-130">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b5806-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="b5806-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b5806-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

