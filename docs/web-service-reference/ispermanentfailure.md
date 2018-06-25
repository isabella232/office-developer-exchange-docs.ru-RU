---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: Элемент IsPermanentFailure указывает, была ли предыдущая попытка индекс элемента неудачно.
ms.openlocfilehash: 39592c15394a57e1c6aa1183ed0ccedeb085e6ea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834085"
---
# <a name="ispermanentfailure"></a><span data-ttu-id="78ac7-103">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="78ac7-103">IsPermanentFailure</span></span>

<span data-ttu-id="78ac7-104">Элемент **IsPermanentFailure** указывает, была ли предыдущая попытка индекс элемента неудачно.</span><span class="sxs-lookup"><span data-stu-id="78ac7-104">The **IsPermanentFailure** element indicates whether a previous attempt to index the item was unsuccessful.</span></span> 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 <span data-ttu-id="78ac7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="78ac7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78ac7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="78ac7-106">Attributes and elements</span></span>

<span data-ttu-id="78ac7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="78ac7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78ac7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="78ac7-108">Attributes</span></span>

<span data-ttu-id="78ac7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="78ac7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78ac7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="78ac7-110">Child elements</span></span>

<span data-ttu-id="78ac7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="78ac7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78ac7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="78ac7-112">Parent elements</span></span>

[<span data-ttu-id="78ac7-113">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="78ac7-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="78ac7-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="78ac7-114">Text value</span></span>

<span data-ttu-id="78ac7-115">Текстовое значение **true** для элемента **IsPermanentFailure** указывает, что предыдущая попытка индекс элемента почтового ящика не удалось выполнить.</span><span class="sxs-lookup"><span data-stu-id="78ac7-115">A text value of **true** for the **IsPermanentFailure** element indicates that a previous attempt to index the mailbox item was unsuccessful.</span></span> <span data-ttu-id="78ac7-116">Значение **false** указывает, что предыдущая попытка индекс элемента почтового ящика прошла успешно.</span><span class="sxs-lookup"><span data-stu-id="78ac7-116">A value of **false** indicates that a previous attempt to index the mailbox item was successful.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="78ac7-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="78ac7-117">Remarks</span></span>

<span data-ttu-id="78ac7-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="78ac7-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="78ac7-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="78ac7-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78ac7-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="78ac7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78ac7-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="78ac7-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78ac7-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="78ac7-122">Schema name</span></span>  <br/> |<span data-ttu-id="78ac7-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="78ac7-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="78ac7-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="78ac7-124">Validation file</span></span>  <br/> |<span data-ttu-id="78ac7-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="78ac7-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78ac7-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="78ac7-126">Can be empty</span></span>  <br/> |<span data-ttu-id="78ac7-127">Нет</span><span class="sxs-lookup"><span data-stu-id="78ac7-127">false</span></span>  <br/> |
   

