---
title: ProgrammaticAccessAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a1fc7dff-a303-4809-b7f4-9672f86c183c
description: Элемент ProgrammaticAccessAllowed указывает, включена ли программный доступ к для данных управляемых правами.
ms.openlocfilehash: 50bcce745bd94bf9c2e5ced93825722307e0a096
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834889"
---
# <a name="programmaticaccessallowed"></a><span data-ttu-id="5175e-103">ProgrammaticAccessAllowed</span><span class="sxs-lookup"><span data-stu-id="5175e-103">ProgrammaticAccessAllowed</span></span>

<span data-ttu-id="5175e-104">Элемент **ProgrammaticAccessAllowed** указывает, включена ли программный доступ к для данных управляемых правами.</span><span class="sxs-lookup"><span data-stu-id="5175e-104">The **ProgrammaticAccessAllowed** element specifies whether programmatic access is enabled for rights managed data.</span></span> 
  
```XML
<ProgrammaticAccessAllowed> true | false </ProgrammaticAccessAllowed>
```

 <span data-ttu-id="5175e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5175e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5175e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5175e-106">Attributes and elements</span></span>

<span data-ttu-id="5175e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5175e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5175e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5175e-108">Attributes</span></span>

<span data-ttu-id="5175e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5175e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5175e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5175e-110">Child elements</span></span>

<span data-ttu-id="5175e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5175e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5175e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5175e-112">Parent elements</span></span>

[<span data-ttu-id="5175e-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="5175e-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="5175e-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5175e-114">Text value</span></span>

<span data-ttu-id="5175e-115">Текстовое значение **true** для элемента **ProgrammaticAccessAllowed** указывает, что данные программными средствами доступен.</span><span class="sxs-lookup"><span data-stu-id="5175e-115">A text value of **true** for the **ProgrammaticAccessAllowed** element indicates that the data is programmatically accessible.</span></span> <span data-ttu-id="5175e-116">Значение **false** указывает, что данные недоступны программными средствами.</span><span class="sxs-lookup"><span data-stu-id="5175e-116">A value of **false** indicates that the data is not programmatically accessible.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5175e-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="5175e-117">Remarks</span></span>

<span data-ttu-id="5175e-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5175e-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5175e-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5175e-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5175e-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5175e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5175e-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5175e-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5175e-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5175e-122">Schema name</span></span>  <br/> |<span data-ttu-id="5175e-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5175e-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="5175e-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5175e-124">Validation file</span></span>  <br/> |<span data-ttu-id="5175e-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5175e-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5175e-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5175e-126">Can be empty</span></span>  <br/> |<span data-ttu-id="5175e-127">Нет</span><span class="sxs-lookup"><span data-stu-id="5175e-127">false</span></span>  <br/> |
   

