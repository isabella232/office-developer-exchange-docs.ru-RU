---
title: ункновнентриес
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
description: Элемент Ункновнентриес содержит массив неизвестных записей разрешений, которые не удается разрешить в службе каталогов Active Directory. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 306e5f226a56694bb1ff32362f77e7dff80865ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840296"
---
# <a name="unknownentries"></a><span data-ttu-id="15b62-104">ункновнентриес</span><span class="sxs-lookup"><span data-stu-id="15b62-104">UnknownEntries</span></span>

<span data-ttu-id="15b62-105">Элемент **ункновнентриес** содержит массив неизвестных записей разрешений, которые не удается разрешить в службе каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="15b62-105">The **UnknownEntries** element contains an array of unknown permission entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="15b62-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="15b62-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntries>
   <UnknownEntry/>
</UnknownEntries>
```

 <span data-ttu-id="15b62-107">**аррайофункновнентриестипе**</span><span class="sxs-lookup"><span data-stu-id="15b62-107">**ArrayOfUnknownEntriesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15b62-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="15b62-108">Attributes and elements</span></span>

<span data-ttu-id="15b62-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="15b62-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15b62-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="15b62-110">Attributes</span></span>

<span data-ttu-id="15b62-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="15b62-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15b62-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="15b62-112">Child elements</span></span>

|<span data-ttu-id="15b62-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="15b62-113">**Element**</span></span>|<span data-ttu-id="15b62-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15b62-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15b62-115">ункновнентри</span><span class="sxs-lookup"><span data-stu-id="15b62-115">UnknownEntry</span></span>](unknownentry.md) <br/> |<span data-ttu-id="15b62-116">Представляет одну неизвестную запись разрешения, которая не может быть разрешена в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="15b62-116">Represents a single unknown permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="15b62-117">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="15b62-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="15b62-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="15b62-118">Parent elements</span></span>

|<span data-ttu-id="15b62-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="15b62-119">**Element**</span></span>|<span data-ttu-id="15b62-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15b62-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15b62-121">PermissionSet (Пермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="15b62-121">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="15b62-122">Содержит все разрешения, настроенные для папки.</span><span class="sxs-lookup"><span data-stu-id="15b62-122">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="15b62-123">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="15b62-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="15b62-124">PermissionSet (Календарпермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="15b62-124">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="15b62-125">Содержит все разрешения, настроенные для папки календаря.</span><span class="sxs-lookup"><span data-stu-id="15b62-125">Contains all the permissions that are configured for a calendar folder.</span></span> <span data-ttu-id="15b62-126">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="15b62-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="15b62-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="15b62-127">Remarks</span></span>

<span data-ttu-id="15b62-128">Вы можете удалять неизвестные записи из папки с помощью операции операцию UpdateFolder с элементом [сетфолдерфиелд](setfolderfield.md) .</span><span class="sxs-lookup"><span data-stu-id="15b62-128">You can delete unknown entries from a folder by using the UpdateFolder operation with the [SetFolderField](setfolderfield.md) element.</span></span> <span data-ttu-id="15b62-129">Неизвестные записи удаляются при сбросе набора разрешений с помощью параметра Сетфолдерфиелд операции операцию UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="15b62-129">The unknown entries are deleted when you reset the PermissionSet by using the SetFolderField option of the UpdateFolder operation.</span></span> <span data-ttu-id="15b62-130">Веб-службы Exchange не поддерживают удаление отдельных записей.</span><span class="sxs-lookup"><span data-stu-id="15b62-130">Exchange Web Services does not support the deletion of individual entries.</span></span> 
  
<span data-ttu-id="15b62-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="15b62-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15b62-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="15b62-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15b62-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="15b62-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15b62-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="15b62-134">Schema Name</span></span>  <br/> |<span data-ttu-id="15b62-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="15b62-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="15b62-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="15b62-136">Validation File</span></span>  <br/> |<span data-ttu-id="15b62-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="15b62-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15b62-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="15b62-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="15b62-139">False</span><span class="sxs-lookup"><span data-stu-id="15b62-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15b62-140">См. также</span><span class="sxs-lookup"><span data-stu-id="15b62-140">See also</span></span>



[<span data-ttu-id="15b62-141">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="15b62-141">UpdateFolder operation</span></span>](updatefolder-operation.md)


- [<span data-ttu-id="15b62-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="15b62-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="15b62-143">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="15b62-143">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

