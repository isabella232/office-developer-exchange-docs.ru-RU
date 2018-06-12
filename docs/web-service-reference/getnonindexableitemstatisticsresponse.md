---
title: GetNonIndexableItemStatisticsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f68b73c-d6b0-4bb5-b89a-fd398d09346c
description: Элемент GetNonIndexableItemStatisticsResponse указывает ответ на запрос GetNonIndexableItemStatistics.
ms.openlocfilehash: 95f59df251517cb76183f6f8bd6c2d4a68bd4cdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762861"
---
# <a name="getnonindexableitemstatisticsresponse"></a><span data-ttu-id="0d03a-103">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="0d03a-103">GetNonIndexableItemStatisticsResponse</span></span>

<span data-ttu-id="0d03a-104">Элемент **GetNonIndexableItemStatisticsResponse** указывает ответ на запрос **GetNonIndexableItemStatistics** .</span><span class="sxs-lookup"><span data-stu-id="0d03a-104">The **GetNonIndexableItemStatisticsResponse** element specifies the response to a **GetNonIndexableItemStatistics** request.</span></span> 
  
```XML
<GetNonIndexableItemStatisticsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemStatistics/>
</GetNonIndexableItemStatisticsResponse>
```

 <span data-ttu-id="0d03a-105">**GetNonIndexableItemStatisticsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0d03a-105">**GetNonIndexableItemStatisticsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d03a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0d03a-106">Attributes and elements</span></span>

<span data-ttu-id="0d03a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0d03a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d03a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0d03a-108">Attributes</span></span>

<span data-ttu-id="0d03a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0d03a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d03a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0d03a-110">Child elements</span></span>

<span data-ttu-id="0d03a-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md)</span><span class="sxs-lookup"><span data-stu-id="0d03a-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d03a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0d03a-112">Parent elements</span></span>

[<span data-ttu-id="0d03a-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0d03a-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="0d03a-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="0d03a-114">Remarks</span></span>

<span data-ttu-id="0d03a-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0d03a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0d03a-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d03a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d03a-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0d03a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d03a-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0d03a-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0d03a-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0d03a-119">Schema name</span></span>  <br/> |<span data-ttu-id="0d03a-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0d03a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0d03a-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0d03a-121">Validation file</span></span>  <br/> |<span data-ttu-id="0d03a-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0d03a-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0d03a-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0d03a-123">Can be empty</span></span>  <br/> |<span data-ttu-id="0d03a-124">Нет</span><span class="sxs-lookup"><span data-stu-id="0d03a-124">false</span></span>  <br/> |
   

