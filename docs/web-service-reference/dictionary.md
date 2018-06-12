---
title: словаря
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Dictionary
api_type:
- schema
ms.assetid: 8309e468-115b-4d6e-b33c-c4719dcecc4c
description: Элемент Dictionary определяет набор записи словаря свойства для объекта конфигурации пользователя.
ms.openlocfilehash: 151abfe7a9a9ae05b8b61af87c33675e025920ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762093"
---
# <a name="dictionary"></a><span data-ttu-id="d42fe-103">словаря</span><span class="sxs-lookup"><span data-stu-id="d42fe-103">Dictionary</span></span>

<span data-ttu-id="d42fe-104">Элемент **Dictionary** определяет набор записи словаря свойства для объекта конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="d42fe-104">The **Dictionary** element defines a set of dictionary property entries for a user configuration object.</span></span> 
  
```xml
<Dictionary>
   <DictionaryEntry/>
</Dictionary>
```

 <span data-ttu-id="d42fe-105">**UserConfigurationDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="d42fe-105">**UserConfigurationDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d42fe-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d42fe-106">Attributes and elements</span></span>

<span data-ttu-id="d42fe-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d42fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d42fe-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d42fe-108">Attributes</span></span>

<span data-ttu-id="d42fe-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d42fe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d42fe-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d42fe-110">Child elements</span></span>

|<span data-ttu-id="d42fe-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d42fe-111">**Element**</span></span>|<span data-ttu-id="d42fe-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d42fe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d42fe-113">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="d42fe-113">DictionaryEntry</span></span>](dictionaryentry.md) <br/> |<span data-ttu-id="d42fe-114">Задает содержимое свойства запись одного словаря.</span><span class="sxs-lookup"><span data-stu-id="d42fe-114">Specifies the contents of a single dictionary entry property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d42fe-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d42fe-115">Parent elements</span></span>

|<span data-ttu-id="d42fe-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d42fe-116">**Element**</span></span>|<span data-ttu-id="d42fe-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d42fe-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d42fe-118">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="d42fe-118">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="d42fe-119">Определяет объект конфигурации одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d42fe-119">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d42fe-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d42fe-120">Text value</span></span>

<span data-ttu-id="d42fe-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="d42fe-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d42fe-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="d42fe-122">Remarks</span></span>

<span data-ttu-id="d42fe-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d42fe-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d42fe-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d42fe-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d42fe-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d42fe-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d42fe-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d42fe-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d42fe-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d42fe-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="d42fe-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d42fe-128">Validation File</span></span>  <br/> |<span data-ttu-id="d42fe-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d42fe-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d42fe-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d42fe-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d42fe-131">False</span><span class="sxs-lookup"><span data-stu-id="d42fe-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d42fe-132">См. также</span><span class="sxs-lookup"><span data-stu-id="d42fe-132">See also</span></span>

- [<span data-ttu-id="d42fe-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d42fe-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

