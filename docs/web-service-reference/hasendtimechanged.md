---
title: HasEndTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0eb444d-8e2e-478b-b785-2b9787ffb226
description: Элемент HasEndTimeChanged определяет, изменился ли время окончания собрания.
ms.openlocfilehash: 046bb302d6f7052c6f1757ce393583b305311e2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833805"
---
# <a name="hasendtimechanged"></a><span data-ttu-id="f970c-103">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="f970c-103">HasEndTimeChanged</span></span>

<span data-ttu-id="f970c-104">Элемент **HasEndTimeChanged** определяет, изменился ли время окончания собрания.</span><span class="sxs-lookup"><span data-stu-id="f970c-104">The **HasEndTimeChanged** element specifies whether the end time for a meeting has changed.</span></span> 
  
```XML
<HasEndTimeChanged>true | false</HasEndTimeChanged>
```

 <span data-ttu-id="f970c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f970c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f970c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f970c-106">Attributes and elements</span></span>

<span data-ttu-id="f970c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f970c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f970c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f970c-108">Attributes</span></span>

<span data-ttu-id="f970c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f970c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f970c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f970c-110">Child elements</span></span>

<span data-ttu-id="f970c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f970c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f970c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f970c-112">Parent elements</span></span>

|<span data-ttu-id="f970c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f970c-113">**Element**</span></span>|<span data-ttu-id="f970c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f970c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f970c-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="f970c-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="f970c-116">Указывает, что был изменен между двумя версиями собрания сообщение запроса.</span><span class="sxs-lookup"><span data-stu-id="f970c-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f970c-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f970c-117">Text value</span></span>

<span data-ttu-id="f970c-118">Текстовое значение **true** для элемента **HasEndTimeChanged** указывает, что изменилось время окончания собрания.</span><span class="sxs-lookup"><span data-stu-id="f970c-118">A text value of **true** for the **HasEndTimeChanged** element indicates that the end time of a meeting has changed.</span></span> <span data-ttu-id="f970c-119">Значение **false** указывает, что время окончания собрания не был изменен.</span><span class="sxs-lookup"><span data-stu-id="f970c-119">A value of **false** indicates that the end time of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f970c-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="f970c-120">Remarks</span></span>

<span data-ttu-id="f970c-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f970c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f970c-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f970c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f970c-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f970c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f970c-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f970c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f970c-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f970c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f970c-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="f970c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f970c-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f970c-127">Validation File</span></span>  <br/> |<span data-ttu-id="f970c-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f970c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f970c-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f970c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f970c-130">См. также</span><span class="sxs-lookup"><span data-stu-id="f970c-130">See also</span></span>



- [<span data-ttu-id="f970c-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f970c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

