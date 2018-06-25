---
title: SearchDumpster
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb62dce-c87a-4714-8023-a6b697a29699
description: Элемент SearchDumpster указывает, следует ли выполнять поиск в корзину Exchange.
ms.openlocfilehash: 4a40ee2da7fdaa4eaa3f5349545a0bfd3e13ba73
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835283"
---
# <a name="searchdumpster"></a><span data-ttu-id="227c2-103">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="227c2-103">SearchDumpster</span></span>

<span data-ttu-id="227c2-104">Элемент **SearchDumpster** указывает, следует ли выполнять поиск в корзину Exchange.</span><span class="sxs-lookup"><span data-stu-id="227c2-104">The **SearchDumpster** element specifies whether to search in the Exchange Dumpster.</span></span> 
  
```XML
<SearchDumpster> true | false </SearchDumpster>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="227c2-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="227c2-105">Attributes and elements</span></span>

<span data-ttu-id="227c2-106">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="227c2-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="227c2-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="227c2-107">Attributes</span></span>

<span data-ttu-id="227c2-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="227c2-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="227c2-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="227c2-109">Child elements</span></span>

<span data-ttu-id="227c2-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="227c2-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="227c2-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="227c2-111">Parent elements</span></span>

[<span data-ttu-id="227c2-112">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="227c2-112">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md)
  
## <a name="text-value"></a><span data-ttu-id="227c2-113">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="227c2-113">Text value</span></span>

<span data-ttu-id="227c2-114">Текстовое значение **true** для элемента **SearchDumpster** указывает, что статистика поиска в почтовом ящике включает в себя корзины Exchange.</span><span class="sxs-lookup"><span data-stu-id="227c2-114">A text value of **true** for the **SearchDumpster** element indicates that the mailbox statistics search includes the Exchange Dumpster.</span></span> <span data-ttu-id="227c2-115">Значение **false** указывает, что поиск корзину Exchange не выполняется.</span><span class="sxs-lookup"><span data-stu-id="227c2-115">A value of **false** indicates that the Exchange Dumpster is not searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="227c2-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="227c2-116">Remarks</span></span>

<span data-ttu-id="227c2-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="227c2-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="227c2-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="227c2-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="227c2-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="227c2-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="227c2-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="227c2-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="227c2-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="227c2-121">Schema name</span></span>  <br/> |<span data-ttu-id="227c2-122">Схема Types</span><span class="sxs-lookup"><span data-stu-id="227c2-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="227c2-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="227c2-123">Validation file</span></span>  <br/> |<span data-ttu-id="227c2-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="227c2-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="227c2-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="227c2-125">Can be empty</span></span>  <br/> ||
   

