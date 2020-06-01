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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460626"
---
# <a name="includenonindexableitems"></a><span data-ttu-id="fcf17-103">инклуденониндексаблеитемс</span><span class="sxs-lookup"><span data-stu-id="fcf17-103">IncludeNonIndexableItems</span></span>

<span data-ttu-id="fcf17-104">Элемент **инклуденониндексаблеитемс** содержит **логическое** значение, указывающее, следует ли включать элементы, которые не могут индексироваться.</span><span class="sxs-lookup"><span data-stu-id="fcf17-104">The **IncludeNonIndexableItems** element contains a **Boolean** value to indicate whether to include items that cannot be indexed.</span></span> 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 <span data-ttu-id="fcf17-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fcf17-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fcf17-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fcf17-106">Attributes and elements</span></span>

<span data-ttu-id="fcf17-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fcf17-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fcf17-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fcf17-108">Attributes</span></span>

<span data-ttu-id="fcf17-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fcf17-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fcf17-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fcf17-110">Child elements</span></span>

<span data-ttu-id="fcf17-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fcf17-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fcf17-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fcf17-112">Parent elements</span></span>

[<span data-ttu-id="fcf17-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="fcf17-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="fcf17-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fcf17-114">Text value</span></span>

<span data-ttu-id="fcf17-115">Текстовое значение **true** для элемента **инклуденониндексаблеитемс** указывает на то, что элементы, которые не могут быть индексированы, включаются в почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="fcf17-115">A text value of **true** for the **IncludeNonIndexableItems** element indicates that items that cannot be indexed are included with mailbox holds.</span></span> <span data-ttu-id="fcf17-116">Значение **false** указывает, что элементы, которые не поддаются индексированию, не включаются в удержание почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="fcf17-116">A value of **false** indicates that the items that cannot be indexed are not included in mailbox holds.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fcf17-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="fcf17-117">Remarks</span></span>

<span data-ttu-id="fcf17-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fcf17-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fcf17-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fcf17-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fcf17-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fcf17-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fcf17-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fcf17-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fcf17-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fcf17-122">Schema name</span></span>  <br/> |<span data-ttu-id="fcf17-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fcf17-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fcf17-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fcf17-124">Validation file</span></span>  <br/> |<span data-ttu-id="fcf17-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fcf17-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fcf17-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fcf17-126">Can be empty</span></span>  <br/> |<span data-ttu-id="fcf17-127">false</span><span class="sxs-lookup"><span data-stu-id="fcf17-127">false</span></span>  <br/> |
   

