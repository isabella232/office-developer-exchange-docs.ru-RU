---
title: EffectiveRights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: Элемент EffectiveRights содержит права клиента на основании параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.
ms.openlocfilehash: 610d9e214a8de648ece667799bb5e67dfcc358f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762262"
---
# <a name="effectiverights"></a><span data-ttu-id="cadb1-104">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="cadb1-104">EffectiveRights</span></span>

<span data-ttu-id="cadb1-105">Элемент **EffectiveRights** содержит права клиента на основании параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="cadb1-105">The **EffectiveRights** element contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="cadb1-106">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cadb1-106">This element is read-only.</span></span> 
  
```XML
<EffectiveRights>
   <CreateAssociated/>
   <CreateContents/>
   <CreateHierarchy/>
   <Delete/>
   <Modify/>
   <Read/>
   <ViewPrivateItems/>
</EffectiveRights>
```

 <span data-ttu-id="cadb1-107">**EffectiveRightsType**</span><span class="sxs-lookup"><span data-stu-id="cadb1-107">**EffectiveRightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cadb1-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cadb1-108">Attributes and elements</span></span>

<span data-ttu-id="cadb1-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cadb1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cadb1-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cadb1-110">Attributes</span></span>

<span data-ttu-id="cadb1-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="cadb1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cadb1-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cadb1-112">Child elements</span></span>

|<span data-ttu-id="cadb1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cadb1-113">**Element**</span></span>|<span data-ttu-id="cadb1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cadb1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cadb1-115">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="cadb1-115">CreateAssociated</span></span>](createassociated.md) <br/> |<span data-ttu-id="cadb1-116">Указывает ли клиента можно создать таблицу связанного содержимого.</span><span class="sxs-lookup"><span data-stu-id="cadb1-116">Indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="cadb1-117">Это свойство используется только для объектов папки.</span><span class="sxs-lookup"><span data-stu-id="cadb1-117">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-118">CreateContents</span><span class="sxs-lookup"><span data-stu-id="cadb1-118">CreateContents</span></span>](createcontents.md) <br/> |<span data-ttu-id="cadb1-119">Указывает ли клиента можно создать таблицу содержимого.</span><span class="sxs-lookup"><span data-stu-id="cadb1-119">Indicates whether a client can create a contents table.</span></span> <span data-ttu-id="cadb1-120">Это свойство используется только для объектов папки.</span><span class="sxs-lookup"><span data-stu-id="cadb1-120">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-121">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="cadb1-121">CreateHierarchy</span></span>](createhierarchy.md) <br/> |<span data-ttu-id="cadb1-122">Указывает ли клиента можно создать таблицу иерархии.</span><span class="sxs-lookup"><span data-stu-id="cadb1-122">Indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="cadb1-123">Это свойство используется только для объектов папки.</span><span class="sxs-lookup"><span data-stu-id="cadb1-123">This property is only used on folder objects.</span></span>  <br/> |
|<span data-ttu-id="cadb1-124">[удаление](delete.md);</span><span class="sxs-lookup"><span data-stu-id="cadb1-124">[Delete](delete.md)</span></span> <br/> |<span data-ttu-id="cadb1-125">Указывает, будет ли это клиент можно удалить папку или элемент.</span><span class="sxs-lookup"><span data-stu-id="cadb1-125">Indicates whether a client can delete a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-126">Изменение</span><span class="sxs-lookup"><span data-stu-id="cadb1-126">Modify</span></span>](modify.md) <br/> |<span data-ttu-id="cadb1-127">Указывает, будет ли это клиент можно изменить папку или элемент.</span><span class="sxs-lookup"><span data-stu-id="cadb1-127">Indicates whether a client can modify a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-128">Чтение</span><span class="sxs-lookup"><span data-stu-id="cadb1-128">Read</span></span>](read.md) <br/> |<span data-ttu-id="cadb1-129">Указывает, будет ли это клиент могут читать папку или элемент.</span><span class="sxs-lookup"><span data-stu-id="cadb1-129">Indicates whether a client can read a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-130">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="cadb1-130">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="cadb1-131">Указывает ли закрытый элемент можно просмотреть.</span><span class="sxs-lookup"><span data-stu-id="cadb1-131">Indicates whether a private item can be viewed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cadb1-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cadb1-132">Parent elements</span></span>

