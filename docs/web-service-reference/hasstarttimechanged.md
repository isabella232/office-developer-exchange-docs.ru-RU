---
title: HasStartTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04a6968d-7fb5-47ee-b66e-dc99c35dbb63
description: Элемент HasStartTimeChanged определяет, изменился ли время начала собрания.
ms.openlocfilehash: 2096084f4ec8848a63d10e0e80fdc7a37e473cd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833809"
---
# <a name="hasstarttimechanged"></a><span data-ttu-id="c26b4-103">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="c26b4-103">HasStartTimeChanged</span></span>

<span data-ttu-id="c26b4-104">Элемент **HasStartTimeChanged** определяет, изменился ли время начала собрания.</span><span class="sxs-lookup"><span data-stu-id="c26b4-104">The **HasStartTimeChanged** element specifies whether the start time for a meeting has changed.</span></span> 
  
```XML
<HasStartTimeChanged> true | false </HasStartTimeChanged>
```

 <span data-ttu-id="c26b4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c26b4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c26b4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c26b4-106">Attributes and elements</span></span>

<span data-ttu-id="c26b4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c26b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c26b4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c26b4-108">Attributes</span></span>

<span data-ttu-id="c26b4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c26b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c26b4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c26b4-110">Child elements</span></span>

<span data-ttu-id="c26b4-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c26b4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c26b4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c26b4-112">Parent elements</span></span>

|<span data-ttu-id="c26b4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c26b4-113">**Element**</span></span>|<span data-ttu-id="c26b4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c26b4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c26b4-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="c26b4-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="c26b4-116">Указывает, что был изменен между двумя версиями собрания сообщение запроса.</span><span class="sxs-lookup"><span data-stu-id="c26b4-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c26b4-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c26b4-117">Text value</span></span>

<span data-ttu-id="c26b4-118">Текстовое значение **true** для элемента **HasStartTimeChanged** указывает, что время начала собрания был изменен.</span><span class="sxs-lookup"><span data-stu-id="c26b4-118">A text value of **true** for the **HasStartTimeChanged** element indicates that the start time for a meeting has changed.</span></span> <span data-ttu-id="c26b4-119">Значение **false** указывает, что, который еще не был изменен время начала.</span><span class="sxs-lookup"><span data-stu-id="c26b4-119">A value of **false** indicates that the start time has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c26b4-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="c26b4-120">Remarks</span></span>

<span data-ttu-id="c26b4-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c26b4-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c26b4-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c26b4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c26b4-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c26b4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c26b4-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c26b4-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c26b4-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c26b4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c26b4-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="c26b4-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="c26b4-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c26b4-127">Validation File</span></span>  <br/> |<span data-ttu-id="c26b4-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c26b4-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c26b4-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c26b4-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c26b4-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c26b4-130">See also</span></span>



- [<span data-ttu-id="c26b4-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c26b4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

