---
title: еффективеригхтс
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
description: Элемент Еффективеригхтс содержит права клиента в зависимости от параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.
ms.openlocfilehash: 3055eb73056750508b48ead29136b56e7ce97ee9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459246"
---
# <a name="effectiverights"></a><span data-ttu-id="81f5e-104">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="81f5e-104">EffectiveRights</span></span>

<span data-ttu-id="81f5e-105">Элемент **еффективеригхтс** содержит права клиента в зависимости от параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="81f5e-105">The **EffectiveRights** element contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="81f5e-106">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81f5e-106">This element is read-only.</span></span> 
  
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

 <span data-ttu-id="81f5e-107">**еффективеригхтстипе**</span><span class="sxs-lookup"><span data-stu-id="81f5e-107">**EffectiveRightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81f5e-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="81f5e-108">Attributes and elements</span></span>

<span data-ttu-id="81f5e-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="81f5e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81f5e-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="81f5e-110">Attributes</span></span>

<span data-ttu-id="81f5e-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="81f5e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81f5e-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="81f5e-112">Child elements</span></span>

|<span data-ttu-id="81f5e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81f5e-113">**Element**</span></span>|<span data-ttu-id="81f5e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81f5e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81f5e-115">креатеассоЦиатед</span><span class="sxs-lookup"><span data-stu-id="81f5e-115">CreateAssociated</span></span>](createassociated.md) <br/> |<span data-ttu-id="81f5e-116">Указывает, может ли клиент создать связанную таблицу содержимого.</span><span class="sxs-lookup"><span data-stu-id="81f5e-116">Indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="81f5e-117">Это свойство используется только для объектов Folder.</span><span class="sxs-lookup"><span data-stu-id="81f5e-117">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-118">креатеконтентс</span><span class="sxs-lookup"><span data-stu-id="81f5e-118">CreateContents</span></span>](createcontents.md) <br/> |<span data-ttu-id="81f5e-119">Указывает, может ли клиент создать таблицу содержимого.</span><span class="sxs-lookup"><span data-stu-id="81f5e-119">Indicates whether a client can create a contents table.</span></span> <span data-ttu-id="81f5e-120">Это свойство используется только для объектов Folder.</span><span class="sxs-lookup"><span data-stu-id="81f5e-120">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-121">креатехиерарчи</span><span class="sxs-lookup"><span data-stu-id="81f5e-121">CreateHierarchy</span></span>](createhierarchy.md) <br/> |<span data-ttu-id="81f5e-122">Указывает, может ли клиент создать таблицу иерархии.</span><span class="sxs-lookup"><span data-stu-id="81f5e-122">Indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="81f5e-123">Это свойство используется только для объектов Folder.</span><span class="sxs-lookup"><span data-stu-id="81f5e-123">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-124">Удаление</span><span class="sxs-lookup"><span data-stu-id="81f5e-124">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="81f5e-125">Указывает, может ли клиент удалить папку или элемент.</span><span class="sxs-lookup"><span data-stu-id="81f5e-125">Indicates whether a client can delete a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-126">Modify</span><span class="sxs-lookup"><span data-stu-id="81f5e-126">Modify</span></span>](modify.md) <br/> |<span data-ttu-id="81f5e-127">Указывает, может ли клиент изменить папку или элемент.</span><span class="sxs-lookup"><span data-stu-id="81f5e-127">Indicates whether a client can modify a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-128">Read</span><span class="sxs-lookup"><span data-stu-id="81f5e-128">Read</span></span>](read.md) <br/> |<span data-ttu-id="81f5e-129">Указывает, может ли клиент прочитать папку или элемент.</span><span class="sxs-lookup"><span data-stu-id="81f5e-129">Indicates whether a client can read a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-130">виевприватеитемс</span><span class="sxs-lookup"><span data-stu-id="81f5e-130">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="81f5e-131">Указывает, можно ли просматривать закрытый элемент.</span><span class="sxs-lookup"><span data-stu-id="81f5e-131">Indicates whether a private item can be viewed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="81f5e-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="81f5e-132">Parent elements</span></span>

