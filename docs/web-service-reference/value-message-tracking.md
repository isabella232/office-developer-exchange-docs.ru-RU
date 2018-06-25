---
title: Значение (отслеживания сообщений)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: cb2f228f-775a-4c7d-82e7-41c7c953c808
description: Элемент Value представляет значение свойства для отслеживания отчетов сообщений.
ms.openlocfilehash: 152e4fe61a4cff8013ae02900bd84bf244ae84a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840460"
---
# <a name="value-message-tracking"></a><span data-ttu-id="26b42-103">Значение (отслеживания сообщений)</span><span class="sxs-lookup"><span data-stu-id="26b42-103">Value (Message Tracking)</span></span>

<span data-ttu-id="26b42-104">Элемент **Value** представляет значение свойства для отслеживания отчетов сообщений.</span><span class="sxs-lookup"><span data-stu-id="26b42-104">The **Value** element represents the property value for a message tracking report.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="26b42-105">**Строка**</span><span class="sxs-lookup"><span data-stu-id="26b42-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="26b42-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="26b42-106">Attributes and elements</span></span>

<span data-ttu-id="26b42-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="26b42-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26b42-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="26b42-108">Attributes</span></span>

<span data-ttu-id="26b42-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="26b42-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26b42-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="26b42-110">Child elements</span></span>

<span data-ttu-id="26b42-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="26b42-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26b42-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="26b42-112">Parent elements</span></span>

|<span data-ttu-id="26b42-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="26b42-113">**Element**</span></span>|<span data-ttu-id="26b42-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="26b42-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26b42-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="26b42-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="26b42-116">Представляет имя и значение пары строк, который используется для создания свойств для отчеты об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="26b42-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="26b42-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="26b42-117">Text value</span></span>

<span data-ttu-id="26b42-118">Текстовое значение является необязательным.</span><span class="sxs-lookup"><span data-stu-id="26b42-118">The text value is optional.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="26b42-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="26b42-119">Remarks</span></span>

<span data-ttu-id="26b42-120">Этот элемент может возникнуть только один раз в элементе [TrackingPropertyType](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="26b42-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="26b42-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="26b42-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26b42-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="26b42-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26b42-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="26b42-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26b42-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="26b42-124">Schema Name</span></span>  <br/> |<span data-ttu-id="26b42-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="26b42-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="26b42-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="26b42-126">Validation File</span></span>  <br/> |<span data-ttu-id="26b42-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="26b42-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26b42-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="26b42-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="26b42-129">False</span><span class="sxs-lookup"><span data-stu-id="26b42-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26b42-130">См. также</span><span class="sxs-lookup"><span data-stu-id="26b42-130">See also</span></span>

- [<span data-ttu-id="26b42-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="26b42-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

