---
title: нотесфолдерпермиссионлевел
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotesFolderPermissionLevel
api_type:
- schema
ms.assetid: 76a2520c-f453-4fd7-b3eb-1c5f4666680a
description: Элемент Нотесфолдерпермиссионлевел содержит разрешения для папки заметок по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 205802592a1fc01451b4fc497e9e0c4c66afd478
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462628"
---
# <a name="notesfolderpermissionlevel"></a><span data-ttu-id="28feb-104">нотесфолдерпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="28feb-104">NotesFolderPermissionLevel</span></span>

<span data-ttu-id="28feb-105">Элемент **нотесфолдерпермиссионлевел** содержит разрешения для папки заметок по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="28feb-105">The **NotesFolderPermissionLevel** element contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="28feb-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="28feb-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<NotesFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</NotesFolderPermissionLevel>
```

 <span data-ttu-id="28feb-107">**делегатефолдерпермиссионлевелтипе**</span><span class="sxs-lookup"><span data-stu-id="28feb-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28feb-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="28feb-108">Attributes and elements</span></span>

<span data-ttu-id="28feb-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="28feb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28feb-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="28feb-110">Attributes</span></span>

<span data-ttu-id="28feb-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="28feb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28feb-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="28feb-112">Child elements</span></span>

<span data-ttu-id="28feb-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="28feb-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="28feb-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="28feb-114">Parent elements</span></span>

|<span data-ttu-id="28feb-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28feb-115">**Element**</span></span>|<span data-ttu-id="28feb-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28feb-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28feb-117">делегатепермиссионс</span><span class="sxs-lookup"><span data-stu-id="28feb-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="28feb-118">Содержит параметры уровня разрешений Delegate для пользователя.</span><span class="sxs-lookup"><span data-stu-id="28feb-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="28feb-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="28feb-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28feb-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="28feb-120">Text value</span></span>

<span data-ttu-id="28feb-121">В следующей таблице перечислены текстовые значения, представляющие уровни разрешений.</span><span class="sxs-lookup"><span data-stu-id="28feb-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="28feb-122">**Текстовые значения уровня разрешений**</span><span class="sxs-lookup"><span data-stu-id="28feb-122">**Permission level text values**</span></span>

|<span data-ttu-id="28feb-123">**Уровень разрешений**</span><span class="sxs-lookup"><span data-stu-id="28feb-123">**Permission level**</span></span>|<span data-ttu-id="28feb-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28feb-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28feb-125">Нет</span><span class="sxs-lookup"><span data-stu-id="28feb-125">None</span></span>  <br/> |<span data-ttu-id="28feb-126">Представитель пользователя не имеет разрешений на доступ к папке Notes.</span><span class="sxs-lookup"><span data-stu-id="28feb-126">The delegate user has no access permissions to the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="28feb-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="28feb-127">Reviewer</span></span>  <br/> |<span data-ttu-id="28feb-128">Делегированный пользователь может читать элементы в папке "Заметки".</span><span class="sxs-lookup"><span data-stu-id="28feb-128">The delegate user can read items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="28feb-129">Автор</span><span class="sxs-lookup"><span data-stu-id="28feb-129">Author</span></span>  <br/> |<span data-ttu-id="28feb-130">Делегированный пользователь может читать и создавать элементы в папке "Заметки".</span><span class="sxs-lookup"><span data-stu-id="28feb-130">The delegate user can read and create items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="28feb-131">Корректор</span><span class="sxs-lookup"><span data-stu-id="28feb-131">Editor</span></span>  <br/> |<span data-ttu-id="28feb-132">Делегированный пользователь может читать, создавать и изменять элементы в папке "Заметки".</span><span class="sxs-lookup"><span data-stu-id="28feb-132">The delegate user can read, create, and modify items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="28feb-133">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="28feb-133">Custom</span></span>  <br/> |<span data-ttu-id="28feb-134">Представитель пользователя имеет пользовательские разрешения на доступ к папке Notes.</span><span class="sxs-lookup"><span data-stu-id="28feb-134">The delegate user has custom access permissions to the Notes folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="28feb-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="28feb-135">Remarks</span></span>

<span data-ttu-id="28feb-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="28feb-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28feb-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="28feb-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28feb-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="28feb-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="28feb-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="28feb-139">Schema Name</span></span>  <br/> |<span data-ttu-id="28feb-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="28feb-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="28feb-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="28feb-141">Validation File</span></span>  <br/> |<span data-ttu-id="28feb-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="28feb-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="28feb-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="28feb-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="28feb-144">False</span><span class="sxs-lookup"><span data-stu-id="28feb-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28feb-145">См. также</span><span class="sxs-lookup"><span data-stu-id="28feb-145">See also</span></span>



[<span data-ttu-id="28feb-146">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="28feb-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="28feb-147">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="28feb-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="28feb-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="28feb-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="28feb-149">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="28feb-149">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