|<span data-ttu-id="cadb1-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cadb1-133">**Element**</span></span>|<span data-ttu-id="cadb1-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cadb1-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cadb1-135">Folder</span><span class="sxs-lookup"><span data-stu-id="cadb1-135">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="cadb1-136">Представляет папку в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="cadb1-136">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-137">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="cadb1-137">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="cadb1-138">Представляет папку задачи в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="cadb1-138">Represents a tasks folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-139">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="cadb1-139">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="cadb1-140">Представляет папку контактов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="cadb1-140">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-141">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="cadb1-141">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="cadb1-142">Представляет папку Календарь в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="cadb1-142">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="cadb1-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="cadb1-144">Представляет папку поиска в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="cadb1-144">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-145">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="cadb1-145">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="cadb1-146">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-146">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-147">Контакт</span><span class="sxs-lookup"><span data-stu-id="cadb1-147">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="cadb1-148">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-148">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-149">DistributionList</span><span class="sxs-lookup"><span data-stu-id="cadb1-149">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="cadb1-150">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="cadb1-150">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-151">Элемент</span><span class="sxs-lookup"><span data-stu-id="cadb1-151">Item</span></span>](item.md) <br/> |<span data-ttu-id="cadb1-152">Представляет универсальный элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-152">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-153">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="cadb1-153">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="cadb1-154">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-154">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-155">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="cadb1-155">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="cadb1-156">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-156">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-157">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="cadb1-157">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="cadb1-158">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-158">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-159">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="cadb1-159">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="cadb1-160">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-160">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-161">Message</span><span class="sxs-lookup"><span data-stu-id="cadb1-161">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="cadb1-162">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-162">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-163">Задача</span><span class="sxs-lookup"><span data-stu-id="cadb1-163">Task</span></span>](task.md) <br/> |<span data-ttu-id="cadb1-164">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-164">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cadb1-165">PostItem</span><span class="sxs-lookup"><span data-stu-id="cadb1-165">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="cadb1-166">Представляет элемент post в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-166">Represents a post item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cadb1-167">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cadb1-167">Text value</span></span>

<span data-ttu-id="cadb1-168">Нет.</span><span class="sxs-lookup"><span data-stu-id="cadb1-168">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cadb1-169">Замечания</span><span class="sxs-lookup"><span data-stu-id="cadb1-169">Remarks</span></span>

<span data-ttu-id="cadb1-170">**EffectiveRights** поддерживается в ответы GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy и SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="cadb1-170">**EffectiveRights** is supported in the GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy, and SyncFolderItems responses.</span></span> <span data-ttu-id="cadb1-171">Свойство **EffectiveRights** предоставляется в фигуре **AllProperties** для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="cadb1-171">The **EffectiveRights** property is exposed in the **AllProperties** shape for folders and items.</span></span> 
  
<span data-ttu-id="cadb1-172">Это свойство **EffectiveRights** предоставляет доступ к те же данные, предоставляемая в свойстве **PR_ACCESS MAPI** .</span><span class="sxs-lookup"><span data-stu-id="cadb1-172">This **EffectiveRights** property provides access to the same information that is provided in the **PR_ACCESS MAPI** property.</span></span> 
  
<span data-ttu-id="cadb1-173">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cadb1-173">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cadb1-174">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cadb1-174">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cadb1-175">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cadb1-175">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cadb1-176">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cadb1-176">Schema Name</span></span>  <br/> |<span data-ttu-id="cadb1-177">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cadb1-177">Types schema</span></span>  <br/> |
|<span data-ttu-id="cadb1-178">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cadb1-178">Validation File</span></span>  <br/> |<span data-ttu-id="cadb1-179">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cadb1-179">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cadb1-180">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cadb1-180">Can be Empty</span></span>  <br/> |<span data-ttu-id="cadb1-181">False</span><span class="sxs-lookup"><span data-stu-id="cadb1-181">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cadb1-182">См. также</span><span class="sxs-lookup"><span data-stu-id="cadb1-182">See also</span></span>

- [<span data-ttu-id="cadb1-183">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cadb1-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="cadb1-184">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="cadb1-184">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

