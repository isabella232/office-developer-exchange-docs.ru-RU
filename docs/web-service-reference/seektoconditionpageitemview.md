---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: Элемент SeekToConditionPageItemView определяет условие, используемое для идентификации в конце поиска, начальный индекс поиска, максимальное записей для возвращения и указания поиска для поиска FindItem или FindConversation.
ms.openlocfilehash: e95246079f8c6e7acffac1dabb278895265767d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835328"
---
# <a name="seektoconditionpageitemview"></a><span data-ttu-id="98e4a-103">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="98e4a-103">SeekToConditionPageItemView</span></span>

<span data-ttu-id="98e4a-104">Элемент **SeekToConditionPageItemView** определяет условие, используемое для идентификации в конце поиска, начальный индекс поиска, максимальное записей для возвращения и указания поиска для **FindItem** или **FindConversation **поиска.</span><span class="sxs-lookup"><span data-stu-id="98e4a-104">The **SeekToConditionPageItemView** element identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span> 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 <span data-ttu-id="98e4a-105">**SeekToConditionPageViewType**</span><span class="sxs-lookup"><span data-stu-id="98e4a-105">**SeekToConditionPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98e4a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="98e4a-106">Attributes and elements</span></span>

<span data-ttu-id="98e4a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="98e4a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98e4a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="98e4a-108">Attributes</span></span>

|<span data-ttu-id="98e4a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="98e4a-109">**Attribute**</span></span>|<span data-ttu-id="98e4a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="98e4a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="98e4a-111">Базисная точка</span><span class="sxs-lookup"><span data-stu-id="98e4a-111">BasePoint</span></span>  <br/> |<span data-ttu-id="98e4a-112">Текстовое значение атрибута **Базисная точка** точка базовый, из которой будет начинаться поиск.</span><span class="sxs-lookup"><span data-stu-id="98e4a-112">The text value of the **BasePoint** attribute is the base point from where the search will start.</span></span> <span data-ttu-id="98e4a-113">Текстовое значение **начала** указывает, что поиск начнется в начале набора результатов.</span><span class="sxs-lookup"><span data-stu-id="98e4a-113">A text value of **Beginning** indicates that the search will start at the beginning of the result set.</span></span> <span data-ttu-id="98e4a-114">Текстовое значение **End** указывает, что поиск начинается в конце набора результатов.</span><span class="sxs-lookup"><span data-stu-id="98e4a-114">A text value of **End** indicates that the search will start at the end of the result set.</span></span>  <br/> |
|<span data-ttu-id="98e4a-115">MaxEntriesReturned</span><span class="sxs-lookup"><span data-stu-id="98e4a-115">MaxEntriesReturned</span></span>  <br/> |<span data-ttu-id="98e4a-116">Текстовое значение атрибута **MaxEntriesReturned** — это максимальное число элементов, которые могут возвращаться в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="98e4a-116">The text value of the **MaxEntriesReturned** attribute is the maximum number of items that can be returned in a result set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="98e4a-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="98e4a-117">Child elements</span></span>

[<span data-ttu-id="98e4a-118">Условие (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="98e4a-118">Condition (RestrictionType)</span></span>](condition-restrictiontype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="98e4a-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="98e4a-119">Parent elements</span></span>

<span data-ttu-id="98e4a-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span><span class="sxs-lookup"><span data-stu-id="98e4a-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="98e4a-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="98e4a-121">Remarks</span></span>

<span data-ttu-id="98e4a-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="98e4a-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="98e4a-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="98e4a-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98e4a-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="98e4a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98e4a-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="98e4a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="98e4a-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="98e4a-126">Schema name</span></span>  <br/> |<span data-ttu-id="98e4a-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="98e4a-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="98e4a-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="98e4a-128">Validation file</span></span>  <br/> |<span data-ttu-id="98e4a-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="98e4a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="98e4a-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="98e4a-130">Can be empty</span></span>  <br/> |<span data-ttu-id="98e4a-131">Нет</span><span class="sxs-lookup"><span data-stu-id="98e4a-131">false</span></span>  <br/> |
   

