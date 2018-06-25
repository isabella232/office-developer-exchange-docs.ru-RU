---
title: Имя (отслеживания сообщений)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: a1669f6d-53f3-4849-9b30-56909aaeac82
description: Элемент Name представляет имя свойства для отслеживания отчетов сообщений.
ms.openlocfilehash: c905df03842de47b2bcbd62897aa9a8cf464cc6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834501"
---
# <a name="name-message-tracking"></a><span data-ttu-id="cba45-103">Имя (отслеживания сообщений)</span><span class="sxs-lookup"><span data-stu-id="cba45-103">Name (Message Tracking)</span></span>

<span data-ttu-id="cba45-104">Элемент **Name** представляет имя свойства для отслеживания отчетов сообщений.</span><span class="sxs-lookup"><span data-stu-id="cba45-104">The **Name** element represents the property name for a message tracking report.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="cba45-105">**Строка**</span><span class="sxs-lookup"><span data-stu-id="cba45-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cba45-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cba45-106">Attributes and elements</span></span>

<span data-ttu-id="cba45-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cba45-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cba45-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cba45-108">Attributes</span></span>

<span data-ttu-id="cba45-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="cba45-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cba45-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cba45-110">Child elements</span></span>

<span data-ttu-id="cba45-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="cba45-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cba45-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cba45-112">Parent elements</span></span>

|<span data-ttu-id="cba45-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cba45-113">**Element**</span></span>|<span data-ttu-id="cba45-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cba45-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cba45-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="cba45-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="cba45-116">Представляет имя и значение пары строк, который используется для создания свойств для отчеты об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="cba45-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cba45-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cba45-117">Text value</span></span>

<span data-ttu-id="cba45-118">Текстовое значение является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="cba45-118">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cba45-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="cba45-119">Remarks</span></span>

<span data-ttu-id="cba45-120">Этот элемент может возникнуть только один раз в элементе [TrackingPropertyType](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="cba45-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="cba45-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="cba45-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cba45-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cba45-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cba45-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cba45-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cba45-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cba45-124">Schema Name</span></span>  <br/> |<span data-ttu-id="cba45-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cba45-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="cba45-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cba45-126">Validation File</span></span>  <br/> |<span data-ttu-id="cba45-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cba45-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cba45-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cba45-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="cba45-129">False</span><span class="sxs-lookup"><span data-stu-id="cba45-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cba45-130">См. также</span><span class="sxs-lookup"><span data-stu-id="cba45-130">See also</span></span>

- [<span data-ttu-id="cba45-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cba45-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

