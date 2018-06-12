---
title: IsWritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: Элемент IsWritable указывает, можно ли запись базовым контакт или получателя Active Directory для.
ms.openlocfilehash: 03f258d01ecfc12dfa4e09ac88f4a75340d2acf3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834158"
---
# <a name="iswritable"></a><span data-ttu-id="66449-103">IsWritable</span><span class="sxs-lookup"><span data-stu-id="66449-103">IsWritable</span></span>

<span data-ttu-id="66449-104">Элемент **IsWritable** указывает, можно ли запись базовым контакт или получателя Active Directory для.</span><span class="sxs-lookup"><span data-stu-id="66449-104">The **IsWritable** element specifies whether the underlying contact or Active Directory recipient can be written to.</span></span> 
  
```XML
<IsWritable> true | false </IsWritable>
```

 <span data-ttu-id="66449-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="66449-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66449-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="66449-106">Attributes and elements</span></span>

<span data-ttu-id="66449-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="66449-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66449-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="66449-108">Attributes</span></span>

<span data-ttu-id="66449-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="66449-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66449-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="66449-110">Child elements</span></span>

<span data-ttu-id="66449-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="66449-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66449-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="66449-112">Parent elements</span></span>

[<span data-ttu-id="66449-113">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="66449-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
  
## <a name="text-value"></a><span data-ttu-id="66449-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="66449-114">Text value</span></span>

<span data-ttu-id="66449-115">Текстовое значение **true** для элемента **IsWritable** указывает, что контакт или объект Active Directory для доступа на запись.</span><span class="sxs-lookup"><span data-stu-id="66449-115">A text value of **true** for the **IsWritable** element indicates that the contact or Active Directory object is available for write access.</span></span> <span data-ttu-id="66449-116">Значение **false** указывает, что контакт или объект Active Directory недоступна для записи.</span><span class="sxs-lookup"><span data-stu-id="66449-116">A value of **false** indicates that the contact or Active Directory object is not available for write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="66449-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="66449-117">Remarks</span></span>

<span data-ttu-id="66449-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="66449-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="66449-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="66449-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

