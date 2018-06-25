---
title: NonIndexableItemDetail
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a26d4c02-f1bd-40c4-9257-5db45e839f17
description: Элемент NonIndexableItemDetail указывает подробные сведения об элементе, которые не могут быть индексированы.
ms.openlocfilehash: ef1bd072a44b42b501a3016c394b89fe6ab25bf0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834543"
---
# <a name="nonindexableitemdetail"></a><span data-ttu-id="ffba3-103">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="ffba3-103">NonIndexableItemDetail</span></span>

<span data-ttu-id="ffba3-104">Элемент **NonIndexableItemDetail** указывает подробные сведения об элементе, которые не могут быть индексированы.</span><span class="sxs-lookup"><span data-stu-id="ffba3-104">The **NonIndexableItemDetail** element specifies detail information about an item that cannot be indexed.</span></span> 
  
```XML
<NonIndexableItemDetail>
   <ItemId/>
   <ErrorCode/>
   <ErrorDescription/>
   <IsPartiallyIndexed/>
   <IsPermanentFailure/>
   <SortValue/>
   <AttemptCount/>
   <LastAttemptTime/>
   <AdditionalInfo/>
</NonIndexableItemDetail>
```

 <span data-ttu-id="ffba3-105">**NonIndexableItemDetailType**</span><span class="sxs-lookup"><span data-stu-id="ffba3-105">**NonIndexableItemDetailType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffba3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ffba3-106">Attributes and elements</span></span>

<span data-ttu-id="ffba3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ffba3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffba3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ffba3-108">Attributes</span></span>

<span data-ttu-id="ffba3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ffba3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffba3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ffba3-110">Child elements</span></span>

<span data-ttu-id="ffba3-111">[Идентификатор элемента](itemid.md) | [код ошибки (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount ](attemptcount.md)  |  [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="ffba3-111">[ItemId](itemid.md) | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount](attemptcount.md) | [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ffba3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ffba3-112">Parent elements</span></span>

[<span data-ttu-id="ffba3-113">Элементы (ArrayOfNonIndexableItemDetailsType)</span><span class="sxs-lookup"><span data-stu-id="ffba3-113">Items (ArrayOfNonIndexableItemDetailsType)</span></span>](items-arrayofnonindexableitemdetailstype.md)
  
## <a name="remarks"></a><span data-ttu-id="ffba3-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="ffba3-114">Remarks</span></span>

<span data-ttu-id="ffba3-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ffba3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ffba3-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffba3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffba3-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ffba3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffba3-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ffba3-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ffba3-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ffba3-119">Schema name</span></span>  <br/> |<span data-ttu-id="ffba3-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ffba3-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="ffba3-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ffba3-121">Validation file</span></span>  <br/> |<span data-ttu-id="ffba3-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ffba3-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ffba3-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ffba3-123">Can be empty</span></span>  <br/> ||
   

