---
title: мессажетраккингсеарчресултс
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
description: Элемент Мессажетраккингсеарчресултс содержит список записей, которые отвечают условиям поиска.
ms.openlocfilehash: 1e03cb135b7b2a125da1e29f7293d233f4e20ddb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468679"
---
# <a name="messagetrackingsearchresults"></a><span data-ttu-id="4f8b7-103">мессажетраккингсеарчресултс</span><span class="sxs-lookup"><span data-stu-id="4f8b7-103">MessageTrackingSearchResults</span></span>

<span data-ttu-id="4f8b7-104">Элемент **мессажетраккингсеарчресултс** содержит список записей, которые отвечают условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="4f8b7-104">The **MessageTrackingSearchResults** element contains a list of records that match the search criteria.</span></span> 
  
```XML
<MessageTrackingSearchResults>
   <MessageTrackingSearchResult/>
</MessageTrackingSearchResults>
```

 <span data-ttu-id="4f8b7-105">**аррайоффиндмессажетраккингсеарчресулттипе**</span><span class="sxs-lookup"><span data-stu-id="4f8b7-105">**ArrayOfFindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f8b7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4f8b7-106">Attributes and elements</span></span>

<span data-ttu-id="4f8b7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4f8b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f8b7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4f8b7-108">Attributes</span></span>

<span data-ttu-id="4f8b7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4f8b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f8b7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4f8b7-110">Child elements</span></span>

|<span data-ttu-id="4f8b7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4f8b7-111">**Element**</span></span>|<span data-ttu-id="4f8b7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4f8b7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f8b7-113">мессажетраккингсеарчресулт</span><span class="sxs-lookup"><span data-stu-id="4f8b7-113">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="4f8b7-114">Содержит один результат одного сообщения для элемента [финдмессажетраккингрепортреспонсе](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="4f8b7-114">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4f8b7-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4f8b7-115">Parent elements</span></span>

|<span data-ttu-id="4f8b7-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4f8b7-116">**Element**</span></span>|<span data-ttu-id="4f8b7-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4f8b7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f8b7-118">финдмессажетраккингрепортреспонсе</span><span class="sxs-lookup"><span data-stu-id="4f8b7-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="4f8b7-119">Содержит состояние и результат одного запроса [операции FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4f8b7-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4f8b7-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4f8b7-120">Text value</span></span>

<span data-ttu-id="4f8b7-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="4f8b7-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4f8b7-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="4f8b7-122">Remarks</span></span>

<span data-ttu-id="4f8b7-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f8b7-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f8b7-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4f8b7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f8b7-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4f8b7-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4f8b7-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4f8b7-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4f8b7-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4f8b7-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4f8b7-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4f8b7-128">Validation File</span></span>  <br/> |<span data-ttu-id="4f8b7-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4f8b7-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4f8b7-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4f8b7-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4f8b7-131">False</span><span class="sxs-lookup"><span data-stu-id="4f8b7-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f8b7-132">См. также</span><span class="sxs-lookup"><span data-stu-id="4f8b7-132">See also</span></span>



- [<span data-ttu-id="4f8b7-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4f8b7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

