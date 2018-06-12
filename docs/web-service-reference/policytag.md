---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: Элемент PolicyTag указывает идентификатор хранения для элемента или папки.
ms.openlocfilehash: d6cd5aab1145f6006912541c8f8c1d0a91d1e17e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834835"
---
# <a name="policytag"></a><span data-ttu-id="9da36-103">PolicyTag</span><span class="sxs-lookup"><span data-stu-id="9da36-103">PolicyTag</span></span>

<span data-ttu-id="9da36-104">Элемент **PolicyTag** указывает идентификатор хранения для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="9da36-104">The **PolicyTag** element specifies the retention identifier on an item or folder.</span></span> 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 <span data-ttu-id="9da36-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="9da36-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9da36-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9da36-106">Attributes and elements</span></span>

<span data-ttu-id="9da36-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9da36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9da36-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9da36-108">Attributes</span></span>

|<span data-ttu-id="9da36-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="9da36-109">**Attribute**</span></span>|<span data-ttu-id="9da36-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9da36-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9da36-111">IsExplicit</span><span class="sxs-lookup"><span data-stu-id="9da36-111">IsExplicit</span></span>  <br/> |<span data-ttu-id="9da36-112">Указывает, было ли явно задано тег политики на элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="9da36-112">Indicates whether a policy tag was explicitly set on an item or folder.</span></span>  <br/> <span data-ttu-id="9da36-113">Текстовое значение **true** для атрибута **IsExplicit** указывает, что тег политики явно была установлена на элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="9da36-113">A text value of **true** for the **IsExplicit** attribute indicates that the policy tag was explicitly set on the item or folder.</span></span> <span data-ttu-id="9da36-114">Текстовое значение **false** указывает, что тег политики неявно была установлена на элемент или папку на основании тег политики родительской папки.</span><span class="sxs-lookup"><span data-stu-id="9da36-114">A text value of **false** indicates that the policy tag was implicitly set on the item or folder based on the parent folder policy tag.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9da36-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9da36-115">Child elements</span></span>

<span data-ttu-id="9da36-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="9da36-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9da36-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9da36-117">Parent elements</span></span>

<span data-ttu-id="9da36-118">[SearchPreviewItem](searchpreviewitem.md) | [элемента](item.md) | [контакт](contact.md) | [сообщение](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [элемента календаря, имеющего](calendaritem.md) | [PostItem](postitem.md) | [задач](task.md)</span><span class="sxs-lookup"><span data-stu-id="9da36-118">[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9da36-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9da36-119">Text value</span></span>

<span data-ttu-id="9da36-120">Текстовое значение элемента **PolicyTag** является идентификатором тег политики.</span><span class="sxs-lookup"><span data-stu-id="9da36-120">The text value of the **PolicyTag** element is the policy tag identifier.</span></span> <span data-ttu-id="9da36-121">Идентификатор тега политики — это GUID.</span><span class="sxs-lookup"><span data-stu-id="9da36-121">The policy tag identifier is a GUID.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9da36-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="9da36-122">Remarks</span></span>

<span data-ttu-id="9da36-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9da36-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9da36-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9da36-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9da36-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9da36-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9da36-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9da36-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9da36-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9da36-127">Schema name</span></span>  <br/> |<span data-ttu-id="9da36-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9da36-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="9da36-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9da36-129">Validation file</span></span>  <br/> |<span data-ttu-id="9da36-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9da36-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9da36-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9da36-131">Can be empty</span></span>  <br/> ||
   

