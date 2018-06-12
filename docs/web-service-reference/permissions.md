---
title: Разрешения
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permissions
api_type:
- schema
ms.assetid: 2ba50bd9-819f-4e5f-a3bb-85a0a87d8a86
description: Элемент Permissions содержит набор разрешений на папку.
ms.openlocfilehash: 08d015c3b1afb58fce0fb4b99466965cc5c29fc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834727"
---
# <a name="permissions"></a><span data-ttu-id="80aee-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80aee-103">Permissions</span></span>

<span data-ttu-id="80aee-104">Элемент **Permissions** содержит набор разрешений на папку.</span><span class="sxs-lookup"><span data-stu-id="80aee-104">The **Permissions** element contains the collection of permissions for a folder.</span></span> 
  
```XML
<Permissions>
   <Permission/>
</Permissions>
```

 <span data-ttu-id="80aee-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="80aee-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80aee-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="80aee-106">Attributes and elements</span></span>

<span data-ttu-id="80aee-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="80aee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80aee-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="80aee-108">Attributes</span></span>

<span data-ttu-id="80aee-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="80aee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80aee-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="80aee-110">Child elements</span></span>

|<span data-ttu-id="80aee-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="80aee-111">**Element**</span></span>|<span data-ttu-id="80aee-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80aee-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80aee-113">Разрешение</span><span class="sxs-lookup"><span data-stu-id="80aee-113">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="80aee-114">Определяет доступ делегата в папку.</span><span class="sxs-lookup"><span data-stu-id="80aee-114">Defines the access that a delegate has to a folder.</span></span> <span data-ttu-id="80aee-115">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="80aee-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="80aee-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="80aee-116">Parent elements</span></span>

|<span data-ttu-id="80aee-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="80aee-117">**Element**</span></span>|<span data-ttu-id="80aee-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80aee-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80aee-119">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="80aee-119">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="80aee-120">Содержит все разрешения, которые настроены для папки.</span><span class="sxs-lookup"><span data-stu-id="80aee-120">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="80aee-121">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="80aee-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="80aee-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="80aee-122">Remarks</span></span>

<span data-ttu-id="80aee-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="80aee-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="80aee-124">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="80aee-124">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="80aee-125">Различия версий</span><span class="sxs-lookup"><span data-stu-id="80aee-125">Version differences</span></span>

<span data-ttu-id="80aee-126">Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange 2013 разрешения папок не возвращаются при [BaseShape](baseshape.md) элемент имеет значение **AllProperties** в запросе [GetFolder](getfolder-operation.md) операции.</span><span class="sxs-lookup"><span data-stu-id="80aee-126">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="80aee-127">Для получения разрешений для папки, добавьте в элемент [AdditionalProperties](additionalproperties.md) в запросе **GetFolder** элемент [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) .</span><span class="sxs-lookup"><span data-stu-id="80aee-127">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="80aee-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="80aee-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80aee-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="80aee-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80aee-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="80aee-130">Schema Name</span></span>  <br/> |<span data-ttu-id="80aee-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="80aee-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="80aee-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="80aee-132">Validation File</span></span>  <br/> |<span data-ttu-id="80aee-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="80aee-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80aee-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="80aee-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="80aee-135">False</span><span class="sxs-lookup"><span data-stu-id="80aee-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80aee-136">См. также</span><span class="sxs-lookup"><span data-stu-id="80aee-136">See also</span></span>



- [<span data-ttu-id="80aee-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="80aee-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="80aee-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="80aee-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

