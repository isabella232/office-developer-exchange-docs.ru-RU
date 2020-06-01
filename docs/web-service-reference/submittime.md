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
ms.openlocfilehash: e4409d962988ee308e0c0b461f9448ef68067fe8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467055"
---
# <a name="submittime"></a><span data-ttu-id="9b121-103">субмиттиме</span><span class="sxs-lookup"><span data-stu-id="9b121-103">SubmitTime</span></span>

<span data-ttu-id="9b121-104">Элемент **субмиттиме** представляет время отправки сообщения на сервер.</span><span class="sxs-lookup"><span data-stu-id="9b121-104">The **SubmitTime** element represents the time at which the message was sent to the server.</span></span> 
  
```XML
<SubmitTime/>
```

 <span data-ttu-id="9b121-105">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="9b121-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b121-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9b121-106">Attributes and elements</span></span>

<span data-ttu-id="9b121-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9b121-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b121-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9b121-108">Attributes</span></span>

<span data-ttu-id="9b121-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9b121-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b121-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9b121-110">Child elements</span></span>

<span data-ttu-id="9b121-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9b121-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9b121-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9b121-112">Parent elements</span></span>

|<span data-ttu-id="9b121-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9b121-113">**Element**</span></span>|<span data-ttu-id="9b121-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9b121-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b121-115">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="9b121-115">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="9b121-116">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9b121-116">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9b121-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9b121-117">Text value</span></span>

<span data-ttu-id="9b121-118">При использовании этого элемента необходимо указать текстовое значение, представляющее дату и время.</span><span class="sxs-lookup"><span data-stu-id="9b121-118">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9b121-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="9b121-119">Remarks</span></span>

<span data-ttu-id="9b121-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b121-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b121-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9b121-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b121-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9b121-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b121-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9b121-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9b121-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9b121-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b121-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9b121-125">Validation File</span></span>  <br/> |<span data-ttu-id="9b121-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9b121-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b121-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9b121-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b121-128">False</span><span class="sxs-lookup"><span data-stu-id="9b121-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b121-129">См. также</span><span class="sxs-lookup"><span data-stu-id="9b121-129">See also</span></span>



[<span data-ttu-id="9b121-130">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="9b121-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="9b121-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9b121-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

