---
title: аддбланктаржеттолинкс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: Элемент Аддбланктаржеттолинкс указывает, что целевой атрибут в HTML-ссылках имеет значение открыть новое окно.
ms.openlocfilehash: 8a47e44d89bcc84bc0e8b61d45f18ff3182f7870
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761332"
---
# <a name="addblanktargettolinks"></a><span data-ttu-id="bf11d-103">аддбланктаржеттолинкс</span><span class="sxs-lookup"><span data-stu-id="bf11d-103">AddBlankTargetToLinks</span></span>

<span data-ttu-id="bf11d-104">Элемент **аддбланктаржеттолинкс** указывает, что целевой атрибут в HTML-ссылках имеет значение открыть новое окно.</span><span class="sxs-lookup"><span data-stu-id="bf11d-104">The **AddBlankTargetToLinks** element specifies that the target attribute in HTML links are set to open a new window.</span></span> 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

<span data-ttu-id="bf11d-105">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="bf11d-105">**xs:Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bf11d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bf11d-106">Attributes and elements</span></span>

<span data-ttu-id="bf11d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bf11d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf11d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bf11d-108">Attributes</span></span>

<span data-ttu-id="bf11d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bf11d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf11d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bf11d-110">Child elements</span></span>

<span data-ttu-id="bf11d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="bf11d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bf11d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bf11d-112">Parent elements</span></span>

|<span data-ttu-id="bf11d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bf11d-113">**Element**</span></span>|<span data-ttu-id="bf11d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf11d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf11d-115">итемшапе</span><span class="sxs-lookup"><span data-stu-id="bf11d-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="bf11d-116">Определяет свойства и контент элемента, включаемые в ответ **GetItem**, **FindItem**, **GetConversationItems** или **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="bf11d-116">Identifies the item properties and content to include in a **GetItem**, **FindItem**, **GetConversationItems** or **SyncFolderItems** response.</span></span><br/><br/>  <span data-ttu-id="bf11d-117">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="bf11d-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bf11d-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bf11d-118">Text value</span></span>

<span data-ttu-id="bf11d-119">Текстовое значение **true** для элемента **аддбланктаржеттолинкс** указывает на то, что все HTML-ссылки будут настроены на открытие нового окна.</span><span class="sxs-lookup"><span data-stu-id="bf11d-119">A text value of **true** for the **AddBlankTargetToLinks** element indicates that all HTML links will be set to open a new window.</span></span> <span data-ttu-id="bf11d-120">Значение **false** указывает, что HTML-ссылки будут открываться в текущем окне.</span><span class="sxs-lookup"><span data-stu-id="bf11d-120">A value of **false** indicates that HTML links will open in the current window.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bf11d-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="bf11d-121">Remarks</span></span>

<span data-ttu-id="bf11d-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="bf11d-122">This element is optional.</span></span>
  
<span data-ttu-id="bf11d-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bf11d-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bf11d-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf11d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf11d-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bf11d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf11d-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bf11d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf11d-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bf11d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="bf11d-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="bf11d-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="bf11d-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bf11d-129">Validation File</span></span>  <br/> |<span data-ttu-id="bf11d-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bf11d-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf11d-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bf11d-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bf11d-132">См. также</span><span class="sxs-lookup"><span data-stu-id="bf11d-132">See also</span></span>

- [<span data-ttu-id="bf11d-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bf11d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

