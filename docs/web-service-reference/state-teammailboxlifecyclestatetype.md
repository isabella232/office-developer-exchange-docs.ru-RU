---
title: Состояние (Теаммаилбокслифециклестатетипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: Элемент state содержит состояние жизненного цикла, заданное для почтового ящика сайта.
ms.openlocfilehash: 597946b48649d997f8dd57823b4e0fcc091a6f84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465165"
---
# <a name="state-teammailboxlifecyclestatetype"></a><span data-ttu-id="ae1b9-103">Состояние (Теаммаилбокслифециклестатетипе)</span><span class="sxs-lookup"><span data-stu-id="ae1b9-103">State (TeamMailboxLifecycleStateType)</span></span>

<span data-ttu-id="ae1b9-104">Элемент **State** содержит состояние жизненного цикла, заданное для почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-104">The **State** element contains the lifecycle state that is set on a site mailbox.</span></span> 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

<span data-ttu-id="ae1b9-105">**теаммаилбокслифециклестатетипе**</span><span class="sxs-lookup"><span data-stu-id="ae1b9-105">**TeamMailboxLifecycleStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ae1b9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ae1b9-106">Attributes and elements</span></span>

<span data-ttu-id="ae1b9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae1b9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ae1b9-108">Attributes</span></span>

<span data-ttu-id="ae1b9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae1b9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ae1b9-110">Child elements</span></span>

<span data-ttu-id="ae1b9-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ae1b9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ae1b9-112">Parent elements</span></span>

[<span data-ttu-id="ae1b9-113">сеттеаммаилбокс</span><span class="sxs-lookup"><span data-stu-id="ae1b9-113">SetTeamMailbox</span></span>](setteammailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="ae1b9-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ae1b9-114">Text value</span></span>

<span data-ttu-id="ae1b9-115">Текстовое значение элемента **State** — это состояние жизненного цикла, заданное для почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-115">The text value of the **State** element is the lifecycle state that is set on a site mailbox.</span></span> <span data-ttu-id="ae1b9-116">Текстовое значение **Active** указывает на то, что почтовый ящик сайта активно используется.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-116">A text value of **Active** indicates that a site mailbox is in active use.</span></span> <span data-ttu-id="ae1b9-117">Текстовое значение **Closed** указывает на то, что почтовый ящик сайта был закрыт и не используется в активном режиме.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-117">A text value of **Closed** indicates that a site mailbox has been closed and is not in active use.</span></span> <span data-ttu-id="ae1b9-118">Несвязанное текстовое **значение указывает на** то, что почтовый ящик сайта не связан с средой совместной работы на основе Интернета.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-118">A text value of **Unlinked** indicates that a site mailbox is not linked to a web-based collaboration environment.</span></span> <span data-ttu-id="ae1b9-119">Значения " **Active**", " **Closed**" и " **пендингделете** " являются взаимоисключающими, но **несвязанное** значение не является взаимоисключающим по отношению к другим значениям.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-119">The **Active**, **Closed**, and **PendingDelete** values are mutually exclusive, but the **Unlinked** value is not mutually exclusive of the other values.</span></span> <span data-ttu-id="ae1b9-120">Текстовое значение **пендингделете** указывает на то, что почтовый ящик сайта ожидает удаления.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-120">A text value of **PendingDelete** indicates that a site mailbox is pending deletion.</span></span> <span data-ttu-id="ae1b9-121">Необходимо закрыть почтовый ящик сайта, прежде чем его можно будет задать в качестве **пендингделете**.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-121">A site mailbox has to be closed before it can be set as **PendingDelete**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae1b9-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="ae1b9-122">Remarks</span></span>

<span data-ttu-id="ae1b9-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ae1b9-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae1b9-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae1b9-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ae1b9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae1b9-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ae1b9-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ae1b9-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ae1b9-127">Schema name</span></span>  <br/> |<span data-ttu-id="ae1b9-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ae1b9-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ae1b9-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ae1b9-129">Validation file</span></span>  <br/> |<span data-ttu-id="ae1b9-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ae1b9-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ae1b9-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ae1b9-131">Can be empty</span></span>  <br/> ||
   

