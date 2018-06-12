---
title: DelegatePermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegatePermissions
api_type:
- schema
ms.assetid: 292badc7-bab3-4368-9d7c-9a8b7edb279b
description: Элемент DelegatePermissions содержит параметры делегата уровень разрешений для пользователя. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 319592b6c3386a07b3094115c335c7fb8ffe1130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762008"
---
# <a name="delegatepermissions"></a><span data-ttu-id="19a4c-104">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="19a4c-104">DelegatePermissions</span></span>

<span data-ttu-id="19a4c-105">Элемент **DelegatePermissions** содержит параметры делегата уровень разрешений для пользователя.</span><span class="sxs-lookup"><span data-stu-id="19a4c-105">The **DelegatePermissions** element contains the delegate permission-level settings for a user.</span></span> <span data-ttu-id="19a4c-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="19a4c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegatePermissions>
   <CalendarFolderPermissionLevel/>
   <TasksFolderPermissionLevel/>
   <InboxFolderPermissionLevel/>
   <ContactsFolderPermissionLevel/>
   <NotesFolderPermissionLevel/>
   <JournalFolderPermissionLevel/>
</DelegatePermissions>
```

<span data-ttu-id="19a4c-107">**DelegatePermissionsType**</span><span class="sxs-lookup"><span data-stu-id="19a4c-107">**DelegatePermissionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="19a4c-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="19a4c-108">Attributes and elements</span></span>

<span data-ttu-id="19a4c-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="19a4c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19a4c-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="19a4c-110">Attributes</span></span>

<span data-ttu-id="19a4c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="19a4c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19a4c-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="19a4c-112">Child elements</span></span>

|<span data-ttu-id="19a4c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="19a4c-113">**Element**</span></span>|<span data-ttu-id="19a4c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="19a4c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19a4c-115">CalendarFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="19a4c-115">CalendarFolderPermissionLevel</span></span>](calendarfolderpermissionlevel.md) <br/> |<span data-ttu-id="19a4c-116">Содержит разрешения для папки календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="19a4c-116">Contains the permissions for the default Calendar folder.</span></span> <span data-ttu-id="19a4c-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="19a4c-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="19a4c-118">TasksFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="19a4c-118">TasksFolderPermissionLevel</span></span>](tasksfolderpermissionlevel.md) <br/> |<span data-ttu-id="19a4c-119">Содержит разрешения для папки задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="19a4c-119">Contains the permissions for the default Task folder.</span></span> <span data-ttu-id="19a4c-120">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="19a4c-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="19a4c-121">InboxFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="19a4c-121">InboxFolderPermissionLevel</span></span>](inboxfolderpermissionlevel.md) <br/> |<span data-ttu-id="19a4c-122">Содержит разрешения для папки "Входящие" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="19a4c-122">Contains the permissions for the default Inbox folder.</span></span> <span data-ttu-id="19a4c-123">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="19a4c-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="19a4c-124">ContactsFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="19a4c-124">ContactsFolderPermissionLevel</span></span>](contactsfolderpermissionlevel.md) <br/> |<span data-ttu-id="19a4c-125">Содержит разрешения для этой папки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="19a4c-125">Contains the permissions for the default Contacts folder.</span></span> <span data-ttu-id="19a4c-126">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="19a4c-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="19a4c-127">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="19a4c-127">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md) <br/> |<span data-ttu-id="19a4c-128">Содержит разрешения для папки заметки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="19a4c-128">Contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="19a4c-129">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="19a4c-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="19a4c-130">JournalFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="19a4c-130">JournalFolderPermissionLevel</span></span>](journalfolderpermissionlevel.md) <br/> |<span data-ttu-id="19a4c-131">Содержит разрешения для папки журнала по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="19a4c-131">Contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="19a4c-132">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="19a4c-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="19a4c-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="19a4c-133">Parent elements</span></span>

|<span data-ttu-id="19a4c-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="19a4c-134">**Element**</span></span>|<span data-ttu-id="19a4c-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="19a4c-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19a4c-136">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="19a4c-136">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="19a4c-137">Определяет один делегат для добавления или обновления в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="19a4c-137">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="19a4c-138">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="19a4c-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="19a4c-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="19a4c-139">Remarks</span></span>

<span data-ttu-id="19a4c-140">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="19a4c-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19a4c-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="19a4c-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19a4c-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="19a4c-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19a4c-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="19a4c-143">Schema Name</span></span>  <br/> |<span data-ttu-id="19a4c-144">Схема Types</span><span class="sxs-lookup"><span data-stu-id="19a4c-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="19a4c-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="19a4c-145">Validation File</span></span>  <br/> |<span data-ttu-id="19a4c-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="19a4c-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19a4c-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="19a4c-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="19a4c-148">False</span><span class="sxs-lookup"><span data-stu-id="19a4c-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19a4c-149">См. также</span><span class="sxs-lookup"><span data-stu-id="19a4c-149">See also</span></span>

- [<span data-ttu-id="19a4c-150">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="19a4c-150">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="19a4c-151">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="19a4c-151">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="19a4c-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="19a4c-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="19a4c-153">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="19a4c-153">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)
