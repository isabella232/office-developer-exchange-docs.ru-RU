---
title: сеарчдумпстер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb62dce-c87a-4714-8023-a6b697a29699
description: Элемент Сеарчдумпстер указывает, следует ли выполнять поиск в корзине Exchange.
ms.openlocfilehash: 067bf8ea3e589aa392c6b8ba6d4dc10b430c1f28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460493"
---
# <a name="searchdumpster"></a><span data-ttu-id="2f69e-103">сеарчдумпстер</span><span class="sxs-lookup"><span data-stu-id="2f69e-103">SearchDumpster</span></span>

<span data-ttu-id="2f69e-104">Элемент **сеарчдумпстер** указывает, следует ли выполнять поиск в корзине Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f69e-104">The **SearchDumpster** element specifies whether to search in the Exchange Dumpster.</span></span> 
  
```XML
<SearchDumpster> true | false </SearchDumpster>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="2f69e-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2f69e-105">Attributes and elements</span></span>

<span data-ttu-id="2f69e-106">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2f69e-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f69e-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2f69e-107">Attributes</span></span>

<span data-ttu-id="2f69e-108">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2f69e-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f69e-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2f69e-109">Child elements</span></span>

<span data-ttu-id="2f69e-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2f69e-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2f69e-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2f69e-111">Parent elements</span></span>

[<span data-ttu-id="2f69e-112">финдмаилбоксстатистиксбикэйвордс</span><span class="sxs-lookup"><span data-stu-id="2f69e-112">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md)
  
## <a name="text-value"></a><span data-ttu-id="2f69e-113">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2f69e-113">Text value</span></span>

<span data-ttu-id="2f69e-114">Текстовое значение **true** для элемента **сеарчдумпстер** указывает на то, что поиск статистики почтового ящика включает корзину Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f69e-114">A text value of **true** for the **SearchDumpster** element indicates that the mailbox statistics search includes the Exchange Dumpster.</span></span> <span data-ttu-id="2f69e-115">Значение **false** указывает на то, что не выполняется поиск в корзине Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f69e-115">A value of **false** indicates that the Exchange Dumpster is not searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2f69e-116">Примечания</span><span class="sxs-lookup"><span data-stu-id="2f69e-116">Remarks</span></span>

<span data-ttu-id="2f69e-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2f69e-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2f69e-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f69e-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f69e-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2f69e-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f69e-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2f69e-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2f69e-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2f69e-121">Schema name</span></span>  <br/> |<span data-ttu-id="2f69e-122">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2f69e-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="2f69e-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2f69e-123">Validation file</span></span>  <br/> |<span data-ttu-id="2f69e-124">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2f69e-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2f69e-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2f69e-125">Can be empty</span></span>  <br/> ||
   

