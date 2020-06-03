---
title: Рекуррингмастеритемид (Итемидтипе)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: Элемент Рекуррингмастеритемид (Итемидтипе) идентифицирует элемент шаблона повторения, определяя идентификаторы одного из связанных элементов вхождения.
ms.openlocfilehash: c725998ad3a728ef1f47ff6491592b461753b895
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468441"
---
# <a name="recurringmasteritemid-itemidtype"></a><span data-ttu-id="033d1-103">Рекуррингмастеритемид (Итемидтипе)</span><span class="sxs-lookup"><span data-stu-id="033d1-103">RecurringMasterItemId (ItemIdType)</span></span>

<span data-ttu-id="033d1-104">Элемент **рекуррингмастеритемид (итемидтипе)** идентифицирует элемент шаблона повторения, определяя идентификаторы одного из связанных элементов вхождения.</span><span class="sxs-lookup"><span data-stu-id="033d1-104">The **RecurringMasterItemId (ItemIdType)** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="033d1-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="033d1-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="033d1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="033d1-106">Attributes and elements</span></span>

<span data-ttu-id="033d1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="033d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="033d1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="033d1-108">Attributes</span></span>

****

|<span data-ttu-id="033d1-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="033d1-109">**Attribute**</span></span>|<span data-ttu-id="033d1-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="033d1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="033d1-111">Id</span><span class="sxs-lookup"><span data-stu-id="033d1-111">Id</span></span>  <br/> |<span data-ttu-id="033d1-112">Определяет один экземпляр повторяющегося элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="033d1-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="033d1-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="033d1-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="033d1-114">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="033d1-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="033d1-115">Определяет конкретную версию одного экземпляра повторяющегося элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="033d1-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="033d1-116">Кроме того, также идентифицируется шаблон повторяющегося элемента, так как он и один экземпляр будут содержать один и тот же ключ изменения.</span><span class="sxs-lookup"><span data-stu-id="033d1-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="033d1-117">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="033d1-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="033d1-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="033d1-118">Child elements</span></span>

<span data-ttu-id="033d1-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="033d1-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="033d1-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="033d1-120">Parent elements</span></span>

[<span data-ttu-id="033d1-121">Reminder</span><span class="sxs-lookup"><span data-stu-id="033d1-121">Reminder</span></span>](reminder.md)
  
## <a name="remarks"></a><span data-ttu-id="033d1-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="033d1-122">Remarks</span></span>

<span data-ttu-id="033d1-123">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="033d1-123">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="033d1-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="033d1-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="033d1-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="033d1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="033d1-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="033d1-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="033d1-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="033d1-127">Schema Name</span></span>  <br/> |<span data-ttu-id="033d1-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="033d1-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="033d1-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="033d1-129">Validation File</span></span>  <br/> |<span data-ttu-id="033d1-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="033d1-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="033d1-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="033d1-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="033d1-132">True</span><span class="sxs-lookup"><span data-stu-id="033d1-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="033d1-133">См. также</span><span class="sxs-lookup"><span data-stu-id="033d1-133">See also</span></span>



[<span data-ttu-id="033d1-134">Reminder</span><span class="sxs-lookup"><span data-stu-id="033d1-134">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="033d1-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="033d1-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

