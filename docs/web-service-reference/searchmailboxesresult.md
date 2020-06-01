---
title: сеарчмаилбоксесресулт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: Элемент Сеарчмаилбоксесресулт содержит результат запроса SearchMailboxes.
ms.openlocfilehash: 79d593d99762aedc6290578b5458f9ac3cad3d26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466705"
---
# <a name="searchmailboxesresult"></a><span data-ttu-id="f6d3c-103">сеарчмаилбоксесресулт</span><span class="sxs-lookup"><span data-stu-id="f6d3c-103">SearchMailboxesResult</span></span>

<span data-ttu-id="f6d3c-104">Элемент **сеарчмаилбоксесресулт** содержит результат запроса **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="f6d3c-104">The **SearchMailboxesResult** element contains the result of the **SearchMailboxes** request.</span></span> 
  
```XML
<SearchMailboxesResult>
   <SearchQueries/>
   <ResultType/>
   <ItemCount/>
   <Size/>
   <PageItemCount/>
   <PageItemSize/>
   <KeywordStats/>
   <Items/>
   <FailedMailboxes/>
   <Refiners/>
   <MailboxStats/>
</SearchMailboxesResult>
```

 <span data-ttu-id="f6d3c-105">**сеарчмаилбоксесресулттипе**</span><span class="sxs-lookup"><span data-stu-id="f6d3c-105">**SearchMailboxesResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6d3c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f6d3c-106">Attributes and elements</span></span>

<span data-ttu-id="f6d3c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f6d3c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6d3c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f6d3c-108">Attributes</span></span>

<span data-ttu-id="f6d3c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f6d3c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6d3c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f6d3c-110">Child elements</span></span>

<span data-ttu-id="f6d3c-111">[Сеарчкуериес](searchqueries.md)  |  [ResultType](resulttype.md)  |  [ItemCount](itemcount.md)  |  [Размер (длинный)](size-long.md)  |  [Пажеитемкаунт](pageitemcount.md)  |  [Пажеитемсизе](pageitemsize.md)  |  [Кэйвордстатс](keywordstats.md)  |  [Элементы (аррайофсеарчпревиевитемстипе)](items-arrayofsearchpreviewitemstype.md)  |  [Фаиледмаилбоксес](failedmailboxes.md)  |  [Уточнения](refiners.md)  |  [Маилбоксстатс](mailboxstats.md)</span><span class="sxs-lookup"><span data-stu-id="f6d3c-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [Refiners](refiners.md) | [MailboxStats](mailboxstats.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f6d3c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f6d3c-112">Parent elements</span></span>

[<span data-ttu-id="f6d3c-113">сеарчмаилбоксесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f6d3c-113">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="f6d3c-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="f6d3c-114">Remarks</span></span>

<span data-ttu-id="f6d3c-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f6d3c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f6d3c-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6d3c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6d3c-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f6d3c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6d3c-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f6d3c-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6d3c-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f6d3c-119">Schema name</span></span>  <br/> |<span data-ttu-id="f6d3c-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f6d3c-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6d3c-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f6d3c-121">Validation file</span></span>  <br/> |<span data-ttu-id="f6d3c-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f6d3c-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6d3c-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f6d3c-123">Can be empty</span></span>  <br/> |<span data-ttu-id="f6d3c-124">false</span><span class="sxs-lookup"><span data-stu-id="f6d3c-124">false</span></span>  <br/> |
   

