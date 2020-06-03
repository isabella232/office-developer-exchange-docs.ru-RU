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
ms.openlocfilehash: 6d0be0eb283de3f4d8f786ff96f4a0d4f49e2009
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526517"
---
# <a name="isarchive"></a><span data-ttu-id="c6859-103">IsArchive</span><span class="sxs-lookup"><span data-stu-id="c6859-103">IsArchive</span></span>

<span data-ttu-id="c6859-104">Элемент **Archive** указывает логическое значение, которое указывает, является ли почтовый ящик архивным.</span><span class="sxs-lookup"><span data-stu-id="c6859-104">The **IsArchive** element specifies a Boolean value that indicates whether the mailbox is an archive mailbox.</span></span> 
  
```XML
<IsArchive>true | false</IsArchive>
```

 <span data-ttu-id="c6859-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c6859-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6859-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c6859-106">Attributes and elements</span></span>

<span data-ttu-id="c6859-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c6859-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6859-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c6859-108">Attributes</span></span>

<span data-ttu-id="c6859-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c6859-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6859-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c6859-110">Child elements</span></span>

<span data-ttu-id="c6859-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c6859-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c6859-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c6859-112">Parent elements</span></span>

<span data-ttu-id="c6859-113">[Фаиледмаилбокс](failedmailbox.md)  |  [Retentionpolicytag используется](retentionpolicytag.md)</span><span class="sxs-lookup"><span data-stu-id="c6859-113">[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c6859-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c6859-114">Text value</span></span>

<span data-ttu-id="c6859-115">Текстовое значение **true** для элемента **Archive** указывает на то, что целевой почтовый ящик является архивным почтовым ящиком.</span><span class="sxs-lookup"><span data-stu-id="c6859-115">A text value of **true** for the **IsArchive** element indicates that the target mailbox is an archive mailbox.</span></span> <span data-ttu-id="c6859-116">Значение **false** указывает, что целевой почтовый ящик не является архивным почтовым ящиком.</span><span class="sxs-lookup"><span data-stu-id="c6859-116">A value of **false** indicates that the target mailbox is not an archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c6859-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="c6859-117">Remarks</span></span>

<span data-ttu-id="c6859-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c6859-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c6859-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6859-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6859-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c6859-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6859-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c6859-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c6859-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c6859-122">Schema Name</span></span>  <br/> |<span data-ttu-id="c6859-123">Схема типа</span><span class="sxs-lookup"><span data-stu-id="c6859-123">Type schema</span></span>  <br/> |
|<span data-ttu-id="c6859-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c6859-124">Validation File</span></span>  <br/> |<span data-ttu-id="c6859-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c6859-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c6859-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c6859-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c6859-127">См. также</span><span class="sxs-lookup"><span data-stu-id="c6859-127">See also</span></span>



- [<span data-ttu-id="c6859-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c6859-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

