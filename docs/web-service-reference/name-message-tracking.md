---
title: Name (отслеживание сообщений)
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
description: Элемент Name представляет имя свойства для отчета об отслеживании сообщений.
ms.openlocfilehash: 86f049c0a90dbeb55418a5eee58079adf17e5ded
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466901"
---
# <a name="name-message-tracking"></a><span data-ttu-id="26310-103">Name (отслеживание сообщений)</span><span class="sxs-lookup"><span data-stu-id="26310-103">Name (Message Tracking)</span></span>

<span data-ttu-id="26310-104">Элемент **Name** представляет имя свойства для отчета об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="26310-104">The **Name** element represents the property name for a message tracking report.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="26310-105">**String**</span><span class="sxs-lookup"><span data-stu-id="26310-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="26310-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="26310-106">Attributes and elements</span></span>

<span data-ttu-id="26310-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="26310-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26310-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="26310-108">Attributes</span></span>

<span data-ttu-id="26310-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="26310-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26310-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="26310-110">Child elements</span></span>

<span data-ttu-id="26310-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="26310-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26310-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="26310-112">Parent elements</span></span>

|<span data-ttu-id="26310-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="26310-113">**Element**</span></span>|<span data-ttu-id="26310-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="26310-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26310-115">траккингпропертитипе</span><span class="sxs-lookup"><span data-stu-id="26310-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="26310-116">Представляет строку имени и значения, используемую для создания свойств отчетов об отслеживании сообщений.</span><span class="sxs-lookup"><span data-stu-id="26310-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="26310-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="26310-117">Text value</span></span>

<span data-ttu-id="26310-118">При использовании этого элемента необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="26310-118">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="26310-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="26310-119">Remarks</span></span>

<span data-ttu-id="26310-120">Этот элемент может встречаться не более одного раз в элементе [траккингпропертитипе](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="26310-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="26310-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="26310-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26310-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="26310-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26310-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="26310-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26310-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="26310-124">Schema Name</span></span>  <br/> |<span data-ttu-id="26310-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="26310-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="26310-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="26310-126">Validation File</span></span>  <br/> |<span data-ttu-id="26310-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="26310-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26310-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="26310-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="26310-129">False</span><span class="sxs-lookup"><span data-stu-id="26310-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26310-130">См. также</span><span class="sxs-lookup"><span data-stu-id="26310-130">See also</span></span>

- [<span data-ttu-id="26310-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="26310-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