|<span data-ttu-id="81f5e-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81f5e-133">**Element**</span></span>|<span data-ttu-id="81f5e-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81f5e-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81f5e-135">Folder</span><span class="sxs-lookup"><span data-stu-id="81f5e-135">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="81f5e-136">Представляет папку в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="81f5e-136">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-137">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="81f5e-137">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="81f5e-138">Представляет папку Tasks в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="81f5e-138">Represents a tasks folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-139">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="81f5e-139">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="81f5e-140">Представляет папку "Контакты" в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="81f5e-140">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-141">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="81f5e-141">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="81f5e-142">Представляет папку "Календарь" в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="81f5e-142">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="81f5e-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="81f5e-144">Представляет папку поиска в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="81f5e-144">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-145">календаритем</span><span class="sxs-lookup"><span data-stu-id="81f5e-145">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="81f5e-146">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-146">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-147">Контакт</span><span class="sxs-lookup"><span data-stu-id="81f5e-147">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="81f5e-148">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-148">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-149">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="81f5e-149">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="81f5e-150">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="81f5e-150">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-151">Ресурс</span><span class="sxs-lookup"><span data-stu-id="81f5e-151">Item</span></span>](item.md) <br/> |<span data-ttu-id="81f5e-152">Представляет общий элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-152">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-153">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="81f5e-153">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="81f5e-154">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-154">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-155">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="81f5e-155">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="81f5e-156">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-156">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-157">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="81f5e-157">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="81f5e-158">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-158">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-159">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="81f5e-159">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="81f5e-160">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-160">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-161">Message</span><span class="sxs-lookup"><span data-stu-id="81f5e-161">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="81f5e-162">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-162">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-163">Задача</span><span class="sxs-lookup"><span data-stu-id="81f5e-163">Task</span></span>](task.md) <br/> |<span data-ttu-id="81f5e-164">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-164">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="81f5e-165">PostItem</span><span class="sxs-lookup"><span data-stu-id="81f5e-165">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="81f5e-166">Представляет элемент POST в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-166">Represents a post item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="81f5e-167">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="81f5e-167">Text value</span></span>

<span data-ttu-id="81f5e-168">Нет.</span><span class="sxs-lookup"><span data-stu-id="81f5e-168">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="81f5e-169">Примечания</span><span class="sxs-lookup"><span data-stu-id="81f5e-169">Remarks</span></span>

<span data-ttu-id="81f5e-170">**Еффективеригхтс** поддерживается в ответах на GetItem, GetItem, FindFolder, FindItem, SyncFolderHierarchy и SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="81f5e-170">**EffectiveRights** is supported in the GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy, and SyncFolderItems responses.</span></span> <span data-ttu-id="81f5e-171">Свойство **еффективеригхтс** отображается в фигуре **аллпропертиес** для папок и элементов.</span><span class="sxs-lookup"><span data-stu-id="81f5e-171">The **EffectiveRights** property is exposed in the **AllProperties** shape for folders and items.</span></span> 
  
<span data-ttu-id="81f5e-172">Это свойство **еффективеригхтс** предоставляет доступ к тем же сведениям, что и в свойстве **MAPI PR_ACCESS** .</span><span class="sxs-lookup"><span data-stu-id="81f5e-172">This **EffectiveRights** property provides access to the same information that is provided in the **PR_ACCESS MAPI** property.</span></span> 
  
<span data-ttu-id="81f5e-173">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f5e-173">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81f5e-174">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="81f5e-174">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81f5e-175">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="81f5e-175">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="81f5e-176">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="81f5e-176">Schema Name</span></span>  <br/> |<span data-ttu-id="81f5e-177">Схема Types</span><span class="sxs-lookup"><span data-stu-id="81f5e-177">Types schema</span></span>  <br/> |
|<span data-ttu-id="81f5e-178">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="81f5e-178">Validation File</span></span>  <br/> |<span data-ttu-id="81f5e-179">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="81f5e-179">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="81f5e-180">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="81f5e-180">Can be Empty</span></span>  <br/> |<span data-ttu-id="81f5e-181">False</span><span class="sxs-lookup"><span data-stu-id="81f5e-181">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81f5e-182">См. также</span><span class="sxs-lookup"><span data-stu-id="81f5e-182">See also</span></span>

- [<span data-ttu-id="81f5e-183">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="81f5e-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="81f5e-184">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="81f5e-184">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

