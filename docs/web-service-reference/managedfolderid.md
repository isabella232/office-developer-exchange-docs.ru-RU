---
title: ManagedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderId
api_type:
- schema
ms.assetid: 3efb7abb-0e91-4d8a-9fa2-3dec8bd17c30
description: Элемент ManagedFolderId содержит идентификатор папки из управляемых папок.
ms.openlocfilehash: acdb69f82678633baff12c46494c39015c36d233
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834340"
---
# <a name="managedfolderid"></a><span data-ttu-id="24f54-103">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="24f54-103">ManagedFolderId</span></span>

<span data-ttu-id="24f54-104">Элемент **ManagedFolderId** содержит идентификатор папки из управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="24f54-104">The **ManagedFolderId** element contains the folder ID of the managed folder.</span></span> 
  
```xml
<ManagedFolderId/>
```

 <span data-ttu-id="24f54-105">**string**</span><span class="sxs-lookup"><span data-stu-id="24f54-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24f54-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="24f54-106">Attributes and elements</span></span>

<span data-ttu-id="24f54-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="24f54-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24f54-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="24f54-108">Attributes</span></span>

<span data-ttu-id="24f54-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="24f54-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24f54-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="24f54-110">Child elements</span></span>

<span data-ttu-id="24f54-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="24f54-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="24f54-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="24f54-112">Parent elements</span></span>

|<span data-ttu-id="24f54-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="24f54-113">**Element**</span></span>|<span data-ttu-id="24f54-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24f54-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24f54-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="24f54-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="24f54-116">Содержит сведения об управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="24f54-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="24f54-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="24f54-117">Text value</span></span>

<span data-ttu-id="24f54-118">Для этого элемента требуется указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="24f54-118">A text value is required for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="24f54-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="24f54-119">Remarks</span></span>

<span data-ttu-id="24f54-120">Значение идентификатора **ManagedFolderId** является эквивалентом свойство **Guid** , получаемых `Get-ManagedFolder` команду Microsoft Windows Powershell.</span><span class="sxs-lookup"><span data-stu-id="24f54-120">The **ManagedFolderId** identifier value is the equivalent of the **Guid** property that is retrieved by the  `Get-ManagedFolder` Microsoft Windows Powershell command.</span></span> <span data-ttu-id="24f54-121">Это значение атрибута **objectGUID** для управляемой папки в службе каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="24f54-121">It is also the value of the **objectGUID** attribute for the managed folder in the Active Directory directory service.</span></span> 
  
<span data-ttu-id="24f54-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="24f54-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24f54-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="24f54-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24f54-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="24f54-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="24f54-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="24f54-125">Schema name</span></span>  <br/> |<span data-ttu-id="24f54-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="24f54-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="24f54-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="24f54-127">Validation file</span></span>  <br/> |<span data-ttu-id="24f54-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="24f54-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="24f54-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="24f54-129">Can be empty</span></span>  <br/> |<span data-ttu-id="24f54-130">False</span><span class="sxs-lookup"><span data-stu-id="24f54-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24f54-131">См. также</span><span class="sxs-lookup"><span data-stu-id="24f54-131">See also</span></span>



[<span data-ttu-id="24f54-132">Операция CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="24f54-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="24f54-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="24f54-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="24f54-134">Удаление папок</span><span class="sxs-lookup"><span data-stu-id="24f54-134">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)
  
[<span data-ttu-id="24f54-135">Добавление управляемых папок</span><span class="sxs-lookup"><span data-stu-id="24f54-135">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

