---
title: DeletedOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrence
api_type:
- schema
ms.assetid: ff24ea15-0cd7-407d-a378-73ec16451870
description: Элемент DeletedOccurrence представляет удаленных вхождение повторяющегося элемента календаря.
ms.openlocfilehash: f12a2ba20f87f7803e492d8422b68c8ecdf9d797
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762026"
---
# <a name="deletedoccurrence"></a><span data-ttu-id="03ff2-103">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="03ff2-103">DeletedOccurrence</span></span>

<span data-ttu-id="03ff2-104">Элемент **DeletedOccurrence** представляет удаленных вхождение повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="03ff2-104">The **DeletedOccurrence** element represents a deleted occurrence of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrence>
   <Start/>
</DeletedOccurrence>
```

 <span data-ttu-id="03ff2-105">**DeletedOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="03ff2-105">**DeletedOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03ff2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="03ff2-106">Attributes and elements</span></span>

<span data-ttu-id="03ff2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="03ff2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03ff2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="03ff2-108">Attributes</span></span>

<span data-ttu-id="03ff2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="03ff2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03ff2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="03ff2-110">Child elements</span></span>

|<span data-ttu-id="03ff2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="03ff2-111">**Element**</span></span>|<span data-ttu-id="03ff2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03ff2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03ff2-113">Start</span><span class="sxs-lookup"><span data-stu-id="03ff2-113">Start</span></span>](start.md) <br/> |<span data-ttu-id="03ff2-114">Представляет время начала удаленного вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="03ff2-114">Represents the start time of a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="03ff2-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="03ff2-115">Parent elements</span></span>

|<span data-ttu-id="03ff2-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="03ff2-116">**Element**</span></span>|<span data-ttu-id="03ff2-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03ff2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03ff2-118">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="03ff2-118">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="03ff2-119">Содержит массив удаленных вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="03ff2-119">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="03ff2-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="03ff2-120">Remarks</span></span>

<span data-ttu-id="03ff2-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="03ff2-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03ff2-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="03ff2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03ff2-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="03ff2-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="03ff2-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="03ff2-124">Schema name</span></span>  <br/> |<span data-ttu-id="03ff2-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="03ff2-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="03ff2-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="03ff2-126">Validation file</span></span>  <br/> |<span data-ttu-id="03ff2-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="03ff2-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="03ff2-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="03ff2-128">Can be empty</span></span>  <br/> |<span data-ttu-id="03ff2-129">False</span><span class="sxs-lookup"><span data-stu-id="03ff2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03ff2-130">См. также</span><span class="sxs-lookup"><span data-stu-id="03ff2-130">See also</span></span>

- [<span data-ttu-id="03ff2-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="03ff2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="03ff2-132">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="03ff2-132">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

