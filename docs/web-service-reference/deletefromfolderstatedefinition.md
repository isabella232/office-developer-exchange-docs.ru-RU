---
title: делетефромфолдерстатедефинитион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3aba59a0-f12a-48b5-842b-11cf4530dd51
description: Элемент Делетефромфолдерстатедефинитион указывает состояние при удалении элемента из папки.
ms.openlocfilehash: 0ea8c61a6839790869781d5d87ca81772b2e38d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455725"
---
# <a name="deletefromfolderstatedefinition"></a><span data-ttu-id="97df4-103">делетефромфолдерстатедефинитион</span><span class="sxs-lookup"><span data-stu-id="97df4-103">DeleteFromFolderStateDefinition</span></span>

<span data-ttu-id="97df4-104">Элемент **делетефромфолдерстатедефинитион** указывает состояние при удалении элемента из папки.</span><span class="sxs-lookup"><span data-stu-id="97df4-104">The **DeleteFromFolderStateDefinition** element specifies the state when an item is deleted from a folder.</span></span> 
  
```XML
<DeleteFromFolderStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeleteFromFolderStateDefinition>
```

 <span data-ttu-id="97df4-105">**делетефромфолдерстатедефинитионтипе**</span><span class="sxs-lookup"><span data-stu-id="97df4-105">**DeleteFromFolderStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97df4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="97df4-106">Attributes and elements</span></span>

<span data-ttu-id="97df4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="97df4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97df4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="97df4-108">Attributes</span></span>

<span data-ttu-id="97df4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97df4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97df4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="97df4-110">Child elements</span></span>

|<span data-ttu-id="97df4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="97df4-111">**Element**</span></span>|<span data-ttu-id="97df4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97df4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97df4-113">Вхождение (переход часового пояса)</span><span class="sxs-lookup"><span data-stu-id="97df4-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="97df4-114">Указывает дату вхождения элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="97df4-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="97df4-115">исоккурренцепресент</span><span class="sxs-lookup"><span data-stu-id="97df4-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="97df4-116">Задает логическое значение, указывающее, присутствует ли экземпляр элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="97df4-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97df4-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="97df4-117">Parent elements</span></span>

|<span data-ttu-id="97df4-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="97df4-118">**Element**</span></span>|<span data-ttu-id="97df4-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97df4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97df4-120">статедефинитион</span><span class="sxs-lookup"><span data-stu-id="97df4-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="97df4-121">Задает определение состояния.</span><span class="sxs-lookup"><span data-stu-id="97df4-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97df4-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="97df4-122">Remarks</span></span>

<span data-ttu-id="97df4-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="97df4-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="97df4-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="97df4-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97df4-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="97df4-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97df4-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="97df4-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97df4-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="97df4-127">Schema Name</span></span>  <br/> |<span data-ttu-id="97df4-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="97df4-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="97df4-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="97df4-129">Validation File</span></span>  <br/> |<span data-ttu-id="97df4-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="97df4-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="97df4-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="97df4-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="97df4-132">См. также</span><span class="sxs-lookup"><span data-stu-id="97df4-132">See also</span></span>

- [<span data-ttu-id="97df4-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="97df4-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

