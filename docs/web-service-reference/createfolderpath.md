---
title: CreateFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 282576cb-a921-49f7-8748-64158fd50c41
description: Элемент CreateFolderPath используется для создания путь к папке и включает в себя идентификатор родительской папки и относительный путь.
ms.openlocfilehash: bfe31d894cfaa0f36da2d1d0045f723e0d261759
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761875"
---
# <a name="createfolderpath"></a><span data-ttu-id="fa5d2-103">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="fa5d2-103">CreateFolderPath</span></span>

<span data-ttu-id="fa5d2-104">Элемент **CreateFolderPath** используется для создания путь к папке и включает в себя идентификатор родительской папки и относительный путь.</span><span class="sxs-lookup"><span data-stu-id="fa5d2-104">The **CreateFolderPath** element is used to create a folder path and includes a parent folder Id and a relative folder path.</span></span> 
  
```XML
<CreateFolderPath>
   <ParentFolderId/>
   <RelativeFolderPath/>
</CreateFolderPath>
```

 <span data-ttu-id="fa5d2-105">**CreateFolderPathType**</span><span class="sxs-lookup"><span data-stu-id="fa5d2-105">**CreateFolderPathType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa5d2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fa5d2-106">Attributes and elements</span></span>

<span data-ttu-id="fa5d2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fa5d2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa5d2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fa5d2-108">Attributes</span></span>

<span data-ttu-id="fa5d2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fa5d2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa5d2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fa5d2-110">Child elements</span></span>

<span data-ttu-id="fa5d2-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [RelativeFolderPath](relativefolderpath.md)</span><span class="sxs-lookup"><span data-stu-id="fa5d2-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [RelativeFolderPath](relativefolderpath.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fa5d2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fa5d2-112">Parent elements</span></span>

<span data-ttu-id="fa5d2-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="fa5d2-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fa5d2-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="fa5d2-114">Remarks</span></span>

<span data-ttu-id="fa5d2-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fa5d2-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fa5d2-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa5d2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa5d2-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fa5d2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa5d2-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fa5d2-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fa5d2-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fa5d2-119">Schema name</span></span>  <br/> |<span data-ttu-id="fa5d2-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fa5d2-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fa5d2-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fa5d2-121">Validation file</span></span>  <br/> |<span data-ttu-id="fa5d2-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fa5d2-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fa5d2-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fa5d2-123">Can be empty</span></span>  <br/> |<span data-ttu-id="fa5d2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="fa5d2-124">false</span></span>  <br/> |
   

