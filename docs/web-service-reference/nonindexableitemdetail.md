---
title: нониндексаблеитемдетаил
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a26d4c02-f1bd-40c4-9257-5db45e839f17
description: Элемент Нониндексаблеитемдетаил указывает подробные сведения об элементе, который невозможно индексировать.
ms.openlocfilehash: ef1bd072a44b42b501a3016c394b89fe6ab25bf0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834543"
---
# <a name="nonindexableitemdetail"></a><span data-ttu-id="2632e-103">нониндексаблеитемдетаил</span><span class="sxs-lookup"><span data-stu-id="2632e-103">NonIndexableItemDetail</span></span>

<span data-ttu-id="2632e-104">Элемент **нониндексаблеитемдетаил** указывает подробные сведения об элементе, который невозможно индексировать.</span><span class="sxs-lookup"><span data-stu-id="2632e-104">The **NonIndexableItemDetail** element specifies detail information about an item that cannot be indexed.</span></span> 
  
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

 <span data-ttu-id="2632e-105">**нониндексаблеитемдетаилтипе**</span><span class="sxs-lookup"><span data-stu-id="2632e-105">**NonIndexableItemDetailType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2632e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2632e-106">Attributes and elements</span></span>

<span data-ttu-id="2632e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2632e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2632e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2632e-108">Attributes</span></span>

<span data-ttu-id="2632e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2632e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2632e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2632e-110">Child elements</span></span>

<span data-ttu-id="2632e-111">[ItemId](itemid.md) | [ErrorCode (итеминдексеррортипе)](errorcode-itemindexerrortype.md) | [еррордескриптион](errordescription.md) | [испартиаллиндексед](ispartiallyindexed.md) | [исперманентфаилуре](ispermanentfailure.md) | [AttemptCount](attemptcount.md)[SortValue](sortvalue.md) | [AdditionalInfo](additionalinfo.md) сортвалуе AttemptCount | [LastAttemptTime](lastattempttime.md)AdditionalInfo | </span><span class="sxs-lookup"><span data-stu-id="2632e-111">[ItemId](itemid.md) | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount](attemptcount.md) | [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2632e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2632e-112">Parent elements</span></span>

[<span data-ttu-id="2632e-113">Элементы (Аррайофнониндексаблеитемдетаилстипе)</span><span class="sxs-lookup"><span data-stu-id="2632e-113">Items (ArrayOfNonIndexableItemDetailsType)</span></span>](items-arrayofnonindexableitemdetailstype.md)
  
## <a name="remarks"></a><span data-ttu-id="2632e-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="2632e-114">Remarks</span></span>

<span data-ttu-id="2632e-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2632e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2632e-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2632e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2632e-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2632e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2632e-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2632e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2632e-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2632e-119">Schema name</span></span>  <br/> |<span data-ttu-id="2632e-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2632e-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="2632e-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2632e-121">Validation file</span></span>  <br/> |<span data-ttu-id="2632e-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2632e-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2632e-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2632e-123">Can be empty</span></span>  <br/> ||
   

