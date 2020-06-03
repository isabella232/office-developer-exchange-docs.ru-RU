---
title: исекстерналмаилбокс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5cc83174-e684-42c8-b72a-f82d3de3bb2f
description: Элемент Исекстерналмаилбокс указывает, является ли почтовый ящик внешним по отношению к Организации.
ms.openlocfilehash: 9be702b05e89857913023a8ec34b78ea4c309274
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455291"
---
# <a name="isexternalmailbox"></a><span data-ttu-id="bb444-103">исекстерналмаилбокс</span><span class="sxs-lookup"><span data-stu-id="bb444-103">IsExternalMailbox</span></span>

<span data-ttu-id="bb444-104">Элемент **исекстерналмаилбокс** указывает, является ли почтовый ящик внешним по отношению к Организации.</span><span class="sxs-lookup"><span data-stu-id="bb444-104">The **IsExternalMailbox** element indicates whether the mailbox is external to the organization.</span></span> 
  
```XML
<IsExternalMailbox>true | false</IsExternalMailbox>
```

 <span data-ttu-id="bb444-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="bb444-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb444-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bb444-106">Attributes and elements</span></span>

<span data-ttu-id="bb444-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bb444-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb444-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bb444-108">Attributes</span></span>

<span data-ttu-id="bb444-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bb444-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb444-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bb444-110">Child elements</span></span>

<span data-ttu-id="bb444-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bb444-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bb444-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bb444-112">Parent elements</span></span>

[<span data-ttu-id="bb444-113">сеарчаблемаилбокс</span><span class="sxs-lookup"><span data-stu-id="bb444-113">SearchableMailbox</span></span>](searchablemailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="bb444-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bb444-114">Text value</span></span>

<span data-ttu-id="bb444-115">Текстовое значение **true** для элемента **исекстерналмаилбокс** указывает на то, что почтовый ящик находится во внешней организации.</span><span class="sxs-lookup"><span data-stu-id="bb444-115">A text value of **true** for the **IsExternalMailbox** element indicates that the mailbox is in an external organization.</span></span> <span data-ttu-id="bb444-116">Значение **false** указывает, что почтовый ящик находится в Организации.</span><span class="sxs-lookup"><span data-stu-id="bb444-116">A value of **false** indicates that the mailbox is in the organization.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bb444-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="bb444-117">Remarks</span></span>

<span data-ttu-id="bb444-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bb444-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bb444-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb444-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb444-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bb444-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb444-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bb444-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bb444-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bb444-122">Schema name</span></span>  <br/> |<span data-ttu-id="bb444-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bb444-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="bb444-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bb444-124">Validation file</span></span>  <br/> |<span data-ttu-id="bb444-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bb444-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bb444-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bb444-126">Can be empty</span></span>  <br/> |<span data-ttu-id="bb444-127">False</span><span class="sxs-lookup"><span data-stu-id="bb444-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb444-128">См. также</span><span class="sxs-lookup"><span data-stu-id="bb444-128">See also</span></span>



- [<span data-ttu-id="bb444-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bb444-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

