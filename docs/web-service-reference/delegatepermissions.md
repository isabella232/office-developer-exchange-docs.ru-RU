---
title: делегатепермиссионс
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
description: Элемент Делегатепермиссионс содержит параметры делегированного уровня разрешений для пользователя. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 2cf8c9a8d3c5db8e13d43c207df173c12fca5acb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457412"
---
# <a name="delegatepermissions"></a><span data-ttu-id="af596-104">делегатепермиссионс</span><span class="sxs-lookup"><span data-stu-id="af596-104">DelegatePermissions</span></span>

<span data-ttu-id="af596-105">Элемент **делегатепермиссионс** содержит параметры делегированного уровня разрешений для пользователя.</span><span class="sxs-lookup"><span data-stu-id="af596-105">The **DelegatePermissions** element contains the delegate permission-level settings for a user.</span></span> <span data-ttu-id="af596-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="af596-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
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

<span data-ttu-id="af596-107">**делегатепермиссионстипе**</span><span class="sxs-lookup"><span data-stu-id="af596-107">**DelegatePermissionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="af596-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="af596-108">Attributes and elements</span></span>

<span data-ttu-id="af596-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="af596-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af596-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="af596-110">Attributes</span></span>

<span data-ttu-id="af596-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="af596-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af596-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="af596-112">Child elements</span></span>

|<span data-ttu-id="af596-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="af596-113">**Element**</span></span>|<span data-ttu-id="af596-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="af596-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af596-115">календарфолдерпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="af596-115">CalendarFolderPermissionLevel</span></span>](calendarfolderpermissionlevel.md) <br/> |<span data-ttu-id="af596-116">Содержит разрешения для папки календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af596-116">Contains the permissions for the default Calendar folder.</span></span> <span data-ttu-id="af596-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="af596-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="af596-118">тасксфолдерпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="af596-118">TasksFolderPermissionLevel</span></span>](tasksfolderpermissionlevel.md) <br/> |<span data-ttu-id="af596-119">Содержит разрешения для папки задач по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af596-119">Contains the permissions for the default Task folder.</span></span> <span data-ttu-id="af596-120">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="af596-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="af596-121">инбоксфолдерпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="af596-121">InboxFolderPermissionLevel</span></span>](inboxfolderpermissionlevel.md) <br/> |<span data-ttu-id="af596-122">Содержит разрешения для папки "Входящие", используемой по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af596-122">Contains the permissions for the default Inbox folder.</span></span> <span data-ttu-id="af596-123">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="af596-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="af596-124">контактсфолдерпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="af596-124">ContactsFolderPermissionLevel</span></span>](contactsfolderpermissionlevel.md) <br/> |<span data-ttu-id="af596-125">Содержит разрешения для папки "Контакты" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af596-125">Contains the permissions for the default Contacts folder.</span></span> <span data-ttu-id="af596-126">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="af596-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="af596-127">нотесфолдерпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="af596-127">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md) <br/> |<span data-ttu-id="af596-128">Содержит разрешения для папки заметок по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af596-128">Contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="af596-129">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="af596-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="af596-130">жаурналфолдерпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="af596-130">JournalFolderPermissionLevel</span></span>](journalfolderpermissionlevel.md) <br/> |<span data-ttu-id="af596-131">Содержит разрешения для папки журнала по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af596-131">Contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="af596-132">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="af596-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af596-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="af596-133">Parent elements</span></span>

|<span data-ttu-id="af596-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="af596-134">**Element**</span></span>|<span data-ttu-id="af596-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="af596-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af596-136">делегатеусер</span><span class="sxs-lookup"><span data-stu-id="af596-136">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="af596-137">Определяет одного делегата для добавления или обновления в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="af596-137">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="af596-138">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="af596-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="af596-139">Примечания</span><span class="sxs-lookup"><span data-stu-id="af596-139">Remarks</span></span>

<span data-ttu-id="af596-140">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="af596-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af596-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="af596-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af596-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="af596-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af596-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="af596-143">Schema Name</span></span>  <br/> |<span data-ttu-id="af596-144">Схема Types</span><span class="sxs-lookup"><span data-stu-id="af596-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="af596-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="af596-145">Validation File</span></span>  <br/> |<span data-ttu-id="af596-146">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="af596-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af596-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="af596-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="af596-148">False</span><span class="sxs-lookup"><span data-stu-id="af596-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af596-149">См. также</span><span class="sxs-lookup"><span data-stu-id="af596-149">See also</span></span>

- [<span data-ttu-id="af596-150">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="af596-150">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="af596-151">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="af596-151">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="af596-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="af596-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="af596-153">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="af596-153">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

