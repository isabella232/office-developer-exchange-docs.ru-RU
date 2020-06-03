---
title: программатикакцессалловед
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a1fc7dff-a303-4809-b7f4-9672f86c183c
description: Элемент Программатикакцессалловед указывает, включен ли программный доступ к данным, управляемым правами.
ms.openlocfilehash: 8a5cf4e57a97807e5940a0402768d7123b9912d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465641"
---
# <a name="programmaticaccessallowed"></a><span data-ttu-id="54762-103">программатикакцессалловед</span><span class="sxs-lookup"><span data-stu-id="54762-103">ProgrammaticAccessAllowed</span></span>

<span data-ttu-id="54762-104">Элемент **программатикакцессалловед** указывает, включен ли программный доступ к данным, управляемым правами.</span><span class="sxs-lookup"><span data-stu-id="54762-104">The **ProgrammaticAccessAllowed** element specifies whether programmatic access is enabled for rights managed data.</span></span> 
  
```XML
<ProgrammaticAccessAllowed> true | false </ProgrammaticAccessAllowed>
```

 <span data-ttu-id="54762-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="54762-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54762-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="54762-106">Attributes and elements</span></span>

<span data-ttu-id="54762-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="54762-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54762-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="54762-108">Attributes</span></span>

<span data-ttu-id="54762-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="54762-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54762-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="54762-110">Child elements</span></span>

<span data-ttu-id="54762-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="54762-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="54762-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="54762-112">Parent elements</span></span>

[<span data-ttu-id="54762-113">ригхтсманажементлиценседата</span><span class="sxs-lookup"><span data-stu-id="54762-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="54762-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="54762-114">Text value</span></span>

<span data-ttu-id="54762-115">Текстовое значение **true** для элемента **программатикакцессалловед** указывает на то, что данные доступны программным способом.</span><span class="sxs-lookup"><span data-stu-id="54762-115">A text value of **true** for the **ProgrammaticAccessAllowed** element indicates that the data is programmatically accessible.</span></span> <span data-ttu-id="54762-116">Значение **false** указывает, что данные недоступны программным способом.</span><span class="sxs-lookup"><span data-stu-id="54762-116">A value of **false** indicates that the data is not programmatically accessible.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="54762-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="54762-117">Remarks</span></span>

<span data-ttu-id="54762-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="54762-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="54762-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="54762-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54762-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="54762-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54762-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="54762-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54762-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="54762-122">Schema name</span></span>  <br/> |<span data-ttu-id="54762-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="54762-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="54762-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="54762-124">Validation file</span></span>  <br/> |<span data-ttu-id="54762-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="54762-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="54762-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="54762-126">Can be empty</span></span>  <br/> |<span data-ttu-id="54762-127">false</span><span class="sxs-lookup"><span data-stu-id="54762-127">false</span></span>  <br/> |
   

