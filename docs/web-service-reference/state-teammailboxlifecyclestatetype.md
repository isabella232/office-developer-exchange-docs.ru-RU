---
title: Состояние (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: Элемент состояния содержит состояния жизненного цикла, заданное для почтового ящика сайта.
ms.openlocfilehash: accd70d36cc34e7364387b98a2e94c56b91f012f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835571"
---
# <a name="state-teammailboxlifecyclestatetype"></a><span data-ttu-id="adf4f-103">Состояние (TeamMailboxLifecycleStateType)</span><span class="sxs-lookup"><span data-stu-id="adf4f-103">State (TeamMailboxLifecycleStateType)</span></span>

<span data-ttu-id="adf4f-104">Элемент **состояния** содержит состояния жизненного цикла, заданное для почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="adf4f-104">The **State** element contains the lifecycle state that is set on a site mailbox.</span></span> 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

<span data-ttu-id="adf4f-105">**TeamMailboxLifecycleStateType**</span><span class="sxs-lookup"><span data-stu-id="adf4f-105">**TeamMailboxLifecycleStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="adf4f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="adf4f-106">Attributes and elements</span></span>

<span data-ttu-id="adf4f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="adf4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="adf4f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="adf4f-108">Attributes</span></span>

<span data-ttu-id="adf4f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="adf4f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="adf4f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="adf4f-110">Child elements</span></span>

<span data-ttu-id="adf4f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="adf4f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="adf4f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="adf4f-112">Parent elements</span></span>

[<span data-ttu-id="adf4f-113">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="adf4f-113">SetTeamMailbox</span></span>](setteammailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="adf4f-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="adf4f-114">Text value</span></span>

<span data-ttu-id="adf4f-115">Текстовое значение элемента **состояние** является состояния жизненного цикла, заданное для почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="adf4f-115">The text value of the **State** element is the lifecycle state that is set on a site mailbox.</span></span> <span data-ttu-id="adf4f-116">Текстовое значение **Active** указывает почтовый ящик сайта в активном использовании.</span><span class="sxs-lookup"><span data-stu-id="adf4f-116">A text value of **Active** indicates that a site mailbox is in active use.</span></span> <span data-ttu-id="adf4f-117">Текстовое значение **Закрыто** указывает, что почтовый ящик сайта был закрыт и не находится в активном использовании.</span><span class="sxs-lookup"><span data-stu-id="adf4f-117">A text value of **Closed** indicates that a site mailbox has been closed and is not in active use.</span></span> <span data-ttu-id="adf4f-118">Текстовое значение **Несвязанные** указывает, что почтовый ящик сайта не связаны в среде совместной работы в Интернете.</span><span class="sxs-lookup"><span data-stu-id="adf4f-118">A text value of **Unlinked** indicates that a site mailbox is not linked to a web-based collaboration environment.</span></span> <span data-ttu-id="adf4f-119">Значения **Active**, **Закрыто**и **PendingDelete** являются взаимоисключающими, но значение **Несвязанные** не взаимно без учета расходов на другие значения.</span><span class="sxs-lookup"><span data-stu-id="adf4f-119">The **Active**, **Closed**, and **PendingDelete** values are mutually exclusive, but the **Unlinked** value is not mutually exclusive of the other values.</span></span> <span data-ttu-id="adf4f-120">Текстовое значение **PendingDelete** указывает, что почтовый ящик сайта — это процесс удаления.</span><span class="sxs-lookup"><span data-stu-id="adf4f-120">A text value of **PendingDelete** indicates that a site mailbox is pending deletion.</span></span> <span data-ttu-id="adf4f-121">Почтового ящика сайта должен быть закрыты перед его можно задать как **PendingDelete**.</span><span class="sxs-lookup"><span data-stu-id="adf4f-121">A site mailbox has to be closed before it can be set as **PendingDelete**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="adf4f-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="adf4f-122">Remarks</span></span>

<span data-ttu-id="adf4f-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="adf4f-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="adf4f-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="adf4f-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="adf4f-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="adf4f-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="adf4f-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="adf4f-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="adf4f-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="adf4f-127">Schema name</span></span>  <br/> |<span data-ttu-id="adf4f-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="adf4f-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="adf4f-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="adf4f-129">Validation file</span></span>  <br/> |<span data-ttu-id="adf4f-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="adf4f-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="adf4f-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="adf4f-131">Can be empty</span></span>  <br/> ||
   

