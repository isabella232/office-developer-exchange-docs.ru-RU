---
title: CreateFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 282576cb-a921-49f7-8748-64158fd50c41
description: Элемент CreateFolderPath используется для создания пути к папке и включает идентификатор родительской папки и относительный путь к папке.
ms.openlocfilehash: e6ce6c9b6e12a6a0fb6792b63368a79c87d06f07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457538"
---
# <a name="createfolderpath"></a><span data-ttu-id="74989-103">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="74989-103">CreateFolderPath</span></span>

<span data-ttu-id="74989-104">Элемент **CreateFolderPath** используется для создания пути к папке и включает идентификатор родительской папки и относительный путь к папке.</span><span class="sxs-lookup"><span data-stu-id="74989-104">The **CreateFolderPath** element is used to create a folder path and includes a parent folder Id and a relative folder path.</span></span> 
  
```XML
<CreateFolderPath>
   <ParentFolderId/>
   <RelativeFolderPath/>
</CreateFolderPath>
```

 <span data-ttu-id="74989-105">**креатефолдерпастипе**</span><span class="sxs-lookup"><span data-stu-id="74989-105">**CreateFolderPathType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74989-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="74989-106">Attributes and elements</span></span>

<span data-ttu-id="74989-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="74989-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74989-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="74989-108">Attributes</span></span>

<span data-ttu-id="74989-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="74989-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74989-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="74989-110">Child elements</span></span>

<span data-ttu-id="74989-111">[ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md)  |  [Релативефолдерпас](relativefolderpath.md)</span><span class="sxs-lookup"><span data-stu-id="74989-111">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [RelativeFolderPath](relativefolderpath.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="74989-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="74989-112">Parent elements</span></span>

<span data-ttu-id="74989-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="74989-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74989-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="74989-114">Remarks</span></span>

<span data-ttu-id="74989-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="74989-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="74989-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="74989-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74989-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="74989-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74989-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="74989-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74989-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="74989-119">Schema name</span></span>  <br/> |<span data-ttu-id="74989-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="74989-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74989-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="74989-121">Validation file</span></span>  <br/> |<span data-ttu-id="74989-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="74989-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74989-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="74989-123">Can be empty</span></span>  <br/> |<span data-ttu-id="74989-124">false</span><span class="sxs-lookup"><span data-stu-id="74989-124">false</span></span>  <br/> |
   

