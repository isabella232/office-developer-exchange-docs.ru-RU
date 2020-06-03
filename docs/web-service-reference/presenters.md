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
ms.openlocfilehash: 0236457020dfc4684569e84d3d54e357af00d102
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529912"
---
# <a name="presenters"></a><span data-ttu-id="520a8-103">Выступающих</span><span class="sxs-lookup"><span data-stu-id="520a8-103">Presenters</span></span>

<span data-ttu-id="520a8-104">Элемент **Presenter** указывает докладчиков для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="520a8-104">The **Presenters** element specifies the presenters for an online meeting.</span></span> 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 <span data-ttu-id="520a8-105">**пресентерстипе**</span><span class="sxs-lookup"><span data-stu-id="520a8-105">**PresentersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="520a8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="520a8-106">Attributes and elements</span></span>

<span data-ttu-id="520a8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="520a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="520a8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="520a8-108">Attributes</span></span>

<span data-ttu-id="520a8-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="520a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="520a8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="520a8-110">Child elements</span></span>

<span data-ttu-id="520a8-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="520a8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="520a8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="520a8-112">Parent elements</span></span>

[<span data-ttu-id="520a8-113">онлинемитингсеттингс</span><span class="sxs-lookup"><span data-stu-id="520a8-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="520a8-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="520a8-114">Text value</span></span>

<span data-ttu-id="520a8-115">Текстовое значение элемента **Presenters** — это тип пользователей, которые могут быть выступающими для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="520a8-115">The text value of **Presenters** element is the type of users that can be a presenter for an online meeting.</span></span> <span data-ttu-id="520a8-116">Текстовые значения для элемента **Presenter** описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="520a8-116">The text values for the **Presenters** element are described in the following table.</span></span> 
  
<span data-ttu-id="520a8-117">**Текстовые значения элементов выступающих**</span><span class="sxs-lookup"><span data-stu-id="520a8-117">**Presenters element text values**</span></span>

|<span data-ttu-id="520a8-118">**Значение**</span><span class="sxs-lookup"><span data-stu-id="520a8-118">**Value**</span></span>|<span data-ttu-id="520a8-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="520a8-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="520a8-120">Отключено</span><span class="sxs-lookup"><span data-stu-id="520a8-120">Disabled</span></span>  <br/> |<span data-ttu-id="520a8-121">Выступающие отключены.</span><span class="sxs-lookup"><span data-stu-id="520a8-121">Presenters are disabled.</span></span>  <br/> |
|<span data-ttu-id="520a8-122">Внутренний</span><span class="sxs-lookup"><span data-stu-id="520a8-122">Internal</span></span>  <br/> |<span data-ttu-id="520a8-123">Докладчиками могут быть только внутренние участники.</span><span class="sxs-lookup"><span data-stu-id="520a8-123">Only internal participants can be presenters.</span></span>  <br/> |
|<span data-ttu-id="520a8-124">Все</span><span class="sxs-lookup"><span data-stu-id="520a8-124">Everyone</span></span>  <br/> |<span data-ttu-id="520a8-125">Любой участник может быть докладчиком.</span><span class="sxs-lookup"><span data-stu-id="520a8-125">Any participant can be a presenter.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="520a8-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="520a8-126">Remarks</span></span>

<span data-ttu-id="520a8-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="520a8-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="520a8-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="520a8-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="520a8-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="520a8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="520a8-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="520a8-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="520a8-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="520a8-131">Schema name</span></span>  <br/> |<span data-ttu-id="520a8-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="520a8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="520a8-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="520a8-133">Validation file</span></span>  <br/> |<span data-ttu-id="520a8-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="520a8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="520a8-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="520a8-135">Can be empty</span></span>  <br/> ||
   

