---
title: IsArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b89d8a78-5c18-4547-aaf4-4b16a93190a7
description: Элемент Archive указывает логическое значение, которое указывает, является ли почтовый ящик архивным.
ms.openlocfilehash: 417afd1afc25e5872d1f511feff34494fe6b7b62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833990"
---
# <a name="isarchive"></a><span data-ttu-id="8da17-103">IsArchive</span><span class="sxs-lookup"><span data-stu-id="8da17-103">IsArchive</span></span>

<span data-ttu-id="8da17-104">Элемент **Archive** указывает логическое значение, которое указывает, является ли почтовый ящик архивным.</span><span class="sxs-lookup"><span data-stu-id="8da17-104">The **IsArchive** element specifies a Boolean value that indicates whether the mailbox is an archive mailbox.</span></span> 
  
```XML
<IsArchive>true | false</IsArchive>
```

 <span data-ttu-id="8da17-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8da17-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8da17-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8da17-106">Attributes and elements</span></span>

<span data-ttu-id="8da17-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8da17-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8da17-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8da17-108">Attributes</span></span>

<span data-ttu-id="8da17-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8da17-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8da17-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8da17-110">Child elements</span></span>

<span data-ttu-id="8da17-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="8da17-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8da17-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8da17-112">Parent elements</span></span>

<span data-ttu-id="8da17-113">[Фаиледмаилбокс](failedmailbox.md) | [retentionpolicytag используется](retentionpolicytag.md)</span><span class="sxs-lookup"><span data-stu-id="8da17-113">[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="8da17-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8da17-114">Text value</span></span>

<span data-ttu-id="8da17-115">Текстовое значение **true** для элемента **Archive** указывает на то, что целевой почтовый ящик является архивным почтовым ящиком.</span><span class="sxs-lookup"><span data-stu-id="8da17-115">A text value of **true** for the **IsArchive** element indicates that the target mailbox is an archive mailbox.</span></span> <span data-ttu-id="8da17-116">Значение **false** указывает, что целевой почтовый ящик не является архивным почтовым ящиком.</span><span class="sxs-lookup"><span data-stu-id="8da17-116">A value of **false** indicates that the target mailbox is not an archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8da17-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="8da17-117">Remarks</span></span>

<span data-ttu-id="8da17-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8da17-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8da17-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8da17-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8da17-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8da17-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8da17-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8da17-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8da17-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8da17-122">Schema Name</span></span>  <br/> |<span data-ttu-id="8da17-123">Схема типа</span><span class="sxs-lookup"><span data-stu-id="8da17-123">Type schema</span></span>  <br/> |
|<span data-ttu-id="8da17-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8da17-124">Validation File</span></span>  <br/> |<span data-ttu-id="8da17-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8da17-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8da17-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8da17-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8da17-127">См. также</span><span class="sxs-lookup"><span data-stu-id="8da17-127">See also</span></span>



- [<span data-ttu-id="8da17-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8da17-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

