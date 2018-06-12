---
title: HasChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 15ff513d-f39e-44ed-a13f-ab3f86fa37e1
description: Элемент HasChanged указывает, изменился ли фото пользователя.
ms.openlocfilehash: b0129e3d3acb43ada16a824e3d21706999d7053c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833802"
---
# <a name="haschanged"></a><span data-ttu-id="b126e-103">HasChanged</span><span class="sxs-lookup"><span data-stu-id="b126e-103">HasChanged</span></span>

<span data-ttu-id="b126e-104">Элемент **HasChanged** указывает, изменился ли фото пользователя.</span><span class="sxs-lookup"><span data-stu-id="b126e-104">The **HasChanged** element indicates whether a user's photo has changed.</span></span> 
  
```XML
<HasChanged> true | false </HasChanged>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="b126e-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b126e-105">Attributes and elements</span></span>

<span data-ttu-id="b126e-106">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b126e-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b126e-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b126e-107">Attributes</span></span>

<span data-ttu-id="b126e-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="b126e-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b126e-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b126e-109">Child elements</span></span>

<span data-ttu-id="b126e-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="b126e-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b126e-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b126e-111">Parent elements</span></span>

[<span data-ttu-id="b126e-112">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="b126e-112">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
  
## <a name="text-value"></a><span data-ttu-id="b126e-113">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b126e-113">Text value</span></span>

<span data-ttu-id="b126e-114">Текстовое значение **true** для элемента **HasChanged** указывает, что фотографию изменился с момента последнего был возвращен.</span><span class="sxs-lookup"><span data-stu-id="b126e-114">A text value of **true** for the **HasChanged** element indicates that the photo has changed since the last time it was returned.</span></span> <span data-ttu-id="b126e-115">Значение **false** указывает, что фотографии не был изменен после последнего выполнения, который был возвращен.</span><span class="sxs-lookup"><span data-stu-id="b126e-115">A value of **false** indicates that the photo has not changed since the last time it was returned.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b126e-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="b126e-116">Remarks</span></span>

<span data-ttu-id="b126e-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b126e-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b126e-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b126e-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b126e-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b126e-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b126e-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b126e-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b126e-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b126e-121">Schema name</span></span>  <br/> |<span data-ttu-id="b126e-122">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b126e-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="b126e-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b126e-123">Validation file</span></span>  <br/> |<span data-ttu-id="b126e-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b126e-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b126e-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b126e-125">Can be empty</span></span>  <br/> ||
   

