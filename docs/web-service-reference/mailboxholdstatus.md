---
title: MailboxHoldStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92608b77-8aa4-403b-a4de-01e3a60af3e0
description: Элемент MailboxHoldStatus указывает состояние удержания почтового ящика.
ms.openlocfilehash: 6703c909d0a7b4e83e190807fc3202ecd4699e7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834288"
---
# <a name="mailboxholdstatus"></a><span data-ttu-id="b416e-103">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="b416e-103">MailboxHoldStatus</span></span>

<span data-ttu-id="b416e-104">Элемент **MailboxHoldStatus** указывает состояние удержания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b416e-104">The **MailboxHoldStatus** element specifies the hold status of the mailbox.</span></span> 
  
```XML
<MailboxHoldStatus>
   <Mailbox/>
   <Status/>
   <AdditionalInfo/>
</MailboxHoldStatus>
```

<span data-ttu-id="b416e-105">**MailboxHoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="b416e-105">**MailboxHoldStatusType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b416e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b416e-106">Attributes and elements</span></span>

<span data-ttu-id="b416e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b416e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b416e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b416e-108">Attributes</span></span>

<span data-ttu-id="b416e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b416e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b416e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b416e-110">Child elements</span></span>

<span data-ttu-id="b416e-111">[Почтовый ящик (string)](mailbox-string.md) | [состояния (HoldStatusType)](status-holdstatustype.md) | [AdditionalInfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="b416e-111">[Mailbox (string)](mailbox-string.md) | [Status (HoldStatusType)](status-holdstatustype.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b416e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b416e-112">Parent elements</span></span>

[<span data-ttu-id="b416e-113">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="b416e-113">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
  
## <a name="remarks"></a><span data-ttu-id="b416e-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="b416e-114">Remarks</span></span>

<span data-ttu-id="b416e-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b416e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b416e-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b416e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b416e-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b416e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b416e-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b416e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b416e-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b416e-119">Schema name</span></span>  <br/> |<span data-ttu-id="b416e-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b416e-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="b416e-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b416e-121">Validation file</span></span>  <br/> |<span data-ttu-id="b416e-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b416e-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b416e-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b416e-123">Can be empty</span></span>  <br/> ||
   

