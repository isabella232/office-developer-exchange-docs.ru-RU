---
title: Состояние (Холдстатустипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: Элемент Status указывает состояние удержания для почтового ящика.
ms.openlocfilehash: c40dc865d2b305ac86fa40d536e2d516a14260ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835579"
---
# <a name="status-holdstatustype"></a><span data-ttu-id="571c6-103">Состояние (Холдстатустипе)</span><span class="sxs-lookup"><span data-stu-id="571c6-103">Status (HoldStatusType)</span></span>

<span data-ttu-id="571c6-104">Элемент **Status** указывает состояние удержания для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="571c6-104">The **Status** element specifies the hold status for a mailbox.</span></span> 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 <span data-ttu-id="571c6-105">**холдстатустипе**</span><span class="sxs-lookup"><span data-stu-id="571c6-105">**HoldStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="571c6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="571c6-106">Attributes and elements</span></span>

<span data-ttu-id="571c6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="571c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="571c6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="571c6-108">Attributes</span></span>

<span data-ttu-id="571c6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="571c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="571c6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="571c6-110">Child elements</span></span>

<span data-ttu-id="571c6-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="571c6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="571c6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="571c6-112">Parent elements</span></span>

[<span data-ttu-id="571c6-113">маилбоксхолдстатус</span><span class="sxs-lookup"><span data-stu-id="571c6-113">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
  
## <a name="text-value"></a><span data-ttu-id="571c6-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="571c6-114">Text value</span></span>

<span data-ttu-id="571c6-115">Текстовое значение элемента **Status** — это состояние удержания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="571c6-115">The text value of the **Status** element is the hold status of a mailbox.</span></span> <span data-ttu-id="571c6-116">Элемент **Status** может иметь значения из следующего списка.</span><span class="sxs-lookup"><span data-stu-id="571c6-116">The **Status** element can have the values in the following list.</span></span> 
  
> <span data-ttu-id="571c6-117">Нотонхолд — почтовый ящик не находится на удержании.</span><span class="sxs-lookup"><span data-stu-id="571c6-117">NotOnHold - The mailbox is not on hold.</span></span>
    
> <span data-ttu-id="571c6-118">Ожидание — почтовый ящик находится в состоянии ожидания размещения или освобождения.</span><span class="sxs-lookup"><span data-stu-id="571c6-118">Pending - The mailbox is pending either being placed or released on hold.</span></span> 
    
> <span data-ttu-id="571c6-119">Onhold — удержание успешно применено к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="571c6-119">OnHold - The hold was successfully applied to the mailbox.</span></span> 
    
> <span data-ttu-id="571c6-120">Партиалхолд — удержание успешно применено к некоторым почтовым ящикам, но не ко всем почтовым ящикам.</span><span class="sxs-lookup"><span data-stu-id="571c6-120">PartialHold - The hold was successfully applied to some mailboxes but not to all mailboxes.</span></span>
    
> <span data-ttu-id="571c6-121">Сбой: не удалось применить удержание к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="571c6-121">Failed - The hold failed to apply to the mailbox.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="571c6-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="571c6-122">Remarks</span></span>

<span data-ttu-id="571c6-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="571c6-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="571c6-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="571c6-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="571c6-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="571c6-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="571c6-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="571c6-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="571c6-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="571c6-127">Schema name</span></span>  <br/> |<span data-ttu-id="571c6-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="571c6-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="571c6-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="571c6-129">Validation file</span></span>  <br/> |<span data-ttu-id="571c6-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="571c6-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="571c6-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="571c6-131">Can be empty</span></span>  <br/> ||
   

