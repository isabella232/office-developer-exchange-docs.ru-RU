---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: Элемент RetentionAction указывает действие, выполняемое для элементов с помощью тега хранения.
ms.openlocfilehash: 54a1038f2e56aad66f89522423ccfbd69dc44a80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835215"
---
# <a name="retentionaction"></a><span data-ttu-id="e03b3-103">RetentionAction</span><span class="sxs-lookup"><span data-stu-id="e03b3-103">RetentionAction</span></span>

<span data-ttu-id="e03b3-104">Элемент **RetentionAction** указывает действие, выполняемое для элементов с помощью тега хранения.</span><span class="sxs-lookup"><span data-stu-id="e03b3-104">The **RetentionAction** element specifies the action performed on items with the retention tag.</span></span> 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 <span data-ttu-id="e03b3-105">**RetentionActionType**</span><span class="sxs-lookup"><span data-stu-id="e03b3-105">**RetentionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e03b3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e03b3-106">Attributes and elements</span></span>

<span data-ttu-id="e03b3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e03b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e03b3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e03b3-108">Attributes</span></span>

<span data-ttu-id="e03b3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e03b3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e03b3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e03b3-110">Child elements</span></span>

<span data-ttu-id="e03b3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e03b3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e03b3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e03b3-112">Parent elements</span></span>

[<span data-ttu-id="e03b3-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="e03b3-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="e03b3-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e03b3-114">Text value</span></span>

<span data-ttu-id="e03b3-115">Текстовое значение элемента **RetentionAction** — это действие, выполняемое для элементов.</span><span class="sxs-lookup"><span data-stu-id="e03b3-115">The text value of the **RetentionAction** element is the action performed on items.</span></span> <span data-ttu-id="e03b3-116">Следующий список содержит текстовые значения для элемента **RetentionAction** .</span><span class="sxs-lookup"><span data-stu-id="e03b3-116">The following list contains the text values for the **RetentionAction** element.</span></span> 
  
> <span data-ttu-id="e03b3-117">**None** - никаких действий выполняется для элемента.</span><span class="sxs-lookup"><span data-stu-id="e03b3-117">**None** - No action is performed on the item.</span></span> 
    
> <span data-ttu-id="e03b3-118">**MoveToDeletedItems** - элемент перемещаются в папку Deleted Items по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e03b3-118">**MoveToDeletedItems** - The item is moved to the default Deleted Items folder.</span></span> 
    
> <span data-ttu-id="e03b3-119">**MoveToFolder** - элемент перемещается в указанную папку.</span><span class="sxs-lookup"><span data-stu-id="e03b3-119">**MoveToFolder** - The item is moved to a specified folder.</span></span> 
    
> <span data-ttu-id="e03b3-120">**DeleteAndAllowRecovery** - элемент удаляется и поместить в корзину.</span><span class="sxs-lookup"><span data-stu-id="e03b3-120">**DeleteAndAllowRecovery** - The item is deleted and put into the Dumpster.</span></span> 
    
> <span data-ttu-id="e03b3-121">**PermanentlyDelete** - элемент окончательно удаляется из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e03b3-121">**PermanentlyDelete** - The item is permanently deleted from the mailbox.</span></span> 
    
> <span data-ttu-id="e03b3-122">**MarkAsPastRetentionLimit** - элемент отмечен как превышении ограничения времени хранения.</span><span class="sxs-lookup"><span data-stu-id="e03b3-122">**MarkAsPastRetentionLimit** - The item is marked as having exceeded the retention time limit.</span></span> 
    
> <span data-ttu-id="e03b3-123">**MoveToArchive** - элемент перемещаются в архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="e03b3-123">**MoveToArchive** - The item is moved to the archive mailbox.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="e03b3-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="e03b3-124">Remarks</span></span>

<span data-ttu-id="e03b3-125">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e03b3-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e03b3-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e03b3-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e03b3-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e03b3-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e03b3-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e03b3-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e03b3-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e03b3-129">Schema name</span></span>  <br/> |<span data-ttu-id="e03b3-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e03b3-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="e03b3-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e03b3-131">Validation file</span></span>  <br/> |<span data-ttu-id="e03b3-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e03b3-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e03b3-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e03b3-133">Can be empty</span></span>  <br/> ||
   

