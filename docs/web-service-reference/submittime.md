---
title: субмиттиме
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
description: Элемент Субмиттиме представляет время отправки сообщения на сервер.
ms.openlocfilehash: 3f19e2ac14b412ef8d1ab59eb069f0223cf782ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835617"
---
# <a name="submittime"></a><span data-ttu-id="faf51-103">субмиттиме</span><span class="sxs-lookup"><span data-stu-id="faf51-103">SubmitTime</span></span>

<span data-ttu-id="faf51-104">Элемент **субмиттиме** представляет время отправки сообщения на сервер.</span><span class="sxs-lookup"><span data-stu-id="faf51-104">The **SubmitTime** element represents the time at which the message was sent to the server.</span></span> 
  
```XML
<SubmitTime/>
```

 <span data-ttu-id="faf51-105">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="faf51-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="faf51-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="faf51-106">Attributes and elements</span></span>

<span data-ttu-id="faf51-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="faf51-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="faf51-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="faf51-108">Attributes</span></span>

<span data-ttu-id="faf51-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="faf51-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="faf51-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="faf51-110">Child elements</span></span>

<span data-ttu-id="faf51-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="faf51-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="faf51-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="faf51-112">Parent elements</span></span>

|<span data-ttu-id="faf51-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="faf51-113">**Element**</span></span>|<span data-ttu-id="faf51-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="faf51-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="faf51-115">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="faf51-115">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="faf51-116">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="faf51-116">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="faf51-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="faf51-117">Text value</span></span>

<span data-ttu-id="faf51-118">При использовании этого элемента необходимо указать текстовое значение, представляющее дату и время.</span><span class="sxs-lookup"><span data-stu-id="faf51-118">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="faf51-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="faf51-119">Remarks</span></span>

<span data-ttu-id="faf51-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="faf51-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="faf51-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="faf51-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="faf51-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="faf51-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="faf51-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="faf51-123">Schema Name</span></span>  <br/> |<span data-ttu-id="faf51-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="faf51-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="faf51-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="faf51-125">Validation File</span></span>  <br/> |<span data-ttu-id="faf51-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="faf51-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="faf51-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="faf51-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="faf51-128">False</span><span class="sxs-lookup"><span data-stu-id="faf51-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="faf51-129">См. также</span><span class="sxs-lookup"><span data-stu-id="faf51-129">See also</span></span>



[<span data-ttu-id="faf51-130">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="faf51-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="faf51-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="faf51-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

