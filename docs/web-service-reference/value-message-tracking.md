---
title: Value (отслеживание сообщений)
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
description: Элемент value представляет значение свойства для отчета об отслеживании сообщений.
ms.openlocfilehash: 152e4fe61a4cff8013ae02900bd84bf244ae84a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840460"
---
# <a name="value-message-tracking"></a><span data-ttu-id="cedb5-103">Value (отслеживание сообщений)</span><span class="sxs-lookup"><span data-stu-id="cedb5-103">Value (Message Tracking)</span></span>

<span data-ttu-id="cedb5-104">Элемент **value** представляет значение свойства для отчета об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="cedb5-104">The **Value** element represents the property value for a message tracking report.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="cedb5-105">**String**</span><span class="sxs-lookup"><span data-stu-id="cedb5-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cedb5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cedb5-106">Attributes and elements</span></span>

<span data-ttu-id="cedb5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cedb5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cedb5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cedb5-108">Attributes</span></span>

<span data-ttu-id="cedb5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="cedb5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cedb5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cedb5-110">Child elements</span></span>

<span data-ttu-id="cedb5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="cedb5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cedb5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cedb5-112">Parent elements</span></span>

|<span data-ttu-id="cedb5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cedb5-113">**Element**</span></span>|<span data-ttu-id="cedb5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cedb5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cedb5-115">траккингпропертитипе</span><span class="sxs-lookup"><span data-stu-id="cedb5-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="cedb5-116">Представляет строку имени и значения, используемую для создания свойств отчетов об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="cedb5-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cedb5-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cedb5-117">Text value</span></span>

<span data-ttu-id="cedb5-118">Значение Text является необязательным.</span><span class="sxs-lookup"><span data-stu-id="cedb5-118">The text value is optional.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cedb5-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="cedb5-119">Remarks</span></span>

<span data-ttu-id="cedb5-120">Этот элемент может встречаться не более одного раз в элементе [траккингпропертитипе](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="cedb5-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="cedb5-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="cedb5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cedb5-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cedb5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cedb5-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cedb5-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cedb5-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cedb5-124">Schema Name</span></span>  <br/> |<span data-ttu-id="cedb5-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cedb5-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="cedb5-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cedb5-126">Validation File</span></span>  <br/> |<span data-ttu-id="cedb5-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cedb5-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cedb5-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cedb5-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="cedb5-129">False</span><span class="sxs-lookup"><span data-stu-id="cedb5-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cedb5-130">См. также</span><span class="sxs-lookup"><span data-stu-id="cedb5-130">See also</span></span>

- [<span data-ttu-id="cedb5-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cedb5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

