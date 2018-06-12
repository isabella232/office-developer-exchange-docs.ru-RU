---
title: FolderClass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderClass
api_type:
- schema
ms.assetid: 0041d135-2869-4612-89a5-d1aa86aa1093
description: Элемент FolderClass представляет класс папки для папки.
ms.openlocfilehash: 87be00563d0375abebf32159ff38d62d03112b95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762616"
---
# <a name="folderclass"></a><span data-ttu-id="dd692-103">FolderClass</span><span class="sxs-lookup"><span data-stu-id="dd692-103">FolderClass</span></span>

<span data-ttu-id="dd692-104">Элемент **FolderClass** представляет класс папки для папки.</span><span class="sxs-lookup"><span data-stu-id="dd692-104">The **FolderClass** element represents the folder class for a folder.</span></span> 
  
```xml
<FolderClass/>
```

 <span data-ttu-id="dd692-105">**string**</span><span class="sxs-lookup"><span data-stu-id="dd692-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd692-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dd692-106">Attributes and elements</span></span>

<span data-ttu-id="dd692-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dd692-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd692-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dd692-108">Attributes</span></span>

<span data-ttu-id="dd692-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd692-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd692-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dd692-110">Child elements</span></span>

<span data-ttu-id="dd692-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd692-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd692-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dd692-112">Parent elements</span></span>

|<span data-ttu-id="dd692-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dd692-113">**Element**</span></span>|<span data-ttu-id="dd692-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd692-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd692-115">Folder</span><span class="sxs-lookup"><span data-stu-id="dd692-115">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="dd692-116">Представляет папку в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="dd692-116">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="dd692-117">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="dd692-117">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="dd692-118">Представляет папку Календарь в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="dd692-118">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="dd692-119">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="dd692-119">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="dd692-120">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="dd692-120">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="dd692-121">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="dd692-121">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="dd692-122">Представляет папку поиска в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="dd692-122">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="dd692-123">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="dd692-123">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="dd692-124">Представляет папку задач в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="dd692-124">Represents a task folder in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd692-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dd692-125">Text value</span></span>

<span data-ttu-id="dd692-126">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="dd692-126">A text value is required.</span></span> <span data-ttu-id="dd692-127">Папка классов обычно начинаются с «IPF.»</span><span class="sxs-lookup"><span data-stu-id="dd692-127">Folder classes typically start with "IPF."</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd692-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="dd692-128">Remarks</span></span>

<span data-ttu-id="dd692-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dd692-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd692-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dd692-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd692-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dd692-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd692-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dd692-132">Schema Name</span></span>  <br/> |<span data-ttu-id="dd692-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dd692-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd692-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dd692-134">Validation File</span></span>  <br/> |<span data-ttu-id="dd692-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dd692-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd692-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dd692-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd692-137">False</span><span class="sxs-lookup"><span data-stu-id="dd692-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd692-138">См. также</span><span class="sxs-lookup"><span data-stu-id="dd692-138">See also</span></span>



- [<span data-ttu-id="dd692-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dd692-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

