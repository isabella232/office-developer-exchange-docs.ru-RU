---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: Элемент RetentionAction указывает действие, выполняемое с элементами с помощью тега хранения.
ms.openlocfilehash: 54a1038f2e56aad66f89522423ccfbd69dc44a80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835215"
---
# <a name="retentionaction"></a><span data-ttu-id="888dd-103">RetentionAction</span><span class="sxs-lookup"><span data-stu-id="888dd-103">RetentionAction</span></span>

<span data-ttu-id="888dd-104">Элемент **RetentionAction** указывает действие, выполняемое с элементами с помощью тега хранения.</span><span class="sxs-lookup"><span data-stu-id="888dd-104">The **RetentionAction** element specifies the action performed on items with the retention tag.</span></span> 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 <span data-ttu-id="888dd-105">**ретентионактионтипе**</span><span class="sxs-lookup"><span data-stu-id="888dd-105">**RetentionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="888dd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="888dd-106">Attributes and elements</span></span>

<span data-ttu-id="888dd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="888dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="888dd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="888dd-108">Attributes</span></span>

<span data-ttu-id="888dd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="888dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="888dd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="888dd-110">Child elements</span></span>

<span data-ttu-id="888dd-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="888dd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="888dd-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="888dd-112">Parent elements</span></span>

[<span data-ttu-id="888dd-113">Retentionpolicytag используется</span><span class="sxs-lookup"><span data-stu-id="888dd-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="888dd-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="888dd-114">Text value</span></span>

<span data-ttu-id="888dd-115">Текстовое значение элемента **RetentionAction** — это действие, выполняемое над элементами.</span><span class="sxs-lookup"><span data-stu-id="888dd-115">The text value of the **RetentionAction** element is the action performed on items.</span></span> <span data-ttu-id="888dd-116">Следующий список содержит текстовые значения для элемента **RetentionAction** .</span><span class="sxs-lookup"><span data-stu-id="888dd-116">The following list contains the text values for the **RetentionAction** element.</span></span> 
  
> <span data-ttu-id="888dd-117">**None** — для элемента не выполняется никаких действий.</span><span class="sxs-lookup"><span data-stu-id="888dd-117">**None** - No action is performed on the item.</span></span> 
    
> <span data-ttu-id="888dd-118">**MoveToDeletedItems** — элемент перемещается в папку "Удаленные" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="888dd-118">**MoveToDeletedItems** - The item is moved to the default Deleted Items folder.</span></span> 
    
> <span data-ttu-id="888dd-119">**MoveToFolder** — элемент перемещается в указанную папку.</span><span class="sxs-lookup"><span data-stu-id="888dd-119">**MoveToFolder** - The item is moved to a specified folder.</span></span> 
    
> <span data-ttu-id="888dd-120">**Делетеандалловрековери** — элемент удален и помещен в корзину.</span><span class="sxs-lookup"><span data-stu-id="888dd-120">**DeleteAndAllowRecovery** - The item is deleted and put into the Dumpster.</span></span> 
    
> <span data-ttu-id="888dd-121">**PermanentlyDelete** — элемент безвозвратно удаляется из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="888dd-121">**PermanentlyDelete** - The item is permanently deleted from the mailbox.</span></span> 
    
> <span data-ttu-id="888dd-122">**Маркаспастретентионлимит** — элемент с пометкой о превышении предельного времени хранения.</span><span class="sxs-lookup"><span data-stu-id="888dd-122">**MarkAsPastRetentionLimit** - The item is marked as having exceeded the retention time limit.</span></span> 
    
> <span data-ttu-id="888dd-123">**MoveToArchive** — элемент перемещается в архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="888dd-123">**MoveToArchive** - The item is moved to the archive mailbox.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="888dd-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="888dd-124">Remarks</span></span>

<span data-ttu-id="888dd-125">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="888dd-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="888dd-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="888dd-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="888dd-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="888dd-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="888dd-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="888dd-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="888dd-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="888dd-129">Schema name</span></span>  <br/> |<span data-ttu-id="888dd-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="888dd-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="888dd-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="888dd-131">Validation file</span></span>  <br/> |<span data-ttu-id="888dd-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="888dd-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="888dd-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="888dd-133">Can be empty</span></span>  <br/> ||
   

