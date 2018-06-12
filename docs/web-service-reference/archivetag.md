---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: Элемент ArchiveTag указывает идентификатор хранения архива тега для элемента или папки.
ms.openlocfilehash: ae9c7d512981af3bf564bcb73a9a27c5c78217fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761493"
---
# <a name="archivetag"></a><span data-ttu-id="3591d-103">ArchiveTag</span><span class="sxs-lookup"><span data-stu-id="3591d-103">ArchiveTag</span></span>

<span data-ttu-id="3591d-104">Элемент **ArchiveTag** указывает идентификатор хранения архива тега для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="3591d-104">The **ArchiveTag** element specifies the retention identifier of the archive tag set on an item or folder.</span></span> 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 <span data-ttu-id="3591d-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="3591d-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3591d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3591d-106">Attributes and elements</span></span>

<span data-ttu-id="3591d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3591d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3591d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3591d-108">Attributes</span></span>

|<span data-ttu-id="3591d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="3591d-109">**Attribute**</span></span>|<span data-ttu-id="3591d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3591d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3591d-111">**IsExplicit**</span><span class="sxs-lookup"><span data-stu-id="3591d-111">**IsExplicit**</span></span> <br/> |<span data-ttu-id="3591d-112">Указывает ли политика хранения явно задать для элемента или папки или ли наследуется от родительской папки.</span><span class="sxs-lookup"><span data-stu-id="3591d-112">Specifies whether the retention policy is explicitly set on an item or folder or whether it is inherited from a parent folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3591d-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3591d-113">Child elements</span></span>

<span data-ttu-id="3591d-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="3591d-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3591d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3591d-115">Parent elements</span></span>

|<span data-ttu-id="3591d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3591d-116">**Element**</span></span>|<span data-ttu-id="3591d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3591d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3591d-118">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="3591d-118">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="3591d-119">Представляет папку, содержащую элементы календаря в первую очередь.</span><span class="sxs-lookup"><span data-stu-id="3591d-119">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="3591d-120">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="3591d-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3591d-121">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="3591d-121">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3591d-122">Контакт</span><span class="sxs-lookup"><span data-stu-id="3591d-122">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="3591d-123">Представляет контакт в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3591d-123">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3591d-124">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="3591d-124">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="3591d-125">Представляет папку Контакты, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3591d-125">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3591d-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="3591d-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="3591d-127">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="3591d-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="3591d-128">Folder</span><span class="sxs-lookup"><span data-stu-id="3591d-128">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="3591d-129">Определяет папку для создания, получение, найти, синхронизировать или обновить.</span><span class="sxs-lookup"><span data-stu-id="3591d-129">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="3591d-130">Элемент</span><span class="sxs-lookup"><span data-stu-id="3591d-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="3591d-131">Представляет универсальный элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3591d-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3591d-132">Message</span><span class="sxs-lookup"><span data-stu-id="3591d-132">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3591d-133">Представляет сообщение электронной почты Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="3591d-133">Represents a Microsoft Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="3591d-134">PostItem</span><span class="sxs-lookup"><span data-stu-id="3591d-134">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="3591d-135">Представляет элемент post в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3591d-135">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3591d-136">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="3591d-136">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="3591d-137">Представляет папку поиска, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3591d-137">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3591d-138">Задача</span><span class="sxs-lookup"><span data-stu-id="3591d-138">Task</span></span>](task.md) <br/> |<span data-ttu-id="3591d-139">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3591d-139">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3591d-140">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="3591d-140">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="3591d-141">Представляет папку задачи, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3591d-141">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3591d-142">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3591d-142">Text value</span></span>

<span data-ttu-id="3591d-143">Текстовое значение элемента **ArchiveTag** — это идентификатор GUID, определяющий политику хранения.</span><span class="sxs-lookup"><span data-stu-id="3591d-143">The text value of the **ArchiveTag** element is a GUID that identifies the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3591d-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="3591d-144">Remarks</span></span>

<span data-ttu-id="3591d-145">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3591d-145">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3591d-146">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3591d-146">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3591d-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3591d-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3591d-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3591d-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3591d-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3591d-149">Schema Name</span></span>  <br/> |<span data-ttu-id="3591d-150">Схема типа</span><span class="sxs-lookup"><span data-stu-id="3591d-150">Type schema</span></span>  <br/> |
|<span data-ttu-id="3591d-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3591d-151">Validation File</span></span>  <br/> |<span data-ttu-id="3591d-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3591d-152">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3591d-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3591d-153">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3591d-154">См. также</span><span class="sxs-lookup"><span data-stu-id="3591d-154">See also</span></span>

- [<span data-ttu-id="3591d-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3591d-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
