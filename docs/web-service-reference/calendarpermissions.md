---
title: календарпермиссионс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissions
api_type:
- schema
ms.assetid: 9b659d83-45fb-42a2-b052-5bc4dbe3854d
description: Элемент Календарпермиссионс содержит массив разрешений календаря для папки. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: f072339212d0fdff3983fbfb6bc8f53c272350c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529471"
---
# <a name="calendarpermissions"></a><span data-ttu-id="a2549-104">календарпермиссионс</span><span class="sxs-lookup"><span data-stu-id="a2549-104">CalendarPermissions</span></span>

<span data-ttu-id="a2549-105">Элемент **календарпермиссионс** содержит массив разрешений календаря для папки.</span><span class="sxs-lookup"><span data-stu-id="a2549-105">The **CalendarPermissions** element contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="a2549-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a2549-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissions>
   <PermissionSet/>
</CalendarPermissions>
```

 <span data-ttu-id="a2549-107">**аррайофкалендарпермиссионстипе**</span><span class="sxs-lookup"><span data-stu-id="a2549-107">**ArrayOfCalendarPermissionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2549-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2549-108">Attributes and elements</span></span>

<span data-ttu-id="a2549-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a2549-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2549-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2549-110">Attributes</span></span>

<span data-ttu-id="a2549-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a2549-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2549-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2549-112">Child elements</span></span>

|<span data-ttu-id="a2549-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2549-113">**Element**</span></span>|<span data-ttu-id="a2549-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2549-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2549-115">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="a2549-115">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="a2549-116">Определяет доступ пользователя, который является представителем, к папке календаря.</span><span class="sxs-lookup"><span data-stu-id="a2549-116">Defines the access that a delegate user has to a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2549-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2549-117">Parent elements</span></span>

|<span data-ttu-id="a2549-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2549-118">**Element**</span></span>|<span data-ttu-id="a2549-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2549-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2549-120">PermissionSet (Календарпермиссионсеттипе)</span><span class="sxs-lookup"><span data-stu-id="a2549-120">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="a2549-121">Содержит все настроенные разрешения для папки "Календарь".</span><span class="sxs-lookup"><span data-stu-id="a2549-121">Contains all the configured permissions for a calendar folder.</span></span> <span data-ttu-id="a2549-122">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="a2549-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2549-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="a2549-123">Remarks</span></span>

<span data-ttu-id="a2549-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a2549-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2549-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a2549-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2549-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a2549-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2549-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a2549-127">Schema Name</span></span>  <br/> |<span data-ttu-id="a2549-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a2549-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2549-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a2549-129">Validation File</span></span>  <br/> |<span data-ttu-id="a2549-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a2549-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2549-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a2549-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2549-132">False</span><span class="sxs-lookup"><span data-stu-id="a2549-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2549-133">См. также</span><span class="sxs-lookup"><span data-stu-id="a2549-133">See also</span></span>



- [<span data-ttu-id="a2549-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a2549-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a2549-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="a2549-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

