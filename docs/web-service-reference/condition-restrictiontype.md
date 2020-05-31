---
title: Condition (Рестриктионтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdb373e-bf1b-4cb0-bbfb-444c6c6cec50
description: Элемент Condition указывает условие, которое используется для определения конца поиска для операции FindItem или FindConversation.
ms.openlocfilehash: 513fc21be52a90698f1c292d6d20d7cdaab07371
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761704"
---
# <a name="condition-restrictiontype"></a><span data-ttu-id="bc6c4-103">Condition (Рестриктионтипе)</span><span class="sxs-lookup"><span data-stu-id="bc6c4-103">Condition (RestrictionType)</span></span>

<span data-ttu-id="bc6c4-104">Элемент **Condition** указывает условие, которое используется для определения конца поиска для операции **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="bc6c4-104">The **Condition** element specifies the condition that is used to identify the end of a search for a **FindItem** or a **FindConversation** operation.</span></span> 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 <span data-ttu-id="bc6c4-105">**рестриктионтипе**</span><span class="sxs-lookup"><span data-stu-id="bc6c4-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc6c4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc6c4-106">Attributes and elements</span></span>

<span data-ttu-id="bc6c4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bc6c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc6c4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc6c4-108">Attributes</span></span>

<span data-ttu-id="bc6c4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc6c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc6c4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc6c4-110">Child elements</span></span>

|<span data-ttu-id="bc6c4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc6c4-111">**Element**</span></span>|<span data-ttu-id="bc6c4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc6c4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc6c4-113">сеарчекспрессион</span><span class="sxs-lookup"><span data-stu-id="bc6c4-113">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="bc6c4-114">Абстрактный элемент, представляющий замененный элемент в ограничении.</span><span class="sxs-lookup"><span data-stu-id="bc6c4-114">Abstract element that represents the substituted element within a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc6c4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc6c4-115">Parent elements</span></span>

|<span data-ttu-id="bc6c4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc6c4-116">**Element**</span></span>|<span data-ttu-id="bc6c4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc6c4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc6c4-118">сиктокондитионпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="bc6c4-118">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="bc6c4-119">Определяет условие, используемое для определения конца поиска, начального индекса поиска, максимальных возвращаемых записей и направления поиска для операции **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="bc6c4-119">Identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or a **FindConversation** operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bc6c4-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="bc6c4-120">Remarks</span></span>

<span data-ttu-id="bc6c4-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bc6c4-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bc6c4-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc6c4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc6c4-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc6c4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc6c4-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc6c4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc6c4-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc6c4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="bc6c4-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="bc6c4-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="bc6c4-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc6c4-127">Validation File</span></span>  <br/> |<span data-ttu-id="bc6c4-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bc6c4-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc6c4-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc6c4-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bc6c4-130">См. также</span><span class="sxs-lookup"><span data-stu-id="bc6c4-130">See also</span></span>



- [<span data-ttu-id="bc6c4-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc6c4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

