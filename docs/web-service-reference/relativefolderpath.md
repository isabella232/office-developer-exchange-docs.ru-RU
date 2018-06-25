---
title: RelativeFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54e3ba52-08a6-4d48-8a44-6fd5fdbffb25
description: Элемент RelativeFolderPath содержит набор папок, которые указывают путь относительный путь к папке будет создан.
ms.openlocfilehash: f568d282e47a41c0aaf6d70ef383e5ef3e2b54bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835051"
---
# <a name="relativefolderpath"></a><span data-ttu-id="cf0b3-103">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="cf0b3-103">RelativeFolderPath</span></span>

<span data-ttu-id="cf0b3-104">Элемент **RelativeFolderPath** содержит набор папок, которые указывают путь относительный путь к папке будет создан.</span><span class="sxs-lookup"><span data-stu-id="cf0b3-104">The **RelativeFolderPath** element contains an array of folders that indicate the relative folder path of the folder path to be created.</span></span> 
  
```XML
<RelativeFolderPath>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</RelativeFolderPath>
```

 <span data-ttu-id="cf0b3-105">**NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="cf0b3-105">**NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf0b3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cf0b3-106">Attributes and elements</span></span>

<span data-ttu-id="cf0b3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cf0b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf0b3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cf0b3-108">Attributes</span></span>

<span data-ttu-id="cf0b3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf0b3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf0b3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cf0b3-110">Child elements</span></span>

<span data-ttu-id="cf0b3-111">[Папка](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span><span class="sxs-lookup"><span data-stu-id="cf0b3-111">[Folder](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf0b3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cf0b3-112">Parent elements</span></span>

[<span data-ttu-id="cf0b3-113">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="cf0b3-113">CreateFolderPath</span></span>](createfolderpath.md)
  
## <a name="remarks"></a><span data-ttu-id="cf0b3-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="cf0b3-114">Remarks</span></span>

<span data-ttu-id="cf0b3-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cf0b3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cf0b3-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf0b3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf0b3-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cf0b3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf0b3-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cf0b3-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cf0b3-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cf0b3-119">Schema name</span></span>  <br/> |<span data-ttu-id="cf0b3-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cf0b3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cf0b3-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cf0b3-121">Validation file</span></span>  <br/> |<span data-ttu-id="cf0b3-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cf0b3-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cf0b3-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cf0b3-123">Can be empty</span></span>  <br/> ||
   

