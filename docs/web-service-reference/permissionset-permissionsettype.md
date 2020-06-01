---
title: PermissionSet (Пермиссионсеттипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d
description: Элемент PermissionSet содержит все разрешения, настроенные для папки.
ms.openlocfilehash: 5639ee8ba64742f39c0274f4e3aaa76d75bea42b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468133"
---
# <a name="permissionset-permissionsettype"></a><span data-ttu-id="b18f6-103">PermissionSet (Пермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="b18f6-103">PermissionSet (PermissionSetType)</span></span>

<span data-ttu-id="b18f6-104">Элемент **PermissionSet** содержит все разрешения, настроенные для папки.</span><span class="sxs-lookup"><span data-stu-id="b18f6-104">The **PermissionSet** element contains all the permissions that are configured for a folder.</span></span> 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="b18f6-105">**пермиссионсеттипе**</span><span class="sxs-lookup"><span data-stu-id="b18f6-105">**PermissionSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b18f6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b18f6-106">Attributes and elements</span></span>

<span data-ttu-id="b18f6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b18f6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b18f6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b18f6-108">Attributes</span></span>

<span data-ttu-id="b18f6-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b18f6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b18f6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b18f6-110">Child elements</span></span>

|<span data-ttu-id="b18f6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b18f6-111">**Element**</span></span>|<span data-ttu-id="b18f6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b18f6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b18f6-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b18f6-113">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="b18f6-114">Содержит коллекцию разрешений для папки.</span><span class="sxs-lookup"><span data-stu-id="b18f6-114">Contains the collection of permissions for a folder.</span></span> <span data-ttu-id="b18f6-115">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="b18f6-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="b18f6-116">ункновнентриес</span><span class="sxs-lookup"><span data-stu-id="b18f6-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="b18f6-117">Содержит массив неизвестных записей, которые не удается разрешить в службе каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b18f6-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="b18f6-118">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="b18f6-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b18f6-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b18f6-119">Parent elements</span></span>

|<span data-ttu-id="b18f6-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b18f6-120">**Element**</span></span>|<span data-ttu-id="b18f6-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b18f6-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b18f6-122">Folder</span><span class="sxs-lookup"><span data-stu-id="b18f6-122">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="b18f6-123">Определяет папку для создания, получения, поиска, синхронизации или обновления.</span><span class="sxs-lookup"><span data-stu-id="b18f6-123">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="b18f6-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="b18f6-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="b18f6-125">Представляет папку поиска, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b18f6-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b18f6-126">контактсфолдер</span><span class="sxs-lookup"><span data-stu-id="b18f6-126">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="b18f6-127">Представляет папку "Контакты", содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b18f6-127">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="b18f6-128">тасксфолдер</span><span class="sxs-lookup"><span data-stu-id="b18f6-128">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="b18f6-129">Представляет папку Tasks, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b18f6-129">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b18f6-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="b18f6-130">Remarks</span></span>

<span data-ttu-id="b18f6-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b18f6-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="b18f6-132">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b18f6-132">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="b18f6-133">Различия версий</span><span class="sxs-lookup"><span data-stu-id="b18f6-133">Version differences</span></span>

<span data-ttu-id="b18f6-134">Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365, или локальной версии Exchange, начиная с Exchange 2013, разрешения для папки не возвращаются, если элемент [басешапе](baseshape.md) имеет значение **аллпропертиес** в запросе операции- [папки](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b18f6-134">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="b18f6-135">Чтобы получить разрешения для папки, добавьте элемент [PermissionSet (пермиссионсеттипе)](permissionset-permissionsettype.md) в элемент [аддитионалпропертиес](additionalproperties.md) в запросе на получение **папки** .</span><span class="sxs-lookup"><span data-stu-id="b18f6-135">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b18f6-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b18f6-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b18f6-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b18f6-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b18f6-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b18f6-138">Schema Name</span></span>  <br/> |<span data-ttu-id="b18f6-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b18f6-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="b18f6-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b18f6-140">Validation File</span></span>  <br/> |<span data-ttu-id="b18f6-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b18f6-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b18f6-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b18f6-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="b18f6-143">False</span><span class="sxs-lookup"><span data-stu-id="b18f6-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b18f6-144">См. также</span><span class="sxs-lookup"><span data-stu-id="b18f6-144">See also</span></span>



- [<span data-ttu-id="b18f6-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b18f6-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="b18f6-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="b18f6-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

