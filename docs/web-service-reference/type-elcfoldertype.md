---
title: Тип (Елкфолдертипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: Элемент Type указывает тип папки, используемой в политике хранения.
ms.openlocfilehash: f6fcc7942a530ada2d6e72c3e38286a7595b09ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465109"
---
# <a name="type-elcfoldertype"></a><span data-ttu-id="369a6-103">Тип (Елкфолдертипе)</span><span class="sxs-lookup"><span data-stu-id="369a6-103">Type (ElcFolderType)</span></span>

<span data-ttu-id="369a6-104">Элемент **Type** указывает тип папки, используемой в политике хранения.</span><span class="sxs-lookup"><span data-stu-id="369a6-104">The **Type** element specifies the type of folder used in a retention policy.</span></span> 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 <span data-ttu-id="369a6-105">**елкфолдертипе**</span><span class="sxs-lookup"><span data-stu-id="369a6-105">**ElcFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="369a6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="369a6-106">Attributes and elements</span></span>

<span data-ttu-id="369a6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="369a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="369a6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="369a6-108">Attributes</span></span>

<span data-ttu-id="369a6-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="369a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="369a6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="369a6-110">Child elements</span></span>

<span data-ttu-id="369a6-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="369a6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="369a6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="369a6-112">Parent elements</span></span>

[<span data-ttu-id="369a6-113">Retentionpolicytag используется</span><span class="sxs-lookup"><span data-stu-id="369a6-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="369a6-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="369a6-114">Text value</span></span>

<span data-ttu-id="369a6-115">Текстовое значение элемента **Type** — это тип папки, используемый в политике хранения.</span><span class="sxs-lookup"><span data-stu-id="369a6-115">The text value of the **Type** element is the folder type used in a retention policy.</span></span> <span data-ttu-id="369a6-116">Текстовое значение может быть одним из следующих значений, которые представляют тип папки по умолчанию: Calendar, Contacts, DeletedItems, Черновики, Inbox, Жункемаил, журнал, Notes, Inbox, SentItems, Tasks, ALL, Манажедкустомфолдер, Рсссубскриптионс, СинЦиссуес, ConversationHistory, Personal, RecoverableItems или Нонипмрут</span><span class="sxs-lookup"><span data-stu-id="369a6-116">The text value can be one of the following values that represent a default folder type: Calendar, Contacts, DeletedItems, Drafts, Inbox, JunkEmail, Journal, Notes, Outbox, SentItems, Tasks, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, Personal, RecoverableItems, or NonIpmRoot</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="369a6-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="369a6-117">Remarks</span></span>

<span data-ttu-id="369a6-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="369a6-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="369a6-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="369a6-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="369a6-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="369a6-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="369a6-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="369a6-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="369a6-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="369a6-122">Schema name</span></span>  <br/> |<span data-ttu-id="369a6-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="369a6-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="369a6-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="369a6-124">Validation file</span></span>  <br/> |<span data-ttu-id="369a6-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="369a6-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="369a6-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="369a6-126">Can be empty</span></span>  <br/> |<span data-ttu-id="369a6-127">false</span><span class="sxs-lookup"><span data-stu-id="369a6-127">false</span></span>  <br/> |
   

