---
title: MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22244afb-99ec-41b4-8f73-3fbccd56d1ab
description: Элемент MarkAllItemsAsRead содержит запрос, помечающий все элементы в папке как прочтенные.
ms.openlocfilehash: 0338b2a1eed503b7e8fb0ec8b4a8ebcf12b6dbd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530890"
---
# <a name="markallitemsasread"></a><span data-ttu-id="f3238-103">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="f3238-103">MarkAllItemsAsRead</span></span>

<span data-ttu-id="f3238-104">Элемент **MarkAllItemsAsRead** содержит запрос, помечающий все элементы в папке как прочтенные.</span><span class="sxs-lookup"><span data-stu-id="f3238-104">The **MarkAllItemsAsRead** element contains the request to mark all the items in a folder as read.</span></span> 
  
```XML
<MarkAllItemsAsRead>
   <ReadFlag/>
   <SuppressReadReceipts/>
   <FolderIds/>
</MarkAllItemsAsRead>
```

 <span data-ttu-id="f3238-105">**маркаллитемсасреадтипе**</span><span class="sxs-lookup"><span data-stu-id="f3238-105">**MarkAllItemsAsReadType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3238-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f3238-106">Attributes and elements</span></span>

<span data-ttu-id="f3238-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f3238-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3238-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f3238-108">Attributes</span></span>

<span data-ttu-id="f3238-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3238-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3238-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f3238-110">Child elements</span></span>

<span data-ttu-id="f3238-111">[Реадфлаг](readflag.md)  |  [Суппрессреадрецеиптс](suppressreadreceipts.md)  |  [Фолдеридс](folderids.md)</span><span class="sxs-lookup"><span data-stu-id="f3238-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3238-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f3238-112">Parent elements</span></span>

<span data-ttu-id="f3238-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="f3238-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3238-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="f3238-114">Remarks</span></span>

<span data-ttu-id="f3238-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f3238-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f3238-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3238-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3238-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f3238-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3238-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f3238-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f3238-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f3238-119">Schema name</span></span>  <br/> |<span data-ttu-id="f3238-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f3238-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f3238-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f3238-121">Validation file</span></span>  <br/> |<span data-ttu-id="f3238-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f3238-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3238-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f3238-123">Can be empty</span></span>  <br/> ||
   

