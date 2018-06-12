---
title: NonIndexableItemStatistic
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 593e0c79-9ec2-4040-a6a3-3c5c61cbdf7c
description: Элемент NonIndexableItemStatistic содержит один статистика для элемента, который не будет индексироваться
ms.openlocfilehash: e604f73216aab4cca259bc6cb7eb80a2fd36cd23
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834540"
---
# <a name="nonindexableitemstatistic"></a><span data-ttu-id="3aa5c-103">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="3aa5c-103">NonIndexableItemStatistic</span></span>

<span data-ttu-id="3aa5c-104">Элемент **NonIndexableItemStatistic** содержит один статистика для элемента, который не будет индексироваться</span><span class="sxs-lookup"><span data-stu-id="3aa5c-104">The **NonIndexableItemStatistic** element contains a single statistic for an item that could not be indexed</span></span> 
  
```XML
<NonIndexableItemStatistic>
   <Mailbox/>
   <ItemCount/>
   <ErrorMessage/>
</NonIndexableItemStatistic>
```

 <span data-ttu-id="3aa5c-105">**NonIndexableItemStatisticType**</span><span class="sxs-lookup"><span data-stu-id="3aa5c-105">**NonIndexableItemStatisticType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3aa5c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3aa5c-106">Attributes and elements</span></span>

<span data-ttu-id="3aa5c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3aa5c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3aa5c-108">Attributes</span></span>

<span data-ttu-id="3aa5c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3aa5c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3aa5c-110">Child elements</span></span>

<span data-ttu-id="3aa5c-111">[Почтовый ящик (string)](mailbox-string.md) | [ItemCount](itemcount.md) | [сообщение об ошибке](errormessage.md)</span><span class="sxs-lookup"><span data-stu-id="3aa5c-111">[Mailbox (string)](mailbox-string.md) | [ItemCount](itemcount.md) | [ErrorMessage](errormessage.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3aa5c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3aa5c-112">Parent elements</span></span>

[<span data-ttu-id="3aa5c-113">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="3aa5c-113">NonIndexableItemStatistics</span></span>](nonindexableitemstatistics.md)
  
## <a name="remarks"></a><span data-ttu-id="3aa5c-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="3aa5c-114">Remarks</span></span>

<span data-ttu-id="3aa5c-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3aa5c-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3aa5c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3aa5c-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3aa5c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3aa5c-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3aa5c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3aa5c-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3aa5c-119">Schema name</span></span>  <br/> |<span data-ttu-id="3aa5c-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3aa5c-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3aa5c-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3aa5c-121">Validation file</span></span>  <br/> |<span data-ttu-id="3aa5c-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3aa5c-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3aa5c-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3aa5c-123">Can be empty</span></span>  <br/> |<span data-ttu-id="3aa5c-124">False</span><span class="sxs-lookup"><span data-stu-id="3aa5c-124">False</span></span>  <br/> |
   

