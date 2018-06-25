---
title: MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22244afb-99ec-41b4-8f73-3fbccd56d1ab
description: Элемент MarkAllItemsAsRead содержит запрос, чтобы пометить все элементы в папке как прочтенные.
ms.openlocfilehash: 9d7eb8eb7194cb5d77e909dc08abfb70e2385d56
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834346"
---
# <a name="markallitemsasread"></a><span data-ttu-id="b11eb-103">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="b11eb-103">MarkAllItemsAsRead</span></span>

<span data-ttu-id="b11eb-104">Элемент **MarkAllItemsAsRead** содержит запрос, чтобы пометить все элементы в папке как прочтенные.</span><span class="sxs-lookup"><span data-stu-id="b11eb-104">The **MarkAllItemsAsRead** element contains the request to mark all the items in a folder as read.</span></span> 
  
```XML
<MarkAllItemsAsRead>
   <ReadFlag/>
   <SuppressReadReceipts/>
   <FolderIds/>
</MarkAllItemsAsRead>
```

 <span data-ttu-id="b11eb-105">**MarkAllItemsAsReadType**</span><span class="sxs-lookup"><span data-stu-id="b11eb-105">**MarkAllItemsAsReadType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b11eb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b11eb-106">Attributes and elements</span></span>

<span data-ttu-id="b11eb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b11eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b11eb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b11eb-108">Attributes</span></span>

<span data-ttu-id="b11eb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b11eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b11eb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b11eb-110">Child elements</span></span>

<span data-ttu-id="b11eb-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span><span class="sxs-lookup"><span data-stu-id="b11eb-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b11eb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b11eb-112">Parent elements</span></span>

<span data-ttu-id="b11eb-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="b11eb-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b11eb-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="b11eb-114">Remarks</span></span>

<span data-ttu-id="b11eb-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b11eb-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b11eb-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b11eb-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b11eb-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b11eb-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b11eb-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b11eb-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b11eb-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b11eb-119">Schema name</span></span>  <br/> |<span data-ttu-id="b11eb-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b11eb-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b11eb-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b11eb-121">Validation file</span></span>  <br/> |<span data-ttu-id="b11eb-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b11eb-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b11eb-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b11eb-123">Can be empty</span></span>  <br/> ||
   

