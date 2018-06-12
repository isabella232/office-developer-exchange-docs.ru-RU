---
title: ArchiveSourceFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5b6a099-3b87-44ef-a197-8198730ff72d
description: Элемент ArchiveSourceFolderId указывает идентификатор исходной папки для элемента архива.
ms.openlocfilehash: b7a5097de734777a71559703ed2d54199edd952e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761494"
---
# <a name="archivesourcefolderid"></a><span data-ttu-id="fbf34-103">ArchiveSourceFolderId</span><span class="sxs-lookup"><span data-stu-id="fbf34-103">ArchiveSourceFolderId</span></span>

<span data-ttu-id="fbf34-104">Элемент **ArchiveSourceFolderId** указывает идентификатор исходной папки для элемента архива.</span><span class="sxs-lookup"><span data-stu-id="fbf34-104">The **ArchiveSourceFolderId** element specifies the Id of the source folder for the archive item.</span></span> 
  
```XML
<ArchiveSourceFolderId>
   <FolderId/>
   <DistinguishedFolderId/>
   <AddressListId/>
</ArchiveSourceFolderId>
```

 <span data-ttu-id="fbf34-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="fbf34-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fbf34-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fbf34-106">Attributes and elements</span></span>

<span data-ttu-id="fbf34-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fbf34-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fbf34-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fbf34-108">Attributes</span></span>

<span data-ttu-id="fbf34-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fbf34-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fbf34-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fbf34-110">Child elements</span></span>

<span data-ttu-id="fbf34-111">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md) | [AddressListId](addresslistid.md)</span><span class="sxs-lookup"><span data-stu-id="fbf34-111">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md) | [AddressListId](addresslistid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fbf34-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fbf34-112">Parent elements</span></span>

[<span data-ttu-id="fbf34-113">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="fbf34-113">ArchiveItem</span></span>](archiveitem.md)
  
## <a name="remarks"></a><span data-ttu-id="fbf34-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="fbf34-114">Remarks</span></span>

<span data-ttu-id="fbf34-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fbf34-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fbf34-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fbf34-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fbf34-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fbf34-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fbf34-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fbf34-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fbf34-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fbf34-119">Schema name</span></span>  <br/> |<span data-ttu-id="fbf34-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fbf34-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fbf34-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fbf34-121">Validation file</span></span>  <br/> |<span data-ttu-id="fbf34-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fbf34-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fbf34-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fbf34-123">Can be empty</span></span>  <br/> |<span data-ttu-id="fbf34-124">Нет</span><span class="sxs-lookup"><span data-stu-id="fbf34-124">false</span></span>  <br/> |
   

