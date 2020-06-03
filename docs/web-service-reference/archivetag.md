---
title: арчиветаг
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: Элемент Арчиветаг указывает идентификатор хранения набора тегов архива для элемента или папки.
ms.openlocfilehash: 23167f3c96a6756fe4c6d915a4de91e815e620d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464765"
---
# <a name="archivetag"></a><span data-ttu-id="28943-103">арчиветаг</span><span class="sxs-lookup"><span data-stu-id="28943-103">ArchiveTag</span></span>

<span data-ttu-id="28943-104">Элемент **арчиветаг** указывает идентификатор хранения набора тегов архива для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="28943-104">The **ArchiveTag** element specifies the retention identifier of the archive tag set on an item or folder.</span></span> 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 <span data-ttu-id="28943-105">**ретентионтагтипе**</span><span class="sxs-lookup"><span data-stu-id="28943-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28943-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="28943-106">Attributes and elements</span></span>

<span data-ttu-id="28943-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="28943-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28943-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="28943-108">Attributes</span></span>

|<span data-ttu-id="28943-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="28943-109">**Attribute**</span></span>|<span data-ttu-id="28943-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28943-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28943-111">**Явный**</span><span class="sxs-lookup"><span data-stu-id="28943-111">**IsExplicit**</span></span> <br/> |<span data-ttu-id="28943-112">Указывает, будет ли политика хранения явно задана для элемента или папки, а также от того, унаследована ли она от родительской папки.</span><span class="sxs-lookup"><span data-stu-id="28943-112">Specifies whether the retention policy is explicitly set on an item or folder or whether it is inherited from a parent folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="28943-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="28943-113">Child elements</span></span>

<span data-ttu-id="28943-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="28943-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="28943-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="28943-115">Parent elements</span></span>

|<span data-ttu-id="28943-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28943-116">**Element**</span></span>|<span data-ttu-id="28943-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28943-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28943-118">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="28943-118">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="28943-119">Представляет папку, в которой в основном содержатся элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="28943-119">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="28943-120">календаритем</span><span class="sxs-lookup"><span data-stu-id="28943-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="28943-121">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="28943-121">Represents an Exchange calendar item.</span></span>  <br/> |
|<span data-ttu-id="28943-122">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="28943-122">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="28943-123">Представляет элемент контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="28943-123">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="28943-124">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="28943-124">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="28943-125">Представляет папку "Контакты", содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="28943-125">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="28943-126">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="28943-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="28943-127">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="28943-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="28943-128">Folder</span><span class="sxs-lookup"><span data-stu-id="28943-128">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="28943-129">Определяет папку для создания, получения, поиска, синхронизации или обновления.</span><span class="sxs-lookup"><span data-stu-id="28943-129">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="28943-130">Ресурс</span><span class="sxs-lookup"><span data-stu-id="28943-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="28943-131">Представляет общий элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="28943-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="28943-132">Сообщение</span><span class="sxs-lookup"><span data-stu-id="28943-132">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="28943-133">Представляет сообщение электронной почты Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="28943-133">Represents a Microsoft Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="28943-134">PostItem</span><span class="sxs-lookup"><span data-stu-id="28943-134">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="28943-135">Представляет элемент POST в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="28943-135">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="28943-136">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="28943-136">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="28943-137">Представляет папку поиска, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="28943-137">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="28943-138">Задача</span><span class="sxs-lookup"><span data-stu-id="28943-138">Task</span></span>](task.md) <br/> |<span data-ttu-id="28943-139">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="28943-139">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="28943-140">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="28943-140">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="28943-141">Представляет папку Tasks, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="28943-141">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28943-142">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="28943-142">Text value</span></span>

<span data-ttu-id="28943-143">Текстовое значение элемента **арчиветаг** — идентификатор GUID, определяющий политику хранения.</span><span class="sxs-lookup"><span data-stu-id="28943-143">The text value of the **ArchiveTag** element is a GUID that identifies the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="28943-144">Примечания</span><span class="sxs-lookup"><span data-stu-id="28943-144">Remarks</span></span>

<span data-ttu-id="28943-145">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="28943-145">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="28943-146">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="28943-146">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28943-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="28943-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28943-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="28943-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="28943-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="28943-149">Schema Name</span></span>  <br/> |<span data-ttu-id="28943-150">Схема типа</span><span class="sxs-lookup"><span data-stu-id="28943-150">Type schema</span></span>  <br/> |
|<span data-ttu-id="28943-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="28943-151">Validation File</span></span>  <br/> |<span data-ttu-id="28943-152">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="28943-152">types.xsd</span></span>  <br/> |
|<span data-ttu-id="28943-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="28943-153">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="28943-154">См. также</span><span class="sxs-lookup"><span data-stu-id="28943-154">See also</span></span>

- [<span data-ttu-id="28943-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="28943-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

