---
title: Область поиска
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: Элемент область поиска определяет область поиска.
ms.openlocfilehash: 352292952c735e7d3893790a660096c6b6966536
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835315"
---
# <a name="searchscope"></a><span data-ttu-id="d9f9c-103">Область поиска</span><span class="sxs-lookup"><span data-stu-id="d9f9c-103">SearchScope</span></span>

<span data-ttu-id="d9f9c-104">Элемент **область поиска** определяет область поиска.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-104">The **SearchScope** element specifies the scope of a search.</span></span> 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 <span data-ttu-id="d9f9c-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="d9f9c-105">**MailboxSearchLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9f9c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d9f9c-106">Attributes and elements</span></span>

<span data-ttu-id="d9f9c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9f9c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d9f9c-108">Attributes</span></span>

<span data-ttu-id="d9f9c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9f9c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d9f9c-110">Child elements</span></span>

<span data-ttu-id="d9f9c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9f9c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d9f9c-112">Parent elements</span></span>

[<span data-ttu-id="d9f9c-113">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="d9f9c-113">MailboxSearchScope</span></span>](mailboxsearchscope.md)
  
## <a name="text-value"></a><span data-ttu-id="d9f9c-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d9f9c-114">Text value</span></span>

<span data-ttu-id="d9f9c-115">Текстовое значение элемента **область поиска** указывает тип почтового ящика, поиск поиск обнаружения.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-115">The text value of the **SearchScope** element indicates the mailbox type that is searched for a discovery search.</span></span> <span data-ttu-id="d9f9c-116">Текстовое значение **PrimaryOnly** указывает, что выполняется поиск основного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-116">A text value of **PrimaryOnly** indicates that the primary mailbox is searched.</span></span> <span data-ttu-id="d9f9c-117">Текстовое значение **ArchiveOnly** указывает, что выполняется поиск в архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-117">A text value of **ArchiveOnly** indicates that the archive mailbox is searched.</span></span> <span data-ttu-id="d9f9c-118">Текстовое значение **всех** указывает, что и первичной и поиск архивных почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-118">A text value of **All** indicates that both the primary and archive mailboxes are searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d9f9c-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="d9f9c-119">Remarks</span></span>

<span data-ttu-id="d9f9c-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d9f9c-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9f9c-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d9f9c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9f9c-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d9f9c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9f9c-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d9f9c-124">Schema name</span></span>  <br/> |<span data-ttu-id="d9f9c-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d9f9c-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9f9c-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d9f9c-126">Validation file</span></span>  <br/> |<span data-ttu-id="d9f9c-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9f9c-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9f9c-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d9f9c-128">Can be empty</span></span>  <br/> ||
   

