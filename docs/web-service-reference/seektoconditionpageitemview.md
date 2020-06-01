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
ms.openlocfilehash: dbb073263740ccdf75367f85f672b7d5ec78f7a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466838"
---
# <a name="seektoconditionpageitemview"></a><span data-ttu-id="11108-103">сиктокондитионпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="11108-103">SeekToConditionPageItemView</span></span>

<span data-ttu-id="11108-104">Элемент **сиктокондитионпажеитемвиев** определяет условие, которое используется для определения конца поиска, начального индекса поиска, максимальных возвращаемых записей и инструкций поиска для поиска **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="11108-104">The **SeekToConditionPageItemView** element identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span> 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 <span data-ttu-id="11108-105">**сиктокондитионпажевиевтипе**</span><span class="sxs-lookup"><span data-stu-id="11108-105">**SeekToConditionPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11108-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="11108-106">Attributes and elements</span></span>

<span data-ttu-id="11108-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="11108-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11108-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="11108-108">Attributes</span></span>

|<span data-ttu-id="11108-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="11108-109">**Attribute**</span></span>|<span data-ttu-id="11108-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11108-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="11108-111">басепоинт</span><span class="sxs-lookup"><span data-stu-id="11108-111">BasePoint</span></span>  <br/> |<span data-ttu-id="11108-112">Текстовое значение атрибута **басепоинт** — это базовая точка, с которой начнется поиск.</span><span class="sxs-lookup"><span data-stu-id="11108-112">The text value of the **BasePoint** attribute is the base point from where the search will start.</span></span> <span data-ttu-id="11108-113">Текстовое значение **start указывает на** то, что поиск начнется с начала набора результатов.</span><span class="sxs-lookup"><span data-stu-id="11108-113">A text value of **Beginning** indicates that the search will start at the beginning of the result set.</span></span> <span data-ttu-id="11108-114">Текстовое значение **End** указывает на то, что поиск начнется в конце набора результатов.</span><span class="sxs-lookup"><span data-stu-id="11108-114">A text value of **End** indicates that the search will start at the end of the result set.</span></span>  <br/> |
|<span data-ttu-id="11108-115">максентриесретурнед</span><span class="sxs-lookup"><span data-stu-id="11108-115">MaxEntriesReturned</span></span>  <br/> |<span data-ttu-id="11108-116">Текстовое значение атрибута **максентриесретурнед** — максимальное количество элементов, которые могут быть возвращены в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="11108-116">The text value of the **MaxEntriesReturned** attribute is the maximum number of items that can be returned in a result set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="11108-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="11108-117">Child elements</span></span>

[<span data-ttu-id="11108-118">Condition (Рестриктионтипе)</span><span class="sxs-lookup"><span data-stu-id="11108-118">Condition (RestrictionType)</span></span>](condition-restrictiontype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="11108-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="11108-119">Parent elements</span></span>

<span data-ttu-id="11108-120">[FindConversation](findconversation.md)  |  [FindItem](finditem.md)</span><span class="sxs-lookup"><span data-stu-id="11108-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="11108-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="11108-121">Remarks</span></span>

<span data-ttu-id="11108-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="11108-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="11108-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="11108-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11108-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="11108-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11108-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="11108-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="11108-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="11108-126">Schema name</span></span>  <br/> |<span data-ttu-id="11108-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="11108-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="11108-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="11108-128">Validation file</span></span>  <br/> |<span data-ttu-id="11108-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="11108-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="11108-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="11108-130">Can be empty</span></span>  <br/> |<span data-ttu-id="11108-131">false</span><span class="sxs-lookup"><span data-stu-id="11108-131">false</span></span>  <br/> |
   

