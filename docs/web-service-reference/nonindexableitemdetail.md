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
ms.openlocfilehash: 4fc4324501570402d22aa303d6af2a60b50b3cc6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466740"
---
# <a name="nonindexableitemdetail"></a><span data-ttu-id="1efa2-103">нониндексаблеитемдетаил</span><span class="sxs-lookup"><span data-stu-id="1efa2-103">NonIndexableItemDetail</span></span>

<span data-ttu-id="1efa2-104">Элемент **нониндексаблеитемдетаил** указывает подробные сведения об элементе, который невозможно индексировать.</span><span class="sxs-lookup"><span data-stu-id="1efa2-104">The **NonIndexableItemDetail** element specifies detail information about an item that cannot be indexed.</span></span> 
  
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

 <span data-ttu-id="1efa2-105">**нониндексаблеитемдетаилтипе**</span><span class="sxs-lookup"><span data-stu-id="1efa2-105">**NonIndexableItemDetailType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1efa2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1efa2-106">Attributes and elements</span></span>

<span data-ttu-id="1efa2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1efa2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1efa2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1efa2-108">Attributes</span></span>

<span data-ttu-id="1efa2-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1efa2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1efa2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1efa2-110">Child elements</span></span>

<span data-ttu-id="1efa2-111">[ItemId](itemid.md)  |  [ErrorCode (итеминдексеррортипе)](errorcode-itemindexerrortype.md)  |  [Еррордескриптион](errordescription.md)  |  [Испартиаллиндексед](ispartiallyindexed.md)  |  [Исперманентфаилуре](ispermanentfailure.md)  |  [Сортвалуе](sortvalue.md)  |  [Аттемпткаунт](attemptcount.md)  |  [Ластаттемпттиме](lastattempttime.md)  |  [Аддитионалинфо](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="1efa2-111">[ItemId](itemid.md) | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount](attemptcount.md) | [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1efa2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1efa2-112">Parent elements</span></span>

[<span data-ttu-id="1efa2-113">Элементы (Аррайофнониндексаблеитемдетаилстипе)</span><span class="sxs-lookup"><span data-stu-id="1efa2-113">Items (ArrayOfNonIndexableItemDetailsType)</span></span>](items-arrayofnonindexableitemdetailstype.md)
  
## <a name="remarks"></a><span data-ttu-id="1efa2-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="1efa2-114">Remarks</span></span>

<span data-ttu-id="1efa2-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1efa2-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1efa2-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1efa2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1efa2-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1efa2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1efa2-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1efa2-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1efa2-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1efa2-119">Schema name</span></span>  <br/> |<span data-ttu-id="1efa2-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1efa2-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="1efa2-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1efa2-121">Validation file</span></span>  <br/> |<span data-ttu-id="1efa2-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1efa2-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1efa2-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1efa2-123">Can be empty</span></span>  <br/> ||
   

