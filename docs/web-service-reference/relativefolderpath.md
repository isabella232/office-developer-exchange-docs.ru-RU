---
title: релативефолдерпас
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54e3ba52-08a6-4d48-8a44-6fd5fdbffb25
description: Элемент Релативефолдерпас содержит массив папок, указывающих относительный путь к папке, которую нужно создать.
ms.openlocfilehash: f568d282e47a41c0aaf6d70ef383e5ef3e2b54bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835051"
---
# <a name="relativefolderpath"></a><span data-ttu-id="09a2e-103">релативефолдерпас</span><span class="sxs-lookup"><span data-stu-id="09a2e-103">RelativeFolderPath</span></span>

<span data-ttu-id="09a2e-104">Элемент **релативефолдерпас** содержит массив папок, указывающих относительный путь к папке, которую нужно создать.</span><span class="sxs-lookup"><span data-stu-id="09a2e-104">The **RelativeFolderPath** element contains an array of folders that indicate the relative folder path of the folder path to be created.</span></span> 
  
```XML
<RelativeFolderPath>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</RelativeFolderPath>
```

 <span data-ttu-id="09a2e-105">**нонемптяррайоффолдерстипе**</span><span class="sxs-lookup"><span data-stu-id="09a2e-105">**NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09a2e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="09a2e-106">Attributes and elements</span></span>

<span data-ttu-id="09a2e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="09a2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09a2e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="09a2e-108">Attributes</span></span>

<span data-ttu-id="09a2e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="09a2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09a2e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="09a2e-110">Child elements</span></span>

<span data-ttu-id="09a2e-111">[Папка](folder.md) | [календарфолдер](calendarfolder.md) | [TasksFolder](tasksfolder.md) [SearchFolder](searchfolder.md)[ContactsFolder](contactsfolder.md)контактсфолдер SearchFolder тасксфолдер |  | </span><span class="sxs-lookup"><span data-stu-id="09a2e-111">[Folder](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09a2e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="09a2e-112">Parent elements</span></span>

[<span data-ttu-id="09a2e-113">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="09a2e-113">CreateFolderPath</span></span>](createfolderpath.md)
  
## <a name="remarks"></a><span data-ttu-id="09a2e-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="09a2e-114">Remarks</span></span>

<span data-ttu-id="09a2e-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="09a2e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="09a2e-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="09a2e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09a2e-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="09a2e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09a2e-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="09a2e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="09a2e-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="09a2e-119">Schema name</span></span>  <br/> |<span data-ttu-id="09a2e-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="09a2e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="09a2e-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="09a2e-121">Validation file</span></span>  <br/> |<span data-ttu-id="09a2e-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="09a2e-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="09a2e-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="09a2e-123">Can be empty</span></span>  <br/> ||
   

