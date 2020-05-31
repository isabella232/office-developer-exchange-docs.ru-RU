---
title: Выступающих
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: Элемент Presenter указывает докладчиков для собрания по сети.
ms.openlocfilehash: f62b458759e0d8199c98827602d6c3fe16aebeea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834875"
---
# <a name="presenters"></a><span data-ttu-id="4a8c7-103">Выступающих</span><span class="sxs-lookup"><span data-stu-id="4a8c7-103">Presenters</span></span>

<span data-ttu-id="4a8c7-104">Элемент **Presenter** указывает докладчиков для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-104">The **Presenters** element specifies the presenters for an online meeting.</span></span> 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 <span data-ttu-id="4a8c7-105">**пресентерстипе**</span><span class="sxs-lookup"><span data-stu-id="4a8c7-105">**PresentersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a8c7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4a8c7-106">Attributes and elements</span></span>

<span data-ttu-id="4a8c7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a8c7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4a8c7-108">Attributes</span></span>

<span data-ttu-id="4a8c7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a8c7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4a8c7-110">Child elements</span></span>

<span data-ttu-id="4a8c7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a8c7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4a8c7-112">Parent elements</span></span>

[<span data-ttu-id="4a8c7-113">онлинемитингсеттингс</span><span class="sxs-lookup"><span data-stu-id="4a8c7-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="4a8c7-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4a8c7-114">Text value</span></span>

<span data-ttu-id="4a8c7-115">Текстовое значение элемента **Presenters** — это тип пользователей, которые могут быть выступающими для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-115">The text value of **Presenters** element is the type of users that can be a presenter for an online meeting.</span></span> <span data-ttu-id="4a8c7-116">Текстовые значения для элемента **Presenter** описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-116">The text values for the **Presenters** element are described in the following table.</span></span> 
  
<span data-ttu-id="4a8c7-117">**Текстовые значения элементов выступающих**</span><span class="sxs-lookup"><span data-stu-id="4a8c7-117">**Presenters element text values**</span></span>

|<span data-ttu-id="4a8c7-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="4a8c7-118">**Value**</span></span>|<span data-ttu-id="4a8c7-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4a8c7-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4a8c7-120">Отключено</span><span class="sxs-lookup"><span data-stu-id="4a8c7-120">Disabled</span></span>  <br/> |<span data-ttu-id="4a8c7-121">Выступающие отключены.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-121">Presenters are disabled.</span></span>  <br/> |
|<span data-ttu-id="4a8c7-122">Внутренний</span><span class="sxs-lookup"><span data-stu-id="4a8c7-122">Internal</span></span>  <br/> |<span data-ttu-id="4a8c7-123">Докладчиками могут быть только внутренние участники.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-123">Only internal participants can be presenters.</span></span>  <br/> |
|<span data-ttu-id="4a8c7-124">Все</span><span class="sxs-lookup"><span data-stu-id="4a8c7-124">Everyone</span></span>  <br/> |<span data-ttu-id="4a8c7-125">Любой участник может быть докладчиком.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-125">Any participant can be a presenter.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4a8c7-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="4a8c7-126">Remarks</span></span>

<span data-ttu-id="4a8c7-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4a8c7-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4a8c7-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a8c7-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4a8c7-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a8c7-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4a8c7-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a8c7-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4a8c7-131">Schema name</span></span>  <br/> |<span data-ttu-id="4a8c7-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4a8c7-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a8c7-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4a8c7-133">Validation file</span></span>  <br/> |<span data-ttu-id="4a8c7-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4a8c7-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a8c7-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4a8c7-135">Can be empty</span></span>  <br/> ||
   

