---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: Элемент SearchScope указывает область поиска.
ms.openlocfilehash: 352292952c735e7d3893790a660096c6b6966536
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835315"
---
# <a name="searchscope"></a><span data-ttu-id="b9168-103">SearchScope</span><span class="sxs-lookup"><span data-stu-id="b9168-103">SearchScope</span></span>

<span data-ttu-id="b9168-104">Элемент **SearchScope** указывает область поиска.</span><span class="sxs-lookup"><span data-stu-id="b9168-104">The **SearchScope** element specifies the scope of a search.</span></span> 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 <span data-ttu-id="b9168-105">**маилбокссеарчлокатионтипе**</span><span class="sxs-lookup"><span data-stu-id="b9168-105">**MailboxSearchLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9168-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b9168-106">Attributes and elements</span></span>

<span data-ttu-id="b9168-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b9168-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9168-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b9168-108">Attributes</span></span>

<span data-ttu-id="b9168-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b9168-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9168-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b9168-110">Child elements</span></span>

<span data-ttu-id="b9168-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b9168-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b9168-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b9168-112">Parent elements</span></span>

[<span data-ttu-id="b9168-113">маилбокссеарчскопе</span><span class="sxs-lookup"><span data-stu-id="b9168-113">MailboxSearchScope</span></span>](mailboxsearchscope.md)
  
## <a name="text-value"></a><span data-ttu-id="b9168-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b9168-114">Text value</span></span>

<span data-ttu-id="b9168-115">Текстовое значение элемента **SearchScope** указывает тип почтового ящика, в котором выполняется поиск поиска обнаружения.</span><span class="sxs-lookup"><span data-stu-id="b9168-115">The text value of the **SearchScope** element indicates the mailbox type that is searched for a discovery search.</span></span> <span data-ttu-id="b9168-116">Текстовое значение **PrimaryOnly** указывает на то, что выполняется поиск основного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b9168-116">A text value of **PrimaryOnly** indicates that the primary mailbox is searched.</span></span> <span data-ttu-id="b9168-117">Текстовое значение **ArchiveOnly** указывает на то, что выполняется поиск архивного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b9168-117">A text value of **ArchiveOnly** indicates that the archive mailbox is searched.</span></span> <span data-ttu-id="b9168-118">Текстовое значение **ALL** означает, что поиск выполняется как в основном, так и в архивных почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="b9168-118">A text value of **All** indicates that both the primary and archive mailboxes are searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b9168-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="b9168-119">Remarks</span></span>

<span data-ttu-id="b9168-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b9168-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b9168-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9168-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9168-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b9168-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9168-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b9168-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b9168-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b9168-124">Schema name</span></span>  <br/> |<span data-ttu-id="b9168-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b9168-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="b9168-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b9168-126">Validation file</span></span>  <br/> |<span data-ttu-id="b9168-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b9168-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b9168-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b9168-128">Can be empty</span></span>  <br/> ||
   

