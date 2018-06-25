---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: Элемент MakeItemImmutable задает логическое значение, указывающее, является ли элемент должна создаваться только для чтения.
ms.openlocfilehash: 63c05fd3572c7b4ab93fe098d9165a117849ef02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834337"
---
# <a name="makeitemimmutable"></a><span data-ttu-id="124c6-103">MakeItemImmutable</span><span class="sxs-lookup"><span data-stu-id="124c6-103">MakeItemImmutable</span></span>

<span data-ttu-id="124c6-104">Элемент **MakeItemImmutable** задает логическое значение, указывающее, является ли элемент должна создаваться только для чтения.</span><span class="sxs-lookup"><span data-stu-id="124c6-104">The **MakeItemImmutable** element specifies a Boolean value that indicates whether an item should be made read-only.</span></span> 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 <span data-ttu-id="124c6-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="124c6-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="124c6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="124c6-106">Attributes and elements</span></span>

<span data-ttu-id="124c6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="124c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="124c6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="124c6-108">Attributes</span></span>

<span data-ttu-id="124c6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="124c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="124c6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="124c6-110">Child elements</span></span>

<span data-ttu-id="124c6-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="124c6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="124c6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="124c6-112">Parent elements</span></span>

[<span data-ttu-id="124c6-113">UpdateItemInRecoverableItems</span><span class="sxs-lookup"><span data-stu-id="124c6-113">UpdateItemInRecoverableItems</span></span>](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a><span data-ttu-id="124c6-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="124c6-114">Text value</span></span>

<span data-ttu-id="124c6-115">Текстовое значение **true** для элемента **MakeItemImmutable** указывает, что элемент должна создаваться только для чтения.</span><span class="sxs-lookup"><span data-stu-id="124c6-115">A text value of **true** for the **MakeItemImmutable** element indicates that the item should be made read-only.</span></span> <span data-ttu-id="124c6-116">Значение **false** указывает, что элемент разрешает доступ на чтение запись.</span><span class="sxs-lookup"><span data-stu-id="124c6-116">A value of **false** indicates that the item allows read-write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="124c6-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="124c6-117">Remarks</span></span>

<span data-ttu-id="124c6-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="124c6-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="124c6-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="124c6-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="124c6-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="124c6-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="124c6-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="124c6-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="124c6-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="124c6-122">Schema name</span></span>  <br/> |<span data-ttu-id="124c6-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="124c6-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="124c6-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="124c6-124">Validation file</span></span>  <br/> |<span data-ttu-id="124c6-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="124c6-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="124c6-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="124c6-126">Can be empty</span></span>  <br/> ||
   

