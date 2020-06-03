---
title: фолдерстоигноре
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: Элемент Фолдерстоигноре определяет список папок, которые игнорируются при извлечении элементов в беседе. Все элементы беседы в игнорируемых папках не возвращаются в ответе GetConversationItems.
ms.openlocfilehash: 07813a54a9a3afa3de23ae94f1c9b191d1cb6fac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44453359"
---
# <a name="folderstoignore"></a><span data-ttu-id="855f2-104">фолдерстоигноре</span><span class="sxs-lookup"><span data-stu-id="855f2-104">FoldersToIgnore</span></span>

<span data-ttu-id="855f2-105">Элемент **фолдерстоигноре** определяет список папок, которые игнорируются при извлечении элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="855f2-105">The **FoldersToIgnore** element identifies a list of folders that are ignored when getting items in a conversation.</span></span> <span data-ttu-id="855f2-106">Все элементы беседы в игнорируемых папках не возвращаются в ответе **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="855f2-106">All conversation items in the ignored folders are not returned in a **GetConversationItems** response.</span></span> 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 <span data-ttu-id="855f2-107">**нонемптяррайофбасефолдеридстипе**</span><span class="sxs-lookup"><span data-stu-id="855f2-107">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="855f2-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="855f2-108">Attributes and elements</span></span>

<span data-ttu-id="855f2-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="855f2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="855f2-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="855f2-110">Attributes</span></span>

<span data-ttu-id="855f2-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="855f2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="855f2-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="855f2-112">Child elements</span></span>

<span data-ttu-id="855f2-113">[FolderId](folderid.md)  |  [Дистингуишедфолдерид](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="855f2-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="855f2-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="855f2-114">Parent elements</span></span>

[<span data-ttu-id="855f2-115">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="855f2-115">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="remarks"></a><span data-ttu-id="855f2-116">Примечания</span><span class="sxs-lookup"><span data-stu-id="855f2-116">Remarks</span></span>

<span data-ttu-id="855f2-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="855f2-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="855f2-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="855f2-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="855f2-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="855f2-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="855f2-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="855f2-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="855f2-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="855f2-121">Schema name</span></span>  <br/> |<span data-ttu-id="855f2-122">Схема Types</span><span class="sxs-lookup"><span data-stu-id="855f2-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="855f2-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="855f2-123">Validation file</span></span>  <br/> |<span data-ttu-id="855f2-124">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="855f2-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="855f2-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="855f2-125">Can be empty</span></span>  <br/> |<span data-ttu-id="855f2-126">false</span><span class="sxs-lookup"><span data-stu-id="855f2-126">false</span></span>  <br/> |
   

