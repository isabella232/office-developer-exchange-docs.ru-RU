---
title: ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c2172e61-876a-4f76-bc9c-263c8be11429
description: Элемент ArchiveItem содержит идентификатор папки источника и массив идентификаторов элементов для элемента связанного архива.
ms.openlocfilehash: 7f2d79f5a9e6798fafcf64e8b1bb680390800992
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761488"
---
# <a name="archiveitem"></a><span data-ttu-id="73ca0-103">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="73ca0-103">ArchiveItem</span></span>

<span data-ttu-id="73ca0-104">Элемент **ArchiveItem** содержит идентификатор папки источника и массив идентификаторов элементов для элемента связанного архива.</span><span class="sxs-lookup"><span data-stu-id="73ca0-104">The **ArchiveItem** element contains the source folder Id and an array of item Ids for the associated archive item.</span></span> 
  
```XML
<ArchiveItem>
   <ArchiveSourceFolderId/>
   <ItemIds/>
</ArchiveItem>
```

 <span data-ttu-id="73ca0-105">**ArchiveItemType**</span><span class="sxs-lookup"><span data-stu-id="73ca0-105">**ArchiveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73ca0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="73ca0-106">Attributes and elements</span></span>

<span data-ttu-id="73ca0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="73ca0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73ca0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="73ca0-108">Attributes</span></span>

<span data-ttu-id="73ca0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="73ca0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73ca0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="73ca0-110">Child elements</span></span>

<span data-ttu-id="73ca0-111">[ArchiveSourceFolderId](archivesourcefolderid.md) | [что ItemID](itemids.md)</span><span class="sxs-lookup"><span data-stu-id="73ca0-111">[ArchiveSourceFolderId](archivesourcefolderid.md) | [ItemIds](itemids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73ca0-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="73ca0-112">Parent elements</span></span>

<span data-ttu-id="73ca0-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="73ca0-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="73ca0-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="73ca0-114">Remarks</span></span>

<span data-ttu-id="73ca0-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="73ca0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="73ca0-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="73ca0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73ca0-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="73ca0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73ca0-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="73ca0-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="73ca0-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="73ca0-119">Schema name</span></span>  <br/> |<span data-ttu-id="73ca0-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="73ca0-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="73ca0-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="73ca0-121">Validation file</span></span>  <br/> |<span data-ttu-id="73ca0-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="73ca0-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73ca0-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="73ca0-123">Can be empty</span></span>  <br/> |<span data-ttu-id="73ca0-124">Нет</span><span class="sxs-lookup"><span data-stu-id="73ca0-124">false</span></span>  <br/> |
   

