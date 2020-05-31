---
title: HasAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: Элемент HasAttachment указывает логическое значение, указывающее, имеет ли элемент вложения.
ms.openlocfilehash: dfe163e0850e835784a43984a34c89f14bfbc59b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833798"
---
# <a name="hasattachment"></a><span data-ttu-id="563e3-103">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="563e3-103">HasAttachment</span></span>

<span data-ttu-id="563e3-104">Элемент **HasAttachment** указывает логическое значение, указывающее, имеет ли элемент вложения.</span><span class="sxs-lookup"><span data-stu-id="563e3-104">The **HasAttachment** element specifies a Boolean value to indicate whether the item has attachments.</span></span> 
  
```XML
<HasAttachment> true | false </HasAttachment
```

 <span data-ttu-id="563e3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="563e3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="563e3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="563e3-106">Attributes and elements</span></span>

<span data-ttu-id="563e3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="563e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="563e3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="563e3-108">Attributes</span></span>

<span data-ttu-id="563e3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="563e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="563e3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="563e3-110">Child elements</span></span>

<span data-ttu-id="563e3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="563e3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="563e3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="563e3-112">Parent elements</span></span>

|<span data-ttu-id="563e3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="563e3-113">**Element**</span></span>|<span data-ttu-id="563e3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="563e3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="563e3-115">сеарчпревиевитем</span><span class="sxs-lookup"><span data-stu-id="563e3-115">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="563e3-116">Задает первые 256 символов элемента почтового ящика для предварительного просмотра без открытия элемента.</span><span class="sxs-lookup"><span data-stu-id="563e3-116">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="563e3-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="563e3-117">Text value</span></span>

<span data-ttu-id="563e3-118">Текстовое значение **true** для элемента **HasAttachment** указывает на то, что элемент имеет вложение.</span><span class="sxs-lookup"><span data-stu-id="563e3-118">A text value of **true** for the **HasAttachment** element indicates that the item has an attachment.</span></span> <span data-ttu-id="563e3-119">Значение **false** указывает на то, что элемент не имеет вложения.</span><span class="sxs-lookup"><span data-stu-id="563e3-119">A value of **false** indicates that the item does not have an attachment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="563e3-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="563e3-120">Remarks</span></span>

<span data-ttu-id="563e3-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="563e3-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="563e3-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="563e3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="563e3-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="563e3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="563e3-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="563e3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="563e3-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="563e3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="563e3-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="563e3-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="563e3-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="563e3-127">Validation File</span></span>  <br/> |<span data-ttu-id="563e3-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="563e3-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="563e3-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="563e3-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="563e3-130">См. также</span><span class="sxs-lookup"><span data-stu-id="563e3-130">See also</span></span>



- [<span data-ttu-id="563e3-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="563e3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

