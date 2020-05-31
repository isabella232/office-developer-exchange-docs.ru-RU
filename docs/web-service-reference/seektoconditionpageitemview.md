---
title: сиктокондитионпажеитемвиев
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: Элемент Сиктокондитионпажеитемвиев определяет условие, которое используется для определения конца поиска, начального индекса поиска, максимальных возвращаемых записей и инструкций поиска для поиска FindItem или FindConversation.
ms.openlocfilehash: e95246079f8c6e7acffac1dabb278895265767d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835328"
---
# <a name="seektoconditionpageitemview"></a><span data-ttu-id="b3f9f-103">сиктокондитионпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="b3f9f-103">SeekToConditionPageItemView</span></span>

<span data-ttu-id="b3f9f-104">Элемент **сиктокондитионпажеитемвиев** определяет условие, которое используется для определения конца поиска, начального индекса поиска, максимальных возвращаемых записей и инструкций поиска для поиска **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="b3f9f-104">The **SeekToConditionPageItemView** element identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span> 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 <span data-ttu-id="b3f9f-105">**сиктокондитионпажевиевтипе**</span><span class="sxs-lookup"><span data-stu-id="b3f9f-105">**SeekToConditionPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3f9f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b3f9f-106">Attributes and elements</span></span>

<span data-ttu-id="b3f9f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b3f9f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3f9f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b3f9f-108">Attributes</span></span>

|<span data-ttu-id="b3f9f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b3f9f-109">**Attribute**</span></span>|<span data-ttu-id="b3f9f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b3f9f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b3f9f-111">басепоинт</span><span class="sxs-lookup"><span data-stu-id="b3f9f-111">BasePoint</span></span>  <br/> |<span data-ttu-id="b3f9f-112">Текстовое значение атрибута **басепоинт** — это базовая точка, с которой начнется поиск.</span><span class="sxs-lookup"><span data-stu-id="b3f9f-112">The text value of the **BasePoint** attribute is the base point from where the search will start.</span></span> <span data-ttu-id="b3f9f-113">Текстовое значение **start указывает на** то, что поиск начнется с начала набора результатов.</span><span class="sxs-lookup"><span data-stu-id="b3f9f-113">A text value of **Beginning** indicates that the search will start at the beginning of the result set.</span></span> <span data-ttu-id="b3f9f-114">Текстовое значение **End** указывает на то, что поиск начнется в конце набора результатов.</span><span class="sxs-lookup"><span data-stu-id="b3f9f-114">A text value of **End** indicates that the search will start at the end of the result set.</span></span>  <br/> |
|<span data-ttu-id="b3f9f-115">максентриесретурнед</span><span class="sxs-lookup"><span data-stu-id="b3f9f-115">MaxEntriesReturned</span></span>  <br/> |<span data-ttu-id="b3f9f-116">Текстовое значение атрибута **максентриесретурнед** — максимальное количество элементов, которые могут быть возвращены в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="b3f9f-116">The text value of the **MaxEntriesReturned** attribute is the maximum number of items that can be returned in a result set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b3f9f-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b3f9f-117">Child elements</span></span>

[<span data-ttu-id="b3f9f-118">Condition (Рестриктионтипе)</span><span class="sxs-lookup"><span data-stu-id="b3f9f-118">Condition (RestrictionType)</span></span>](condition-restrictiontype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="b3f9f-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b3f9f-119">Parent elements</span></span>

<span data-ttu-id="b3f9f-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span><span class="sxs-lookup"><span data-stu-id="b3f9f-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b3f9f-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="b3f9f-121">Remarks</span></span>

<span data-ttu-id="b3f9f-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b3f9f-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b3f9f-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3f9f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3f9f-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b3f9f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3f9f-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b3f9f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b3f9f-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b3f9f-126">Schema name</span></span>  <br/> |<span data-ttu-id="b3f9f-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b3f9f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b3f9f-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b3f9f-128">Validation file</span></span>  <br/> |<span data-ttu-id="b3f9f-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b3f9f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b3f9f-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b3f9f-130">Can be empty</span></span>  <br/> |<span data-ttu-id="b3f9f-131">false</span><span class="sxs-lookup"><span data-stu-id="b3f9f-131">false</span></span>  <br/> |
   

