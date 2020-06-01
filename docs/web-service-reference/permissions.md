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
description: Элемент Permissions содержит коллекцию разрешений для папки.
ms.openlocfilehash: b8616cefdb8c453106753fb0788a6c7d6a0ded79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459218"
---
# <a name="permissions"></a><span data-ttu-id="5ea60-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ea60-103">Permissions</span></span>

<span data-ttu-id="5ea60-104">Элемент **Permissions** содержит коллекцию разрешений для папки.</span><span class="sxs-lookup"><span data-stu-id="5ea60-104">The **Permissions** element contains the collection of permissions for a folder.</span></span> 
  
```XML
<Permissions>
   <Permission/>
</Permissions>
```

 <span data-ttu-id="5ea60-105">**пермиссионтипе**</span><span class="sxs-lookup"><span data-stu-id="5ea60-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ea60-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5ea60-106">Attributes and elements</span></span>

<span data-ttu-id="5ea60-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5ea60-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ea60-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5ea60-108">Attributes</span></span>

<span data-ttu-id="5ea60-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5ea60-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ea60-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5ea60-110">Child elements</span></span>

|<span data-ttu-id="5ea60-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5ea60-111">**Element**</span></span>|<span data-ttu-id="5ea60-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5ea60-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ea60-113">Разрешение</span><span class="sxs-lookup"><span data-stu-id="5ea60-113">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="5ea60-114">Определяет доступ к папке делегата.</span><span class="sxs-lookup"><span data-stu-id="5ea60-114">Defines the access that a delegate has to a folder.</span></span> <span data-ttu-id="5ea60-115">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="5ea60-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ea60-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5ea60-116">Parent elements</span></span>

|<span data-ttu-id="5ea60-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5ea60-117">**Element**</span></span>|<span data-ttu-id="5ea60-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5ea60-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ea60-119">PermissionSet (Пермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="5ea60-119">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="5ea60-120">Содержит все разрешения, настроенные для папки.</span><span class="sxs-lookup"><span data-stu-id="5ea60-120">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="5ea60-121">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="5ea60-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5ea60-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="5ea60-122">Remarks</span></span>

<span data-ttu-id="5ea60-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5ea60-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="5ea60-124">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5ea60-124">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="5ea60-125">Различия версий</span><span class="sxs-lookup"><span data-stu-id="5ea60-125">Version differences</span></span>

<span data-ttu-id="5ea60-126">Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365, или локальной версии Exchange, начиная с Exchange 2013, разрешения для папки не возвращаются, если элемент [басешапе](baseshape.md) имеет значение **аллпропертиес** в запросе операции- [папки](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5ea60-126">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="5ea60-127">Чтобы получить разрешения для папки, добавьте элемент [PermissionSet (пермиссионсеттипе)](permissionset-permissionsettype.md) в элемент [аддитионалпропертиес](additionalproperties.md) в запросе на получение **папки** .</span><span class="sxs-lookup"><span data-stu-id="5ea60-127">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5ea60-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5ea60-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ea60-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5ea60-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5ea60-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5ea60-130">Schema Name</span></span>  <br/> |<span data-ttu-id="5ea60-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5ea60-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="5ea60-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5ea60-132">Validation File</span></span>  <br/> |<span data-ttu-id="5ea60-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5ea60-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5ea60-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5ea60-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ea60-135">False</span><span class="sxs-lookup"><span data-stu-id="5ea60-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ea60-136">См. также</span><span class="sxs-lookup"><span data-stu-id="5ea60-136">See also</span></span>



- [<span data-ttu-id="5ea60-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5ea60-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5ea60-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="5ea60-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

