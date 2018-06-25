---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: Элемент AddBlankTargetToLinks указывает, что атрибут target в HTML-ссылки откройте новое окно.
ms.openlocfilehash: 8a47e44d89bcc84bc0e8b61d45f18ff3182f7870
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761332"
---
# <a name="addblanktargettolinks"></a><span data-ttu-id="0e406-103">AddBlankTargetToLinks</span><span class="sxs-lookup"><span data-stu-id="0e406-103">AddBlankTargetToLinks</span></span>

<span data-ttu-id="0e406-104">Элемент **AddBlankTargetToLinks** указывает, что атрибут target в HTML-ссылки откройте новое окно.</span><span class="sxs-lookup"><span data-stu-id="0e406-104">The **AddBlankTargetToLinks** element specifies that the target attribute in HTML links are set to open a new window.</span></span> 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

<span data-ttu-id="0e406-105">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="0e406-105">**xs:Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0e406-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0e406-106">Attributes and elements</span></span>

<span data-ttu-id="0e406-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0e406-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e406-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0e406-108">Attributes</span></span>

<span data-ttu-id="0e406-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0e406-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e406-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0e406-110">Child elements</span></span>

<span data-ttu-id="0e406-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="0e406-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e406-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0e406-112">Parent elements</span></span>

|<span data-ttu-id="0e406-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0e406-113">**Element**</span></span>|<span data-ttu-id="0e406-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0e406-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e406-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="0e406-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="0e406-116">Определяет свойства элемента и содержимого для включения в **GetItem**, **FindItem**, **GetConversationItems** или **SyncFolderItems** ответа.</span><span class="sxs-lookup"><span data-stu-id="0e406-116">Identifies the item properties and content to include in a **GetItem**, **FindItem**, **GetConversationItems** or **SyncFolderItems** response.</span></span><br/><br/>  <span data-ttu-id="0e406-117">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0e406-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e406-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0e406-118">Text value</span></span>

<span data-ttu-id="0e406-119">Текстовое значение **true** для элемента **AddBlankTargetToLinks** указывает, что все ссылки HTML-код будет иметь значение откройте новое окно.</span><span class="sxs-lookup"><span data-stu-id="0e406-119">A text value of **true** for the **AddBlankTargetToLinks** element indicates that all HTML links will be set to open a new window.</span></span> <span data-ttu-id="0e406-120">Значение **false** указывает, что HTML-ссылки будут открываться в текущем окне.</span><span class="sxs-lookup"><span data-stu-id="0e406-120">A value of **false** indicates that HTML links will open in the current window.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0e406-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="0e406-121">Remarks</span></span>

<span data-ttu-id="0e406-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0e406-122">This element is optional.</span></span>
  
<span data-ttu-id="0e406-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0e406-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0e406-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0e406-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e406-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0e406-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e406-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0e406-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e406-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0e406-127">Schema Name</span></span>  <br/> |<span data-ttu-id="0e406-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="0e406-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="0e406-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0e406-129">Validation File</span></span>  <br/> |<span data-ttu-id="0e406-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0e406-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e406-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0e406-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0e406-132">См. также</span><span class="sxs-lookup"><span data-stu-id="0e406-132">See also</span></span>

- [<span data-ttu-id="0e406-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0e406-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

