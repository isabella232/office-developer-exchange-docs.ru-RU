---
title: IsFolderVisible
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderVisible
api_type:
- schema
ms.assetid: dd611fb5-9424-4ff9-bb27-c882c73c0c74
description: Элемент IsFolderVisible указывает, может ли пользователь просматривать папки. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 27a6bca9ae71bc93de6c22cb87c8d582025144e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834019"
---
# <a name="isfoldervisible"></a><span data-ttu-id="abd42-104">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="abd42-104">IsFolderVisible</span></span>

<span data-ttu-id="abd42-105">Элемент **IsFolderVisible** указывает, может ли пользователь просматривать папки.</span><span class="sxs-lookup"><span data-stu-id="abd42-105">The **IsFolderVisible** element indicates whether a user can view a folder.</span></span> <span data-ttu-id="abd42-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="abd42-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderVisible/>
```

 <span data-ttu-id="abd42-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="abd42-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="abd42-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="abd42-108">Attributes and elements</span></span>

<span data-ttu-id="abd42-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="abd42-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="abd42-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="abd42-110">Attributes</span></span>

<span data-ttu-id="abd42-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="abd42-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="abd42-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="abd42-112">Child elements</span></span>

<span data-ttu-id="abd42-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="abd42-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="abd42-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="abd42-114">Parent elements</span></span>

|<span data-ttu-id="abd42-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="abd42-115">**Element**</span></span>|<span data-ttu-id="abd42-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="abd42-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abd42-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="abd42-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="abd42-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="abd42-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="abd42-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="abd42-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="abd42-p104">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="abd42-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="abd42-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="abd42-123">Text value</span></span>

<span data-ttu-id="abd42-124">Текстовое значение **true,** указывает, что пользователь может просматривать папку.</span><span class="sxs-lookup"><span data-stu-id="abd42-124">A text value of **true** indicates that the user can view the folder.</span></span> <span data-ttu-id="abd42-125">Значение **false** указывает, что пользователь не может просматривать папку.</span><span class="sxs-lookup"><span data-stu-id="abd42-125">A value of **false** indicates that the user cannot view the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="abd42-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="abd42-126">Remarks</span></span>

<span data-ttu-id="abd42-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="abd42-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="abd42-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="abd42-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="abd42-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="abd42-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="abd42-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="abd42-130">Schema Name</span></span>  <br/> |<span data-ttu-id="abd42-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="abd42-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="abd42-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="abd42-132">Validation File</span></span>  <br/> |<span data-ttu-id="abd42-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="abd42-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="abd42-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="abd42-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="abd42-135">False</span><span class="sxs-lookup"><span data-stu-id="abd42-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="abd42-136">См. также</span><span class="sxs-lookup"><span data-stu-id="abd42-136">See also</span></span>



- [<span data-ttu-id="abd42-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="abd42-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="abd42-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="abd42-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

