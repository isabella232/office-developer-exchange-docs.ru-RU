---
title: NonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12f2934a-008c-4236-b8b3-7c7b6b5707e2
description: Элемент NonIndexableItemStatistics содержит массив статистики для элементов, которые не удалось проиндексировать.
ms.openlocfilehash: 1414053b6d39f4cd08ccfd1a11faaf1b13c2052b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834544"
---
# <a name="nonindexableitemstatistics"></a><span data-ttu-id="d327d-103">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="d327d-103">NonIndexableItemStatistics</span></span>

<span data-ttu-id="d327d-104">Элемент **NonIndexableItemStatistics** содержит массив статистики для элементов, которые не удалось проиндексировать.</span><span class="sxs-lookup"><span data-stu-id="d327d-104">The **NonIndexableItemStatistics** element contains an array of statistics for items that could not be indexed.</span></span> 
  
```XML
<NonIndexableItemStatistics>
   <NonIndexableItemStatistic/>
</NonIndexableItemStatistics>
```

 <span data-ttu-id="d327d-105">**ArrayOfNonIndexableItemStatisticsType**</span><span class="sxs-lookup"><span data-stu-id="d327d-105">**ArrayOfNonIndexableItemStatisticsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d327d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d327d-106">Attributes and elements</span></span>

<span data-ttu-id="d327d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d327d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d327d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d327d-108">Attributes</span></span>

<span data-ttu-id="d327d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d327d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d327d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d327d-110">Child elements</span></span>

[<span data-ttu-id="d327d-111">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="d327d-111">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
  
### <a name="parent-elements"></a><span data-ttu-id="d327d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d327d-112">Parent elements</span></span>

<span data-ttu-id="d327d-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="d327d-113">[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d327d-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="d327d-114">Remarks</span></span>

<span data-ttu-id="d327d-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d327d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d327d-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d327d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d327d-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d327d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d327d-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d327d-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d327d-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d327d-119">Schema name</span></span>  <br/> |<span data-ttu-id="d327d-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d327d-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d327d-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d327d-121">Validation file</span></span>  <br/> |<span data-ttu-id="d327d-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d327d-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d327d-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d327d-123">Can be empty</span></span>  <br/> |<span data-ttu-id="d327d-124">False</span><span class="sxs-lookup"><span data-stu-id="d327d-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d327d-125">См. также</span><span class="sxs-lookup"><span data-stu-id="d327d-125">See also</span></span>



[<span data-ttu-id="d327d-126">Операция GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="d327d-126">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)


- [<span data-ttu-id="d327d-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d327d-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

