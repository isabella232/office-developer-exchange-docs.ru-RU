---
title: Константа
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Constant
api_type:
- schema
ms.assetid: 340af0cd-9f12-44ab-b8f1-21d107c8d0c9
description: Элемент Constant определяет константное значение в ограничении.
ms.openlocfilehash: 6cb2eaa4227a8fd0985e8ff5a15d647c3bb1cd6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461557"
---
# <a name="constant"></a><span data-ttu-id="91178-103">Константа</span><span class="sxs-lookup"><span data-stu-id="91178-103">Constant</span></span>

<span data-ttu-id="91178-104">Элемент **Constant** определяет константное значение в ограничении.</span><span class="sxs-lookup"><span data-stu-id="91178-104">The **Constant** element identifies a constant value in a restriction.</span></span> 
  
```xml
<Constant Value="" />
```

 <span data-ttu-id="91178-105">**константвалуетипе**</span><span class="sxs-lookup"><span data-stu-id="91178-105">**ConstantValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91178-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="91178-106">Attributes and elements</span></span>

<span data-ttu-id="91178-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="91178-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91178-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="91178-108">Attributes</span></span>

|<span data-ttu-id="91178-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="91178-109">**Attribute**</span></span>|<span data-ttu-id="91178-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="91178-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="91178-111">**Значение**</span><span class="sxs-lookup"><span data-stu-id="91178-111">**Value**</span></span> <br/> |<span data-ttu-id="91178-112">Указывает значение, которое требуется сравнить в ограничении.</span><span class="sxs-lookup"><span data-stu-id="91178-112">Specifies the value to compare in the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="91178-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="91178-113">Child elements</span></span>

<span data-ttu-id="91178-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="91178-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91178-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="91178-115">Parent elements</span></span>

|<span data-ttu-id="91178-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="91178-116">**Element**</span></span>|<span data-ttu-id="91178-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="91178-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91178-118">Contains</span><span class="sxs-lookup"><span data-stu-id="91178-118">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="91178-119">Представляет выражение поиска, которое определяет, содержит ли данное свойство предоставленное строковое значение константы.</span><span class="sxs-lookup"><span data-stu-id="91178-119">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="91178-120">фиелдуриорконстант</span><span class="sxs-lookup"><span data-stu-id="91178-120">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="91178-121">Представляет свойство или значение константы, которое будет использоваться при сравнении с другим свойством.</span><span class="sxs-lookup"><span data-stu-id="91178-121">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="91178-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="91178-122">Remarks</span></span>

<span data-ttu-id="91178-123">Строковое значение в атрибуте **value** должно быть приводимым к типу, с которым выполняется сравнение.</span><span class="sxs-lookup"><span data-stu-id="91178-123">The string value in the **Value** attribute must be coercible into the type you are trying to compare against.</span></span> <span data-ttu-id="91178-124">Например, если вы сравниваете свойство Date/Time со значением константы, строковое значение должно представлять дату и время.</span><span class="sxs-lookup"><span data-stu-id="91178-124">For example, if you are comparing a date/time property against a constant value, the string value must represent a date/time.</span></span> 
  
<span data-ttu-id="91178-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="91178-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91178-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="91178-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91178-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="91178-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91178-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="91178-128">Schema Name</span></span>  <br/> |<span data-ttu-id="91178-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="91178-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="91178-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="91178-130">Validation File</span></span>  <br/> |<span data-ttu-id="91178-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="91178-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91178-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="91178-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="91178-133">False</span><span class="sxs-lookup"><span data-stu-id="91178-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91178-134">См. также</span><span class="sxs-lookup"><span data-stu-id="91178-134">See also</span></span>



- [<span data-ttu-id="91178-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="91178-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

