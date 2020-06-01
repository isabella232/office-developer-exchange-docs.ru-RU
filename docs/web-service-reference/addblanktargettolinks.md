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
ms.openlocfilehash: 1d4d36c1f4b98ebee96baea683c40527d2a9ec27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465045"
---
# <a name="addblanktargettolinks"></a><span data-ttu-id="1859f-103">аддбланктаржеттолинкс</span><span class="sxs-lookup"><span data-stu-id="1859f-103">AddBlankTargetToLinks</span></span>

<span data-ttu-id="1859f-104">Элемент **аддбланктаржеттолинкс** указывает, что целевой атрибут в HTML-ссылках имеет значение открыть новое окно.</span><span class="sxs-lookup"><span data-stu-id="1859f-104">The **AddBlankTargetToLinks** element specifies that the target attribute in HTML links are set to open a new window.</span></span> 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

<span data-ttu-id="1859f-105">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="1859f-105">**xs:Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1859f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1859f-106">Attributes and elements</span></span>

<span data-ttu-id="1859f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1859f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1859f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1859f-108">Attributes</span></span>

<span data-ttu-id="1859f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1859f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1859f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1859f-110">Child elements</span></span>

<span data-ttu-id="1859f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1859f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1859f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1859f-112">Parent elements</span></span>

|<span data-ttu-id="1859f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1859f-113">**Element**</span></span>|<span data-ttu-id="1859f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1859f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1859f-115">итемшапе</span><span class="sxs-lookup"><span data-stu-id="1859f-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="1859f-116">Определяет свойства и контент элемента, включаемые в ответ **GetItem**, **FindItem**, **GetConversationItems** или **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="1859f-116">Identifies the item properties and content to include in a **GetItem**, **FindItem**, **GetConversationItems** or **SyncFolderItems** response.</span></span><br/><br/>  <span data-ttu-id="1859f-117">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="1859f-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1859f-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1859f-118">Text value</span></span>

<span data-ttu-id="1859f-119">Текстовое значение **true** для элемента **аддбланктаржеттолинкс** указывает на то, что все HTML-ссылки будут настроены на открытие нового окна.</span><span class="sxs-lookup"><span data-stu-id="1859f-119">A text value of **true** for the **AddBlankTargetToLinks** element indicates that all HTML links will be set to open a new window.</span></span> <span data-ttu-id="1859f-120">Значение **false** указывает, что HTML-ссылки будут открываться в текущем окне.</span><span class="sxs-lookup"><span data-stu-id="1859f-120">A value of **false** indicates that HTML links will open in the current window.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1859f-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="1859f-121">Remarks</span></span>

<span data-ttu-id="1859f-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="1859f-122">This element is optional.</span></span>
  
<span data-ttu-id="1859f-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1859f-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1859f-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1859f-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1859f-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1859f-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1859f-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1859f-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1859f-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1859f-127">Schema Name</span></span>  <br/> |<span data-ttu-id="1859f-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="1859f-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="1859f-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1859f-129">Validation File</span></span>  <br/> |<span data-ttu-id="1859f-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1859f-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1859f-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1859f-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1859f-132">См. также</span><span class="sxs-lookup"><span data-stu-id="1859f-132">See also</span></span>

- [<span data-ttu-id="1859f-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1859f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

