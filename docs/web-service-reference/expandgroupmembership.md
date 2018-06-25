---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: Элемент ExpandGroupMembership указывает, следует ли разверните узел членов группы, возвращаемый запросом GetSearchableMailboxes.
ms.openlocfilehash: 11bfcf6893a147c726c94df77f7d9a9dfbaa773e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762433"
---
# <a name="expandgroupmembership"></a><span data-ttu-id="6014f-103">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="6014f-103">ExpandGroupMembership</span></span>

<span data-ttu-id="6014f-104">Элемент **ExpandGroupMembership** указывает, следует ли разверните узел членов группы, возвращаемый запросом **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="6014f-104">The **ExpandGroupMembership** element indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 <span data-ttu-id="6014f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6014f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6014f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6014f-106">Attributes and elements</span></span>

<span data-ttu-id="6014f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6014f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6014f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6014f-108">Attributes</span></span>

<span data-ttu-id="6014f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6014f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6014f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6014f-110">Child elements</span></span>

<span data-ttu-id="6014f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6014f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6014f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6014f-112">Parent elements</span></span>

<span data-ttu-id="6014f-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="6014f-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6014f-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6014f-114">Text value</span></span>

<span data-ttu-id="6014f-115">Текстовое значение **true** для элемента **ExpandGroupElement** указывает, что членство в группах будет развернут.</span><span class="sxs-lookup"><span data-stu-id="6014f-115">A text value of **true** for the **ExpandGroupElement** element indicates that group membership is expanded.</span></span> <span data-ttu-id="6014f-116">Значение **false** указывает, что членство в группах не развернут для отображения членов группы.</span><span class="sxs-lookup"><span data-stu-id="6014f-116">A value of **false** indicates that the group membership is not expanded to show the members of the group.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6014f-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="6014f-117">Remarks</span></span>

<span data-ttu-id="6014f-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6014f-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6014f-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6014f-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6014f-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6014f-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6014f-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6014f-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6014f-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6014f-122">Schema name</span></span>  <br/> |<span data-ttu-id="6014f-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6014f-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6014f-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6014f-124">Validation file</span></span>  <br/> |<span data-ttu-id="6014f-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6014f-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6014f-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6014f-126">Can be empty</span></span>  <br/> |<span data-ttu-id="6014f-127">Нет</span><span class="sxs-lookup"><span data-stu-id="6014f-127">false</span></span>  <br/> |
   

