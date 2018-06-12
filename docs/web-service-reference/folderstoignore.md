---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: Элемент FoldersToIgnore определяет список папок, которые используются, когда извлечение элементов в беседе. Все элементы беседы в игнорируемыми папок не возвращаются в ответ GetConversationItems.
ms.openlocfilehash: 96c094996c601e685dc1c7e6b869a790ce7d74a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762638"
---
# <a name="folderstoignore"></a><span data-ttu-id="caaec-104">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="caaec-104">FoldersToIgnore</span></span>

<span data-ttu-id="caaec-105">Элемент **FoldersToIgnore** определяет список папок, которые используются, когда извлечение элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="caaec-105">The **FoldersToIgnore** element identifies a list of folders that are ignored when getting items in a conversation.</span></span> <span data-ttu-id="caaec-106">Все элементы беседы в игнорируемыми папок не возвращаются в ответ **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="caaec-106">All conversation items in the ignored folders are not returned in a **GetConversationItems** response.</span></span> 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 <span data-ttu-id="caaec-107">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="caaec-107">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="caaec-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="caaec-108">Attributes and elements</span></span>

<span data-ttu-id="caaec-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="caaec-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="caaec-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="caaec-110">Attributes</span></span>

<span data-ttu-id="caaec-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="caaec-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="caaec-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="caaec-112">Child elements</span></span>

<span data-ttu-id="caaec-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="caaec-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="caaec-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="caaec-114">Parent elements</span></span>

[<span data-ttu-id="caaec-115">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="caaec-115">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="remarks"></a><span data-ttu-id="caaec-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="caaec-116">Remarks</span></span>

<span data-ttu-id="caaec-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="caaec-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="caaec-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="caaec-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="caaec-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="caaec-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="caaec-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="caaec-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="caaec-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="caaec-121">Schema name</span></span>  <br/> |<span data-ttu-id="caaec-122">Схема Types</span><span class="sxs-lookup"><span data-stu-id="caaec-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="caaec-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="caaec-123">Validation file</span></span>  <br/> |<span data-ttu-id="caaec-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="caaec-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="caaec-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="caaec-125">Can be empty</span></span>  <br/> |<span data-ttu-id="caaec-126">Нет</span><span class="sxs-lookup"><span data-stu-id="caaec-126">false</span></span>  <br/> |
   

