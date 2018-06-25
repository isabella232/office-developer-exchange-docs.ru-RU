---
title: GroupIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4d32cb3b-eb84-4816-89cd-26dcf5131bc8
description: Элемент GroupIds определяет массив идентификаторов мгновенного обмена сообщениями группы.
ms.openlocfilehash: 0e463a3a74eb3a4996b521f77e1175913b22d16b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833763"
---
# <a name="groupids"></a><span data-ttu-id="37929-103">GroupIds</span><span class="sxs-lookup"><span data-stu-id="37929-103">GroupIds</span></span>

<span data-ttu-id="37929-104">Элемент **GroupIds** определяет массив идентификаторов мгновенного обмена сообщениями группы.</span><span class="sxs-lookup"><span data-stu-id="37929-104">The **GroupIds** element identifies an array of instant messaging group identifiers.</span></span> 
  
```XML
<GroupIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
   <RecurringMasterItemIdRanges/>
</GroupIds>
```

 <span data-ttu-id="37929-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="37929-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37929-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="37929-106">Attributes and elements</span></span>

<span data-ttu-id="37929-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="37929-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37929-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="37929-108">Attributes</span></span>

<span data-ttu-id="37929-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="37929-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37929-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="37929-110">Child elements</span></span>

<span data-ttu-id="37929-111">[Идентификатор элемента](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span><span class="sxs-lookup"><span data-stu-id="37929-111">[ItemId](itemid.md) | [OccurrenceItemId](occurrenceitemid.md) | [RecurringMasterItemId](recurringmasteritemid.md) | [RecurringMasterItemIdRanges](recurringmasteritemidranges.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="37929-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="37929-112">Parent elements</span></span>

[<span data-ttu-id="37929-113">GetImItems</span><span class="sxs-lookup"><span data-stu-id="37929-113">GetImItems</span></span>](getimitems.md)
  
## <a name="remarks"></a><span data-ttu-id="37929-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="37929-114">Remarks</span></span>

<span data-ttu-id="37929-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="37929-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="37929-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="37929-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37929-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="37929-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37929-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="37929-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="37929-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="37929-119">Schema name</span></span>  <br/> |<span data-ttu-id="37929-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="37929-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="37929-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="37929-121">Validation file</span></span>  <br/> |<span data-ttu-id="37929-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="37929-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="37929-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="37929-123">Can be empty</span></span>  <br/> ||
   

