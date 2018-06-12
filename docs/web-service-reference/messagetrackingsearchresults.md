---
title: MessageTrackingSearchResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResults
api_type:
- schema
ms.assetid: 6bf36f37-c2b3-40c1-a4df-31573ed8642a
description: Элемент MessageTrackingSearchResults содержит список записей, которые соответствуют условиям поиска.
ms.openlocfilehash: 866cc8d4e9afa8347eb7bd0d9e9acaddc616c396
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834454"
---
# <a name="messagetrackingsearchresults"></a><span data-ttu-id="c1002-103">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="c1002-103">MessageTrackingSearchResults</span></span>

<span data-ttu-id="c1002-104">Элемент **MessageTrackingSearchResults** содержит список записей, которые соответствуют условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="c1002-104">The **MessageTrackingSearchResults** element contains a list of records that match the search criteria.</span></span> 
  
```XML
<MessageTrackingSearchResults>
   <MessageTrackingSearchResult/>
</MessageTrackingSearchResults>
```

 <span data-ttu-id="c1002-105">**ArrayOfFindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="c1002-105">**ArrayOfFindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1002-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c1002-106">Attributes and elements</span></span>

<span data-ttu-id="c1002-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c1002-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1002-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c1002-108">Attributes</span></span>

<span data-ttu-id="c1002-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c1002-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1002-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c1002-110">Child elements</span></span>

|<span data-ttu-id="c1002-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1002-111">**Element**</span></span>|<span data-ttu-id="c1002-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1002-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1002-113">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="c1002-113">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="c1002-114">Содержит результат одного сообщения для элемента [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="c1002-114">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1002-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c1002-115">Parent elements</span></span>

|<span data-ttu-id="c1002-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1002-116">**Element**</span></span>|<span data-ttu-id="c1002-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1002-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1002-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="c1002-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="c1002-119">Содержит состояние и результат одного запроса [FindMessageTrackingReport операции](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c1002-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c1002-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c1002-120">Text value</span></span>

<span data-ttu-id="c1002-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="c1002-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c1002-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="c1002-122">Remarks</span></span>

<span data-ttu-id="c1002-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1002-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1002-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c1002-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1002-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c1002-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c1002-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c1002-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c1002-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c1002-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c1002-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c1002-128">Validation File</span></span>  <br/> |<span data-ttu-id="c1002-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c1002-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c1002-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c1002-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c1002-131">False</span><span class="sxs-lookup"><span data-stu-id="c1002-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1002-132">См. также</span><span class="sxs-lookup"><span data-stu-id="c1002-132">See also</span></span>



- [<span data-ttu-id="c1002-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c1002-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

