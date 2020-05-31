---
title: жетнониндексаблеитемстатистиксреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c969475a-238d-47ec-947a-fe3c53c8c1e9
description: Элемент Жетнониндексаблеитемстатистиксреспонсемессаже указывает ответное сообщение для запроса GetNonIndexableItemStatistics.
ms.openlocfilehash: 5d2de21378fe53af16679c5648a1bb8accb223fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762862"
---
# <a name="getnonindexableitemstatisticsresponsemessage"></a><span data-ttu-id="ff463-103">жетнониндексаблеитемстатистиксреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ff463-103">GetNonIndexableItemStatisticsResponseMessage</span></span>

<span data-ttu-id="ff463-104">Элемент **жетнониндексаблеитемстатистиксреспонсемессаже** указывает ответное сообщение для запроса **GetNonIndexableItemStatistics** .</span><span class="sxs-lookup"><span data-stu-id="ff463-104">The **GetNonIndexableItemStatisticsResponseMessage** element specifies the response message for a **GetNonIndexableItemStatistics** request.</span></span> 
  
```XML
<GetNonIndexableItemStatisticsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemStatistics/>
</GetNonIndexableItemStatisticsResponseMessage>
```

 <span data-ttu-id="ff463-105">**жетнониндексаблеитемстатистиксреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="ff463-105">**GetNonIndexableItemStatisticsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff463-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ff463-106">Attributes and elements</span></span>

<span data-ttu-id="ff463-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ff463-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff463-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ff463-108">Attributes</span></span>

<span data-ttu-id="ff463-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ff463-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff463-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ff463-110">Child elements</span></span>

<span data-ttu-id="ff463-111">[Мессажетекст](messagetext.md) | [респонсекоде](responsecode.md) | [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) [MessageXml](messagexml.md)[DescriptiveLinkKey](descriptivelinkkey.md)дескриптивелинккэй мессажексмл GetNonIndexableItemStatistics |  | </span><span class="sxs-lookup"><span data-stu-id="ff463-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff463-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ff463-112">Parent elements</span></span>

[<span data-ttu-id="ff463-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="ff463-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="ff463-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="ff463-114">Remarks</span></span>

<span data-ttu-id="ff463-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ff463-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ff463-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff463-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff463-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ff463-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff463-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ff463-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff463-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ff463-119">Schema name</span></span>  <br/> |<span data-ttu-id="ff463-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ff463-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff463-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ff463-121">Validation file</span></span>  <br/> |<span data-ttu-id="ff463-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ff463-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff463-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ff463-123">Can be empty</span></span>  <br/> |<span data-ttu-id="ff463-124">false</span><span class="sxs-lookup"><span data-stu-id="ff463-124">false</span></span>  <br/> |
   

