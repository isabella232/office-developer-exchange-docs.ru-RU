---
title: DeleteFromFolderStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3aba59a0-f12a-48b5-842b-11cf4530dd51
description: Элемент DeleteFromFolderStateDefinition указывает состояние, когда элемент удаляется из папки.
ms.openlocfilehash: 7b6374b9fa55d3b08569e8ac9e247dd6e5bebc24
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762039"
---
# <a name="deletefromfolderstatedefinition"></a><span data-ttu-id="7953c-103">DeleteFromFolderStateDefinition</span><span class="sxs-lookup"><span data-stu-id="7953c-103">DeleteFromFolderStateDefinition</span></span>

<span data-ttu-id="7953c-104">Элемент **DeleteFromFolderStateDefinition** указывает состояние, когда элемент удаляется из папки.</span><span class="sxs-lookup"><span data-stu-id="7953c-104">The **DeleteFromFolderStateDefinition** element specifies the state when an item is deleted from a folder.</span></span> 
  
```XML
<DeleteFromFolderStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeleteFromFolderStateDefinition>
```

 <span data-ttu-id="7953c-105">**DeleteFromFolderStateDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="7953c-105">**DeleteFromFolderStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7953c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7953c-106">Attributes and elements</span></span>

<span data-ttu-id="7953c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7953c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7953c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7953c-108">Attributes</span></span>

<span data-ttu-id="7953c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7953c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7953c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7953c-110">Child elements</span></span>

|<span data-ttu-id="7953c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7953c-111">**Element**</span></span>|<span data-ttu-id="7953c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7953c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7953c-113">Вхождение (часовой пояс переходов)</span><span class="sxs-lookup"><span data-stu-id="7953c-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="7953c-114">Указывает дату вхождение элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="7953c-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7953c-115">IsOccurrencePresent</span><span class="sxs-lookup"><span data-stu-id="7953c-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="7953c-116">Задает логическое значение, которое указывает наличие вхождения элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="7953c-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7953c-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7953c-117">Parent elements</span></span>

|<span data-ttu-id="7953c-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7953c-118">**Element**</span></span>|<span data-ttu-id="7953c-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7953c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7953c-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="7953c-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="7953c-121">Задает определение состояний.</span><span class="sxs-lookup"><span data-stu-id="7953c-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7953c-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="7953c-122">Remarks</span></span>

<span data-ttu-id="7953c-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7953c-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7953c-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7953c-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7953c-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7953c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7953c-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7953c-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7953c-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7953c-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7953c-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="7953c-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="7953c-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7953c-129">Validation File</span></span>  <br/> |<span data-ttu-id="7953c-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7953c-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7953c-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7953c-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7953c-132">См. также</span><span class="sxs-lookup"><span data-stu-id="7953c-132">See also</span></span>

- [<span data-ttu-id="7953c-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7953c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

