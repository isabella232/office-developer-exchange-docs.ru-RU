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
ms.openlocfilehash: 00c5b5e615ed9b253c79dae9dc2b89c797853089
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463939"
---
# <a name="condition-restrictiontype"></a><span data-ttu-id="d8f81-103">Condition (Рестриктионтипе)</span><span class="sxs-lookup"><span data-stu-id="d8f81-103">Condition (RestrictionType)</span></span>

<span data-ttu-id="d8f81-104">Элемент **Condition** указывает условие, которое используется для определения конца поиска для операции **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="d8f81-104">The **Condition** element specifies the condition that is used to identify the end of a search for a **FindItem** or a **FindConversation** operation.</span></span> 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 <span data-ttu-id="d8f81-105">**рестриктионтипе**</span><span class="sxs-lookup"><span data-stu-id="d8f81-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8f81-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d8f81-106">Attributes and elements</span></span>

<span data-ttu-id="d8f81-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d8f81-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8f81-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d8f81-108">Attributes</span></span>

<span data-ttu-id="d8f81-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d8f81-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8f81-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d8f81-110">Child elements</span></span>

|<span data-ttu-id="d8f81-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d8f81-111">**Element**</span></span>|<span data-ttu-id="d8f81-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8f81-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8f81-113">сеарчекспрессион</span><span class="sxs-lookup"><span data-stu-id="d8f81-113">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="d8f81-114">Абстрактный элемент, представляющий замененный элемент в ограничении.</span><span class="sxs-lookup"><span data-stu-id="d8f81-114">Abstract element that represents the substituted element within a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8f81-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d8f81-115">Parent elements</span></span>

|<span data-ttu-id="d8f81-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d8f81-116">**Element**</span></span>|<span data-ttu-id="d8f81-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8f81-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8f81-118">сиктокондитионпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="d8f81-118">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="d8f81-119">Определяет условие, используемое для определения конца поиска, начального индекса поиска, максимальных возвращаемых записей и направления поиска для операции **FindItem** или **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="d8f81-119">Identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or a **FindConversation** operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d8f81-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="d8f81-120">Remarks</span></span>

<span data-ttu-id="d8f81-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d8f81-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d8f81-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8f81-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8f81-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d8f81-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8f81-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d8f81-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8f81-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d8f81-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d8f81-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="d8f81-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d8f81-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d8f81-127">Validation File</span></span>  <br/> |<span data-ttu-id="d8f81-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d8f81-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8f81-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d8f81-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d8f81-130">См. также</span><span class="sxs-lookup"><span data-stu-id="d8f81-130">See also</span></span>



- [<span data-ttu-id="d8f81-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d8f81-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

