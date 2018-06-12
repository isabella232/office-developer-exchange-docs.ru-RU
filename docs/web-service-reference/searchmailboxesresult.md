---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: Элемент SearchMailboxesResult содержит результат запроса SearchMailboxes.
ms.openlocfilehash: 93e5837216ef8942b77ac2a91f5ef5f0ad001756
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835300"
---
# <a name="searchmailboxesresult"></a><span data-ttu-id="385b8-103">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="385b8-103">SearchMailboxesResult</span></span>

<span data-ttu-id="385b8-104">Элемент **SearchMailboxesResult** содержит результат запроса **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="385b8-104">The **SearchMailboxesResult** element contains the result of the **SearchMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="385b8-105">**SearchMailboxesResultType**</span><span class="sxs-lookup"><span data-stu-id="385b8-105">**SearchMailboxesResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="385b8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="385b8-106">Attributes and elements</span></span>

<span data-ttu-id="385b8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="385b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="385b8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="385b8-108">Attributes</span></span>

<span data-ttu-id="385b8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="385b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="385b8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="385b8-110">Child elements</span></span>

<span data-ttu-id="385b8-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [ItemCount](itemcount.md) | [размер (длинный)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [элементов () ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [уточнений](refiners.md) | [MailboxStats](mailboxstats.md)</span><span class="sxs-lookup"><span data-stu-id="385b8-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [Refiners](refiners.md) | [MailboxStats](mailboxstats.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="385b8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="385b8-112">Parent elements</span></span>

[<span data-ttu-id="385b8-113">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="385b8-113">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="385b8-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="385b8-114">Remarks</span></span>

<span data-ttu-id="385b8-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="385b8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="385b8-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="385b8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="385b8-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="385b8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="385b8-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="385b8-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="385b8-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="385b8-119">Schema name</span></span>  <br/> |<span data-ttu-id="385b8-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="385b8-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="385b8-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="385b8-121">Validation file</span></span>  <br/> |<span data-ttu-id="385b8-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="385b8-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="385b8-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="385b8-123">Can be empty</span></span>  <br/> |<span data-ttu-id="385b8-124">Нет</span><span class="sxs-lookup"><span data-stu-id="385b8-124">false</span></span>  <br/> |
   

