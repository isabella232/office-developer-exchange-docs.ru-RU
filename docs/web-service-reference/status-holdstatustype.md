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
ms.openlocfilehash: cecfdfaf67b00b6f8cf02188e7a4df7062a732e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459989"
---
# <a name="status-holdstatustype"></a><span data-ttu-id="ad10f-103">Состояние (Холдстатустипе)</span><span class="sxs-lookup"><span data-stu-id="ad10f-103">Status (HoldStatusType)</span></span>

<span data-ttu-id="ad10f-104">Элемент **Status** указывает состояние удержания для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="ad10f-104">The **Status** element specifies the hold status for a mailbox.</span></span> 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 <span data-ttu-id="ad10f-105">**холдстатустипе**</span><span class="sxs-lookup"><span data-stu-id="ad10f-105">**HoldStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad10f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ad10f-106">Attributes and elements</span></span>

<span data-ttu-id="ad10f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ad10f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad10f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ad10f-108">Attributes</span></span>

<span data-ttu-id="ad10f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ad10f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad10f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ad10f-110">Child elements</span></span>

<span data-ttu-id="ad10f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ad10f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ad10f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ad10f-112">Parent elements</span></span>

[<span data-ttu-id="ad10f-113">маилбоксхолдстатус</span><span class="sxs-lookup"><span data-stu-id="ad10f-113">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
  
## <a name="text-value"></a><span data-ttu-id="ad10f-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ad10f-114">Text value</span></span>

<span data-ttu-id="ad10f-115">Текстовое значение элемента **Status** — это состояние удержания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="ad10f-115">The text value of the **Status** element is the hold status of a mailbox.</span></span> <span data-ttu-id="ad10f-116">Элемент **Status** может иметь значения из следующего списка.</span><span class="sxs-lookup"><span data-stu-id="ad10f-116">The **Status** element can have the values in the following list.</span></span> 
  
> <span data-ttu-id="ad10f-117">Нотонхолд — почтовый ящик не находится на удержании.</span><span class="sxs-lookup"><span data-stu-id="ad10f-117">NotOnHold - The mailbox is not on hold.</span></span>
    
> <span data-ttu-id="ad10f-118">Ожидание — почтовый ящик находится в состоянии ожидания размещения или освобождения.</span><span class="sxs-lookup"><span data-stu-id="ad10f-118">Pending - The mailbox is pending either being placed or released on hold.</span></span> 
    
> <span data-ttu-id="ad10f-119">Onhold — удержание успешно применено к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="ad10f-119">OnHold - The hold was successfully applied to the mailbox.</span></span> 
    
> <span data-ttu-id="ad10f-120">Партиалхолд — удержание успешно применено к некоторым почтовым ящикам, но не ко всем почтовым ящикам.</span><span class="sxs-lookup"><span data-stu-id="ad10f-120">PartialHold - The hold was successfully applied to some mailboxes but not to all mailboxes.</span></span>
    
> <span data-ttu-id="ad10f-121">Сбой: не удалось применить удержание к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="ad10f-121">Failed - The hold failed to apply to the mailbox.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="ad10f-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="ad10f-122">Remarks</span></span>

<span data-ttu-id="ad10f-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ad10f-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ad10f-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad10f-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad10f-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ad10f-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad10f-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ad10f-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad10f-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ad10f-127">Schema name</span></span>  <br/> |<span data-ttu-id="ad10f-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ad10f-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad10f-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ad10f-129">Validation file</span></span>  <br/> |<span data-ttu-id="ad10f-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ad10f-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad10f-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ad10f-131">Can be empty</span></span>  <br/> ||
   

