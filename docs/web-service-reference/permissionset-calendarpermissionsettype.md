---
title: PermissionSet (Календарпермиссионсеттипе)
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
ms.assetid: 75f20033-85eb-4627-b4f8-be85e4889e96
description: Элемент PermissionSet содержит все разрешения, настроенные для папки календаря.
ms.openlocfilehash: b2e642fd2ee8ded4d0d4c67509a5587f7b1efa8a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834728"
---
# <a name="permissionset-calendarpermissionsettype"></a><span data-ttu-id="4fb79-103">PermissionSet (Календарпермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="4fb79-103">PermissionSet (CalendarPermissionSetType)</span></span>

<span data-ttu-id="4fb79-104">Элемент **PermissionSet** содержит все разрешения, настроенные для папки календаря.</span><span class="sxs-lookup"><span data-stu-id="4fb79-104">The **PermissionSet** element contains all the permissions that are configured for a calendar folder.</span></span> 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="4fb79-105">**календарпермиссонсеттипе**</span><span class="sxs-lookup"><span data-stu-id="4fb79-105">**CalendarPermissonSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fb79-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4fb79-106">Attributes and elements</span></span>

<span data-ttu-id="4fb79-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4fb79-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fb79-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4fb79-108">Attributes</span></span>

<span data-ttu-id="4fb79-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4fb79-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fb79-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4fb79-110">Child elements</span></span>

|<span data-ttu-id="4fb79-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4fb79-111">**Element**</span></span>|<span data-ttu-id="4fb79-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4fb79-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fb79-113">календарпермиссионс</span><span class="sxs-lookup"><span data-stu-id="4fb79-113">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="4fb79-114">Содержит массив разрешений календаря для папки.</span><span class="sxs-lookup"><span data-stu-id="4fb79-114">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="4fb79-115">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="4fb79-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4fb79-116">ункновнентриес</span><span class="sxs-lookup"><span data-stu-id="4fb79-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="4fb79-117">Содержит массив неизвестных записей, которые не удается разрешить в службе каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4fb79-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="4fb79-118">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="4fb79-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4fb79-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4fb79-119">Parent elements</span></span>

|<span data-ttu-id="4fb79-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4fb79-120">**Element**</span></span>|<span data-ttu-id="4fb79-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4fb79-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fb79-122">календарфолдер</span><span class="sxs-lookup"><span data-stu-id="4fb79-122">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="4fb79-123">Представляет папку, в которой в основном содержатся элементы календаря.</span><span class="sxs-lookup"><span data-stu-id="4fb79-123">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4fb79-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="4fb79-124">Remarks</span></span>

<span data-ttu-id="4fb79-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fb79-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="4fb79-126">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4fb79-126">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="4fb79-127">Различия версий</span><span class="sxs-lookup"><span data-stu-id="4fb79-127">Version differences</span></span>

<span data-ttu-id="4fb79-128">Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365, или локальной версии Exchange, начиная с Exchange 2013, разрешения для папки не возвращаются, если элемент [басешапе](baseshape.md) имеет значение **аллпропертиес** в запросе операции- [папки](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4fb79-128">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="4fb79-129">Чтобы получить разрешения для папки, добавьте элемент [PermissionSet (пермиссионсеттипе)](permissionset-permissionsettype.md) в элемент [аддитионалпропертиес](additionalproperties.md) в запросе на получение **папки** .</span><span class="sxs-lookup"><span data-stu-id="4fb79-129">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="4fb79-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4fb79-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fb79-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4fb79-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4fb79-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4fb79-132">Schema Name</span></span>  <br/> |<span data-ttu-id="4fb79-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4fb79-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="4fb79-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4fb79-134">Validation File</span></span>  <br/> |<span data-ttu-id="4fb79-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4fb79-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4fb79-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4fb79-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="4fb79-137">False</span><span class="sxs-lookup"><span data-stu-id="4fb79-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fb79-138">См. также</span><span class="sxs-lookup"><span data-stu-id="4fb79-138">See also</span></span>



- [<span data-ttu-id="4fb79-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4fb79-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="4fb79-140">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="4fb79-140">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

