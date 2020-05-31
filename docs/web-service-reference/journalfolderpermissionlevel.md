---
title: жаурналфолдерпермиссионлевел
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- JournalFolderPermissionLevel
api_type:
- schema
ms.assetid: 564525fa-cd95-4c1a-9d6c-3806be664579
description: Элемент Жаурналфолдерпермиссионлевел содержит разрешения для папки журнала по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 030c2682fd6eaaf46c8be04e8357c285296816cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834184"
---
# <a name="journalfolderpermissionlevel"></a><span data-ttu-id="b31e5-104">жаурналфолдерпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="b31e5-104">JournalFolderPermissionLevel</span></span>

<span data-ttu-id="b31e5-105">Элемент **жаурналфолдерпермиссионлевел** содержит разрешения для папки журнала по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b31e5-105">The **JournalFolderPermissionLevel** element contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="b31e5-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b31e5-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<JournalFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</JournalFolderPermissionLevel>
```

 <span data-ttu-id="b31e5-107">**делегатефолдерпермиссионлевелтипе**</span><span class="sxs-lookup"><span data-stu-id="b31e5-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b31e5-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b31e5-108">Attributes and elements</span></span>

<span data-ttu-id="b31e5-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b31e5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b31e5-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b31e5-110">Attributes</span></span>

<span data-ttu-id="b31e5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b31e5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b31e5-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b31e5-112">Child elements</span></span>

<span data-ttu-id="b31e5-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="b31e5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b31e5-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b31e5-114">Parent elements</span></span>

|<span data-ttu-id="b31e5-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b31e5-115">**Element**</span></span>|<span data-ttu-id="b31e5-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b31e5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b31e5-117">делегатепермиссионс</span><span class="sxs-lookup"><span data-stu-id="b31e5-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="b31e5-118">Содержит параметры уровня разрешений Delegate для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b31e5-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="b31e5-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="b31e5-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b31e5-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b31e5-120">Text value</span></span>

<span data-ttu-id="b31e5-121">В следующей таблице перечислены текстовые значения, представляющие уровни разрешений.</span><span class="sxs-lookup"><span data-stu-id="b31e5-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="b31e5-122">**Текстовые значения уровня разрешений**</span><span class="sxs-lookup"><span data-stu-id="b31e5-122">**Permission level text values**</span></span>

|<span data-ttu-id="b31e5-123">**Уровень разрешений**</span><span class="sxs-lookup"><span data-stu-id="b31e5-123">**Permission level**</span></span>|<span data-ttu-id="b31e5-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b31e5-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b31e5-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b31e5-125">None</span></span>  <br/> |<span data-ttu-id="b31e5-126">Представитель пользователя не имеет разрешений на доступ к папке журнала.</span><span class="sxs-lookup"><span data-stu-id="b31e5-126">The delegate user has no access permissions to the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="b31e5-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="b31e5-127">Reviewer</span></span>  <br/> |<span data-ttu-id="b31e5-128">Делегированный пользователь может читать элементы в папке "Дневник".</span><span class="sxs-lookup"><span data-stu-id="b31e5-128">The delegate user can read items in the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="b31e5-129">Автор</span><span class="sxs-lookup"><span data-stu-id="b31e5-129">Author</span></span>  <br/> |<span data-ttu-id="b31e5-130">Делегированный пользователь может читать и создавать элементы в папке "Дневник".</span><span class="sxs-lookup"><span data-stu-id="b31e5-130">The delegate user can read and create items in the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="b31e5-131">Редактор</span><span class="sxs-lookup"><span data-stu-id="b31e5-131">Editor</span></span>  <br/> |<span data-ttu-id="b31e5-132">Делегированный пользователь может читать, создавать и изменять элементы в папке "Дневник".</span><span class="sxs-lookup"><span data-stu-id="b31e5-132">The delegate user can read, create, and modify items in the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="b31e5-133">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="b31e5-133">Custom</span></span>  <br/> |<span data-ttu-id="b31e5-134">Представитель пользователя имеет пользовательские разрешения на доступ к папке журнала.</span><span class="sxs-lookup"><span data-stu-id="b31e5-134">The delegate user has custom access permissions to the Journal folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b31e5-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="b31e5-135">Remarks</span></span>

<span data-ttu-id="b31e5-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b31e5-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b31e5-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b31e5-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b31e5-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b31e5-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b31e5-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b31e5-139">Schema Name</span></span>  <br/> |<span data-ttu-id="b31e5-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b31e5-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="b31e5-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b31e5-141">Validation File</span></span>  <br/> |<span data-ttu-id="b31e5-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b31e5-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b31e5-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b31e5-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="b31e5-144">False</span><span class="sxs-lookup"><span data-stu-id="b31e5-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b31e5-145">См. также</span><span class="sxs-lookup"><span data-stu-id="b31e5-145">See also</span></span>



[<span data-ttu-id="b31e5-146">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="b31e5-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="b31e5-147">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="b31e5-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="b31e5-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b31e5-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="b31e5-149">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="b31e5-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

