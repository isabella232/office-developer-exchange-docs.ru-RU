---
title: UnknownEntries
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownEntries
api_type:
- schema
ms.assetid: 107ec73e-083a-4956-9d37-33d4734cc157
description: Элемент UnknownEntries содержит массив объектов Неизвестный разрешений, которые не удалось разрешить от службы каталогов Active Directory. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 306e5f226a56694bb1ff32362f77e7dff80865ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840296"
---
# <a name="unknownentries"></a><span data-ttu-id="92dfa-104">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="92dfa-104">UnknownEntries</span></span>

<span data-ttu-id="92dfa-105">Элемент **UnknownEntries** содержит массив объектов Неизвестный разрешений, которые не удалось разрешить от службы каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="92dfa-105">The **UnknownEntries** element contains an array of unknown permission entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="92dfa-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="92dfa-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntries>
   <UnknownEntry/>
</UnknownEntries>
```

 <span data-ttu-id="92dfa-107">**ArrayOfUnknownEntriesType**</span><span class="sxs-lookup"><span data-stu-id="92dfa-107">**ArrayOfUnknownEntriesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92dfa-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="92dfa-108">Attributes and elements</span></span>

<span data-ttu-id="92dfa-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="92dfa-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92dfa-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="92dfa-110">Attributes</span></span>

<span data-ttu-id="92dfa-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="92dfa-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92dfa-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="92dfa-112">Child elements</span></span>

|<span data-ttu-id="92dfa-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="92dfa-113">**Element**</span></span>|<span data-ttu-id="92dfa-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="92dfa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92dfa-115">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="92dfa-115">UnknownEntry</span></span>](unknownentry.md) <br/> |<span data-ttu-id="92dfa-116">Представляет элемент одного Неизвестный разрешения, который не удается разрешить с Active Directory.</span><span class="sxs-lookup"><span data-stu-id="92dfa-116">Represents a single unknown permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="92dfa-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="92dfa-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92dfa-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="92dfa-118">Parent elements</span></span>

|<span data-ttu-id="92dfa-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="92dfa-119">**Element**</span></span>|<span data-ttu-id="92dfa-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="92dfa-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92dfa-121">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="92dfa-121">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="92dfa-122">Содержит все разрешения, которые настроены для папки.</span><span class="sxs-lookup"><span data-stu-id="92dfa-122">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="92dfa-123">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="92dfa-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="92dfa-124">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="92dfa-124">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="92dfa-125">Содержит все разрешения, которые настроены для папки «Календарь».</span><span class="sxs-lookup"><span data-stu-id="92dfa-125">Contains all the permissions that are configured for a calendar folder.</span></span> <span data-ttu-id="92dfa-126">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="92dfa-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="92dfa-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="92dfa-127">Remarks</span></span>

<span data-ttu-id="92dfa-128">Неизвестный записи можно удалить из папки с помощью операции UpdateFolder элемент [SetFolderField](setfolderfield.md) .</span><span class="sxs-lookup"><span data-stu-id="92dfa-128">You can delete unknown entries from a folder by using the UpdateFolder operation with the [SetFolderField](setfolderfield.md) element.</span></span> <span data-ttu-id="92dfa-129">Неизвестный записи будут удалены при сбросе PermissionSet с помощью параметра SetFolderField UpdateFolder операции.</span><span class="sxs-lookup"><span data-stu-id="92dfa-129">The unknown entries are deleted when you reset the PermissionSet by using the SetFolderField option of the UpdateFolder operation.</span></span> <span data-ttu-id="92dfa-130">Веб-служб Exchange не поддерживает удаление отдельных операций.</span><span class="sxs-lookup"><span data-stu-id="92dfa-130">Exchange Web Services does not support the deletion of individual entries.</span></span> 
  
<span data-ttu-id="92dfa-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="92dfa-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92dfa-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="92dfa-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92dfa-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="92dfa-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92dfa-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="92dfa-134">Schema Name</span></span>  <br/> |<span data-ttu-id="92dfa-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="92dfa-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="92dfa-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="92dfa-136">Validation File</span></span>  <br/> |<span data-ttu-id="92dfa-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="92dfa-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92dfa-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="92dfa-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="92dfa-139">False</span><span class="sxs-lookup"><span data-stu-id="92dfa-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92dfa-140">См. также</span><span class="sxs-lookup"><span data-stu-id="92dfa-140">See also</span></span>



[<span data-ttu-id="92dfa-141">Операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="92dfa-141">UpdateFolder operation</span></span>](updatefolder-operation.md)


- [<span data-ttu-id="92dfa-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="92dfa-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="92dfa-143">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="92dfa-143">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

