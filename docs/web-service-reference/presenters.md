---
title: Докладчики
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: Элемент выступающие указывает докладчики в собрании по сети.
ms.openlocfilehash: f62b458759e0d8199c98827602d6c3fe16aebeea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834875"
---
# <a name="presenters"></a><span data-ttu-id="1c705-103">Докладчики</span><span class="sxs-lookup"><span data-stu-id="1c705-103">Presenters</span></span>

<span data-ttu-id="1c705-104">Элемент **выступающие** указывает докладчики в собрании по сети.</span><span class="sxs-lookup"><span data-stu-id="1c705-104">The **Presenters** element specifies the presenters for an online meeting.</span></span> 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 <span data-ttu-id="1c705-105">**PresentersType**</span><span class="sxs-lookup"><span data-stu-id="1c705-105">**PresentersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c705-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1c705-106">Attributes and elements</span></span>

<span data-ttu-id="1c705-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1c705-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c705-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1c705-108">Attributes</span></span>

<span data-ttu-id="1c705-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1c705-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c705-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1c705-110">Child elements</span></span>

<span data-ttu-id="1c705-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="1c705-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1c705-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1c705-112">Parent elements</span></span>

[<span data-ttu-id="1c705-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="1c705-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="1c705-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1c705-114">Text value</span></span>

<span data-ttu-id="1c705-115">Текстовое значение элемента **выступающие** — тип пользователей, которые могут быть выступающим собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="1c705-115">The text value of **Presenters** element is the type of users that can be a presenter for an online meeting.</span></span> <span data-ttu-id="1c705-116">Текстовые значения для элемента **выступающие** описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="1c705-116">The text values for the **Presenters** element are described in the following table.</span></span> 
  
<span data-ttu-id="1c705-117">**Докладчики элемент текстовые значения**</span><span class="sxs-lookup"><span data-stu-id="1c705-117">**Presenters element text values**</span></span>

|<span data-ttu-id="1c705-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="1c705-118">**Value**</span></span>|<span data-ttu-id="1c705-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1c705-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1c705-120">Отключена</span><span class="sxs-lookup"><span data-stu-id="1c705-120">Disabled</span></span>  <br/> |<span data-ttu-id="1c705-121">Докладчики отключены.</span><span class="sxs-lookup"><span data-stu-id="1c705-121">Presenters are disabled.</span></span>  <br/> |
|<span data-ttu-id="1c705-122">Внутренний</span><span class="sxs-lookup"><span data-stu-id="1c705-122">Internal</span></span>  <br/> |<span data-ttu-id="1c705-123">Только внутренние участников может быть выступающим.</span><span class="sxs-lookup"><span data-stu-id="1c705-123">Only internal participants can be presenters.</span></span>  <br/> |
|<span data-ttu-id="1c705-124">Всем пользователям</span><span class="sxs-lookup"><span data-stu-id="1c705-124">Everyone</span></span>  <br/> |<span data-ttu-id="1c705-125">Любой участник может быть выступающим.</span><span class="sxs-lookup"><span data-stu-id="1c705-125">Any participant can be a presenter.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1c705-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="1c705-126">Remarks</span></span>

<span data-ttu-id="1c705-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1c705-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1c705-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c705-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c705-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1c705-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c705-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1c705-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c705-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1c705-131">Schema name</span></span>  <br/> |<span data-ttu-id="1c705-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1c705-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="1c705-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1c705-133">Validation file</span></span>  <br/> |<span data-ttu-id="1c705-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1c705-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c705-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1c705-135">Can be empty</span></span>  <br/> ||
   

