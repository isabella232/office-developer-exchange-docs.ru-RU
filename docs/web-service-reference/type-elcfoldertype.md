---
title: Тип (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: Элемент Type указывает тип папки, используемые в политику хранения.
ms.openlocfilehash: f679a9237a577d26d4b28e1b25f3e135f7193903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840244"
---
# <a name="type-elcfoldertype"></a><span data-ttu-id="d213f-103">Тип (ElcFolderType)</span><span class="sxs-lookup"><span data-stu-id="d213f-103">Type (ElcFolderType)</span></span>

<span data-ttu-id="d213f-104">Элемент **Type** указывает тип папки, используемые в политику хранения.</span><span class="sxs-lookup"><span data-stu-id="d213f-104">The **Type** element specifies the type of folder used in a retention policy.</span></span> 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 <span data-ttu-id="d213f-105">**ElcFolderType**</span><span class="sxs-lookup"><span data-stu-id="d213f-105">**ElcFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d213f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d213f-106">Attributes and elements</span></span>

<span data-ttu-id="d213f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d213f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d213f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d213f-108">Attributes</span></span>

<span data-ttu-id="d213f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d213f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d213f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d213f-110">Child elements</span></span>

<span data-ttu-id="d213f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d213f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d213f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d213f-112">Parent elements</span></span>

[<span data-ttu-id="d213f-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="d213f-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="d213f-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d213f-114">Text value</span></span>

<span data-ttu-id="d213f-115">Текстовое значение элемента **Тип** — тип папки, используемые в политику хранения.</span><span class="sxs-lookup"><span data-stu-id="d213f-115">The text value of the **Type** element is the folder type used in a retention policy.</span></span> <span data-ttu-id="d213f-116">Текстовое значение может иметь одно из следующих значений, которые представляют тип папки по умолчанию: календарь, контакты, DeletedItems, Черновики, папки "Входящие", JunkEmail, журнала, заметки, Исходящие, папки "Отправленные", задач, все, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, личные, RecoverableItems или NonIpmRoot</span><span class="sxs-lookup"><span data-stu-id="d213f-116">The text value can be one of the following values that represent a default folder type: Calendar, Contacts, DeletedItems, Drafts, Inbox, JunkEmail, Journal, Notes, Outbox, SentItems, Tasks, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, Personal, RecoverableItems, or NonIpmRoot</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d213f-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="d213f-117">Remarks</span></span>

<span data-ttu-id="d213f-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d213f-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d213f-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d213f-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d213f-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d213f-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d213f-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d213f-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d213f-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d213f-122">Schema name</span></span>  <br/> |<span data-ttu-id="d213f-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d213f-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="d213f-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d213f-124">Validation file</span></span>  <br/> |<span data-ttu-id="d213f-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d213f-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d213f-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d213f-126">Can be empty</span></span>  <br/> |<span data-ttu-id="d213f-127">Нет</span><span class="sxs-lookup"><span data-stu-id="d213f-127">false</span></span>  <br/> |
   

