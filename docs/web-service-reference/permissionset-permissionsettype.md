---
title: PermissionSet (PermissionSetType)
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
description: Элемент PermissionSet содержит все разрешения, которые настроены для папки.
ms.openlocfilehash: 0fa0ac78a0db2bf382ad413cbb8bd072aa88c6fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834732"
---
# <a name="permissionset-permissionsettype"></a><span data-ttu-id="8a97d-103">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="8a97d-103">PermissionSet (PermissionSetType)</span></span>

<span data-ttu-id="8a97d-104">Элемент **PermissionSet** содержит все разрешения, которые настроены для папки.</span><span class="sxs-lookup"><span data-stu-id="8a97d-104">The **PermissionSet** element contains all the permissions that are configured for a folder.</span></span> 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="8a97d-105">**PermissionSetType**</span><span class="sxs-lookup"><span data-stu-id="8a97d-105">**PermissionSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a97d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8a97d-106">Attributes and elements</span></span>

<span data-ttu-id="8a97d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8a97d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a97d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8a97d-108">Attributes</span></span>

<span data-ttu-id="8a97d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8a97d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a97d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8a97d-110">Child elements</span></span>

|<span data-ttu-id="8a97d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a97d-111">**Element**</span></span>|<span data-ttu-id="8a97d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a97d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a97d-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a97d-113">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="8a97d-114">Содержит набор разрешений на папку.</span><span class="sxs-lookup"><span data-stu-id="8a97d-114">Contains the collection of permissions for a folder.</span></span> <span data-ttu-id="8a97d-115">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="8a97d-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="8a97d-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="8a97d-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="8a97d-117">Содержит массив Неизвестный записей, которые не удалось разрешить от службы каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8a97d-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="8a97d-118">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="8a97d-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a97d-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8a97d-119">Parent elements</span></span>

|<span data-ttu-id="8a97d-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a97d-120">**Element**</span></span>|<span data-ttu-id="8a97d-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a97d-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a97d-122">Folder</span><span class="sxs-lookup"><span data-stu-id="8a97d-122">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="8a97d-123">Определяет папку для создания, получение, найти, синхронизировать или обновить.</span><span class="sxs-lookup"><span data-stu-id="8a97d-123">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="8a97d-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="8a97d-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="8a97d-125">Представляет папку поиска, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8a97d-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8a97d-126">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="8a97d-126">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="8a97d-127">Представляет папку Контакты, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8a97d-127">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8a97d-128">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="8a97d-128">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="8a97d-129">Представляет папку задачи, содержащихся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="8a97d-129">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8a97d-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="8a97d-130">Remarks</span></span>

<span data-ttu-id="8a97d-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a97d-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="8a97d-132">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8a97d-132">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="8a97d-133">Различия версий</span><span class="sxs-lookup"><span data-stu-id="8a97d-133">Version differences</span></span>

<span data-ttu-id="8a97d-134">Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange 2013 разрешения папок не возвращаются при [BaseShape](baseshape.md) элемент имеет значение **AllProperties** в запросе [GetFolder](getfolder-operation.md) операции.</span><span class="sxs-lookup"><span data-stu-id="8a97d-134">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="8a97d-135">Для получения разрешений для папки, добавьте в элемент [AdditionalProperties](additionalproperties.md) в запросе **GetFolder** элемент [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) .</span><span class="sxs-lookup"><span data-stu-id="8a97d-135">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8a97d-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8a97d-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a97d-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8a97d-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a97d-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8a97d-138">Schema Name</span></span>  <br/> |<span data-ttu-id="8a97d-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8a97d-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="8a97d-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8a97d-140">Validation File</span></span>  <br/> |<span data-ttu-id="8a97d-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8a97d-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a97d-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8a97d-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a97d-143">False</span><span class="sxs-lookup"><span data-stu-id="8a97d-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a97d-144">См. также</span><span class="sxs-lookup"><span data-stu-id="8a97d-144">See also</span></span>



- [<span data-ttu-id="8a97d-145">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a97d-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="8a97d-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="8a97d-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

