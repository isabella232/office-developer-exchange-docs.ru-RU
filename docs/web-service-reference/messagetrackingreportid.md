---
title: MessageTrackingReportId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReportId
api_type:
- schema
ms.assetid: 9c604ca3-10fe-4760-b7fd-8b52f1a0c712
description: Элемент MessageTrackingReportId представляет сообщение, его идентификатор сообщения, организации, где сообщение об ошибке, сервер, на котором было отправлено сообщение и внутренний идентификатор, который уникальным образом определяет сообщение.
ms.openlocfilehash: 8e0d85b203b8a34acedb5f6b9fe46359d5e0b97c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834456"
---
# <a name="messagetrackingreportid"></a><span data-ttu-id="761b3-103">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="761b3-103">MessageTrackingReportId</span></span>

<span data-ttu-id="761b3-104">Элемент **MessageTrackingReportId** представляет сообщение, его идентификатор сообщения, организации, где сообщение об ошибке, сервер, на котором было отправлено сообщение и внутренний идентификатор, который уникальным образом определяет сообщение.</span><span class="sxs-lookup"><span data-stu-id="761b3-104">The **MessageTrackingReportId** element represents the message by its message ID, the organization where the message was found, the server on which the message was submitted, and an internal ID that uniquely identifies the message.</span></span> 
  
```XML
<MessageTrackingReportId/>
```

 <span data-ttu-id="761b3-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="761b3-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="761b3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="761b3-106">Attributes and elements</span></span>

<span data-ttu-id="761b3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="761b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="761b3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="761b3-108">Attributes</span></span>

<span data-ttu-id="761b3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="761b3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="761b3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="761b3-110">Child elements</span></span>

<span data-ttu-id="761b3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="761b3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="761b3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="761b3-112">Parent elements</span></span>

|<span data-ttu-id="761b3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="761b3-113">**Element**</span></span>|<span data-ttu-id="761b3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="761b3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="761b3-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="761b3-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="761b3-116">Содержит запроса для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного сообщения, отслеживания отчетов для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="761b3-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="761b3-117">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="761b3-117">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="761b3-118">Содержит результат одного сообщения для элемента [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="761b3-118">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="761b3-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="761b3-119">Text value</span></span>

<span data-ttu-id="761b3-120">Текстовое значение, представляющее строку является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="761b3-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="761b3-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="761b3-121">Remarks</span></span>

<span data-ttu-id="761b3-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="761b3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="761b3-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="761b3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="761b3-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="761b3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="761b3-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="761b3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="761b3-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="761b3-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="761b3-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="761b3-127">Validation File</span></span>  <br/> |<span data-ttu-id="761b3-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="761b3-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="761b3-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="761b3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="761b3-130">False</span><span class="sxs-lookup"><span data-stu-id="761b3-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="761b3-131">См. также</span><span class="sxs-lookup"><span data-stu-id="761b3-131">See also</span></span>



[<span data-ttu-id="761b3-132">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="761b3-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="761b3-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="761b3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

