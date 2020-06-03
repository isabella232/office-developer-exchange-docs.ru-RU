---
title: инклуденониндексаблеитемс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: Элемент Инклуденониндексаблеитемс содержит логическое значение, указывающее, следует ли включать элементы, которые не могут индексироваться.
ms.openlocfilehash: eab559e938f0b949d79626ae5bf61b3d4a838924
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460626"
---
# <a name="includenonindexableitems"></a><span data-ttu-id="52cc5-103">инклуденониндексаблеитемс</span><span class="sxs-lookup"><span data-stu-id="52cc5-103">IncludeNonIndexableItems</span></span>

<span data-ttu-id="52cc5-104">Элемент **инклуденониндексаблеитемс** содержит **логическое** значение, указывающее, следует ли включать элементы, которые не могут индексироваться.</span><span class="sxs-lookup"><span data-stu-id="52cc5-104">The **IncludeNonIndexableItems** element contains a **Boolean** value to indicate whether to include items that cannot be indexed.</span></span> 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 <span data-ttu-id="52cc5-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="52cc5-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52cc5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="52cc5-106">Attributes and elements</span></span>

<span data-ttu-id="52cc5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="52cc5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52cc5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="52cc5-108">Attributes</span></span>

<span data-ttu-id="52cc5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="52cc5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52cc5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="52cc5-110">Child elements</span></span>

<span data-ttu-id="52cc5-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="52cc5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="52cc5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="52cc5-112">Parent elements</span></span>

[<span data-ttu-id="52cc5-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="52cc5-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="52cc5-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="52cc5-114">Text value</span></span>

<span data-ttu-id="52cc5-115">Текстовое значение **true** для элемента **инклуденониндексаблеитемс** указывает на то, что элементы, которые не могут быть индексированы, включаются в почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="52cc5-115">A text value of **true** for the **IncludeNonIndexableItems** element indicates that items that cannot be indexed are included with mailbox holds.</span></span> <span data-ttu-id="52cc5-116">Значение **false** указывает, что элементы, которые не поддаются индексированию, не включаются в удержание почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="52cc5-116">A value of **false** indicates that the items that cannot be indexed are not included in mailbox holds.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="52cc5-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="52cc5-117">Remarks</span></span>

<span data-ttu-id="52cc5-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="52cc5-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="52cc5-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="52cc5-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52cc5-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="52cc5-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52cc5-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="52cc5-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="52cc5-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="52cc5-122">Schema name</span></span>  <br/> |<span data-ttu-id="52cc5-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="52cc5-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="52cc5-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="52cc5-124">Validation file</span></span>  <br/> |<span data-ttu-id="52cc5-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="52cc5-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="52cc5-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="52cc5-126">Can be empty</span></span>  <br/> |<span data-ttu-id="52cc5-127">false</span><span class="sxs-lookup"><span data-stu-id="52cc5-127">false</span></span>  <br/> |
   

