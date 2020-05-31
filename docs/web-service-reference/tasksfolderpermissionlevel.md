---
title: тасксфолдерпермиссионлевел
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: Элемент Тасксфолдерпермиссионлевел содержит разрешения для папки Tasks по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 49807896f9175bafbef106c41d1c9dff8f6178c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840137"
---
# <a name="tasksfolderpermissionlevel"></a><span data-ttu-id="afaad-104">тасксфолдерпермиссионлевел</span><span class="sxs-lookup"><span data-stu-id="afaad-104">TasksFolderPermissionLevel</span></span>

<span data-ttu-id="afaad-105">Элемент **тасксфолдерпермиссионлевел** содержит разрешения для папки Tasks по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="afaad-105">The **TasksFolderPermissionLevel** element contains the permissions for the default Tasks folder.</span></span> <span data-ttu-id="afaad-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="afaad-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<TasksFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</TasksFolderPermissionLevel>
```

<span data-ttu-id="afaad-107">**делегатефолдерпермиссионлевелтипе**</span><span class="sxs-lookup"><span data-stu-id="afaad-107">**DelegateFolderPermissionLevelType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="afaad-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="afaad-108">Attributes and elements</span></span>

<span data-ttu-id="afaad-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="afaad-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afaad-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="afaad-110">Attributes</span></span>

<span data-ttu-id="afaad-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="afaad-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afaad-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="afaad-112">Child elements</span></span>

<span data-ttu-id="afaad-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="afaad-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afaad-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="afaad-114">Parent elements</span></span>

|<span data-ttu-id="afaad-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="afaad-115">**Element**</span></span>|<span data-ttu-id="afaad-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="afaad-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afaad-117">делегатепермиссионс</span><span class="sxs-lookup"><span data-stu-id="afaad-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="afaad-118">Содержит параметры уровня разрешений Delegate для пользователя.</span><span class="sxs-lookup"><span data-stu-id="afaad-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="afaad-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="afaad-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afaad-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="afaad-120">Text value</span></span>

<span data-ttu-id="afaad-121">В следующей таблице перечислены текстовые значения, представляющие уровни разрешений.</span><span class="sxs-lookup"><span data-stu-id="afaad-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="afaad-122">**Текстовые значения уровня разрешений**</span><span class="sxs-lookup"><span data-stu-id="afaad-122">**Permission level text values**</span></span>

|<span data-ttu-id="afaad-123">**Уровень разрешений**</span><span class="sxs-lookup"><span data-stu-id="afaad-123">**Permission level**</span></span>|<span data-ttu-id="afaad-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="afaad-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="afaad-125">Нет</span><span class="sxs-lookup"><span data-stu-id="afaad-125">None</span></span>  <br/> |<span data-ttu-id="afaad-126">Представитель пользователя не имеет разрешений на доступ к папке "задачи".</span><span class="sxs-lookup"><span data-stu-id="afaad-126">The delegate user has no access permissions to the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="afaad-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="afaad-127">Reviewer</span></span>  <br/> |<span data-ttu-id="afaad-128">Делегированный пользователь может читать элементы в папке "задачи".</span><span class="sxs-lookup"><span data-stu-id="afaad-128">The delegate user can read items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="afaad-129">Автор</span><span class="sxs-lookup"><span data-stu-id="afaad-129">Author</span></span>  <br/> |<span data-ttu-id="afaad-130">Делегированный пользователь может читать и создавать элементы в папке "задачи".</span><span class="sxs-lookup"><span data-stu-id="afaad-130">The delegate user can read and create items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="afaad-131">Редактор</span><span class="sxs-lookup"><span data-stu-id="afaad-131">Editor</span></span>  <br/> |<span data-ttu-id="afaad-132">Делегированный пользователь может читать, создавать и изменять элементы в папке "задачи".</span><span class="sxs-lookup"><span data-stu-id="afaad-132">The delegate user can read, create, and modify items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="afaad-133">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="afaad-133">Custom</span></span>  <br/> |<span data-ttu-id="afaad-134">Представитель пользователя имеет пользовательские разрешения на доступ к папке "задачи".</span><span class="sxs-lookup"><span data-stu-id="afaad-134">The delegate user has custom access permissions to the Tasks folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="afaad-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="afaad-135">Remarks</span></span>

<span data-ttu-id="afaad-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="afaad-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afaad-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="afaad-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afaad-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="afaad-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afaad-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="afaad-139">Schema Name</span></span>  <br/> |<span data-ttu-id="afaad-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="afaad-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="afaad-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="afaad-141">Validation File</span></span>  <br/> |<span data-ttu-id="afaad-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="afaad-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afaad-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="afaad-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="afaad-144">False</span><span class="sxs-lookup"><span data-stu-id="afaad-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afaad-145">См. также</span><span class="sxs-lookup"><span data-stu-id="afaad-145">See also</span></span>

- [<span data-ttu-id="afaad-146">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="afaad-146">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="afaad-147">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="afaad-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="afaad-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="afaad-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="afaad-149">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="afaad-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

