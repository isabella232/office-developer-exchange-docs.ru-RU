---
title: IsMembershipGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: Элемент IsMembershipGroup задает логическое значение, указывающее, является ли объект группы рассылки или почтового ящика.
ms.openlocfilehash: 03ab0dc75d2c798b7f2afeef85aa45f0349be70a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834050"
---
# <a name="ismembershipgroup"></a><span data-ttu-id="7186a-103">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="7186a-103">IsMembershipGroup</span></span>

<span data-ttu-id="7186a-104">Элемент **IsMembershipGroup** задает логическое значение, указывающее, является ли объект группы рассылки или почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7186a-104">The **IsMembershipGroup** element specifies a Boolean value that indicates whether the entity is a distribution group or a mailbox.</span></span> 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
```

 <span data-ttu-id="7186a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7186a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7186a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7186a-106">Attributes and elements</span></span>

<span data-ttu-id="7186a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7186a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7186a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7186a-108">Attributes</span></span>

<span data-ttu-id="7186a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7186a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7186a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7186a-110">Child elements</span></span>

<span data-ttu-id="7186a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7186a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7186a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7186a-112">Parent elements</span></span>

|<span data-ttu-id="7186a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7186a-113">**Element**</span></span>|<span data-ttu-id="7186a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7186a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7186a-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="7186a-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="7186a-116">Указывает почтового ящика возвращаются из **GetSearchableMailboxes** запроса.</span><span class="sxs-lookup"><span data-stu-id="7186a-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7186a-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7186a-117">Text value</span></span>

<span data-ttu-id="7186a-118">Текстовое значение **true** для элемента **IsMembershipGroup** указывает, что сущность является группу рассылки или почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7186a-118">A text value of **true** for the **IsMembershipGroup** element indicates that the entity is a distribution group or a mailbox.</span></span> <span data-ttu-id="7186a-119">Значение false указывает, что объект не является группу рассылки или почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7186a-119">A value of false indicates that the entity is not a distribution group or a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7186a-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="7186a-120">Remarks</span></span>

<span data-ttu-id="7186a-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7186a-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7186a-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7186a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7186a-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7186a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7186a-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7186a-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7186a-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7186a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7186a-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="7186a-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="7186a-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7186a-127">Validation File</span></span>  <br/> |<span data-ttu-id="7186a-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7186a-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7186a-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7186a-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7186a-130">См. также</span><span class="sxs-lookup"><span data-stu-id="7186a-130">See also</span></span>



- [<span data-ttu-id="7186a-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7186a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

