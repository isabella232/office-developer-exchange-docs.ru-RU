---
title: ModifyRecipientsAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f25e673-0df0-4285-bf03-a083a395cdab
description: Элемент ModifyRecipientsAllowed указывает, включена ли изменения из получателей.
ms.openlocfilehash: 2b07c7fa8e6b5872621c8b019b60584abbf98e3c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834473"
---
# <a name="modifyrecipientsallowed"></a><span data-ttu-id="59910-103">ModifyRecipientsAllowed</span><span class="sxs-lookup"><span data-stu-id="59910-103">ModifyRecipientsAllowed</span></span>

<span data-ttu-id="59910-104">Элемент **ModifyRecipientsAllowed** указывает, включена ли изменения из получателей.</span><span class="sxs-lookup"><span data-stu-id="59910-104">The **ModifyRecipientsAllowed** element specifies whether modification of the recipients is enabled.</span></span> 
  
```XML
<ModifyRecipientsAllowed> true | false </ModifyRecipientsAllowed>
```

 <span data-ttu-id="59910-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="59910-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59910-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="59910-106">Attributes and elements</span></span>

<span data-ttu-id="59910-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="59910-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59910-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="59910-108">Attributes</span></span>

<span data-ttu-id="59910-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="59910-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59910-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="59910-110">Child elements</span></span>

<span data-ttu-id="59910-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="59910-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59910-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="59910-112">Parent elements</span></span>

[<span data-ttu-id="59910-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="59910-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="59910-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="59910-114">Text value</span></span>

<span data-ttu-id="59910-115">Текстовое значение **true** для элемента **ModifyRecipientsAllowed** указывает, что список получателей элемента можно изменить для элемента с помощью управления правами на его.</span><span class="sxs-lookup"><span data-stu-id="59910-115">A text value of **true** for the **ModifyRecipientsAllowed** element indicates that the item recipient list is modifiable for an item with rights management enabled on it.</span></span> <span data-ttu-id="59910-116">Значение **false** указывает, что список получателей не является изменяемым.</span><span class="sxs-lookup"><span data-stu-id="59910-116">A value of **false** indicates that the recipient list is not modifiable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="59910-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="59910-117">Remarks</span></span>

<span data-ttu-id="59910-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="59910-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="59910-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="59910-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59910-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="59910-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59910-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="59910-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59910-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="59910-122">Schema name</span></span>  <br/> |<span data-ttu-id="59910-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="59910-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="59910-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="59910-124">Validation file</span></span>  <br/> |<span data-ttu-id="59910-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="59910-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59910-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="59910-126">Can be empty</span></span>  <br/> ||
   

