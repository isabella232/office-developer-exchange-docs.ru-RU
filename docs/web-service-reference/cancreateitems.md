---
title: канкреатеитемс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanCreateItems
api_type:
- schema
ms.assetid: c4574e9a-3c42-40a1-a5f9-79b6560e9b30
description: Элемент Канкреатеитемс указывает, имеет ли пользователь разрешение на создание элементов в папке. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 73d3d967774d9fcff53722d0936462025e02b659
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458784"
---
# <a name="cancreateitems"></a><span data-ttu-id="a88fe-104">канкреатеитемс</span><span class="sxs-lookup"><span data-stu-id="a88fe-104">CanCreateItems</span></span>

<span data-ttu-id="a88fe-105">Элемент **канкреатеитемс** указывает, имеет ли пользователь разрешение на создание элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="a88fe-105">The **CanCreateItems** element indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="a88fe-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a88fe-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateItems/>
```

 <span data-ttu-id="a88fe-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a88fe-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a88fe-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a88fe-108">Attributes and elements</span></span>

<span data-ttu-id="a88fe-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a88fe-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a88fe-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a88fe-110">Attributes</span></span>

<span data-ttu-id="a88fe-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a88fe-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a88fe-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a88fe-112">Child elements</span></span>

<span data-ttu-id="a88fe-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a88fe-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a88fe-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a88fe-114">Parent elements</span></span>

|<span data-ttu-id="a88fe-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a88fe-115">**Element**</span></span>|<span data-ttu-id="a88fe-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a88fe-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a88fe-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="a88fe-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="a88fe-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="a88fe-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="a88fe-120">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="a88fe-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="a88fe-p104">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="a88fe-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a88fe-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a88fe-123">Text value</span></span>

<span data-ttu-id="a88fe-124">Текстовое значение **true** указывает на то, что пользователь может создавать элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="a88fe-124">A text value of **true** indicates that the user can create items in the folder.</span></span> <span data-ttu-id="a88fe-125">Значение **false** указывает, что пользователь не может создавать элементы в папке.</span><span class="sxs-lookup"><span data-stu-id="a88fe-125">A value of **false** indicates that the user cannot create items in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a88fe-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="a88fe-126">Remarks</span></span>

<span data-ttu-id="a88fe-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a88fe-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a88fe-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a88fe-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a88fe-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a88fe-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a88fe-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a88fe-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a88fe-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a88fe-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="a88fe-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a88fe-132">Validation File</span></span>  <br/> |<span data-ttu-id="a88fe-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a88fe-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a88fe-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a88fe-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a88fe-135">False</span><span class="sxs-lookup"><span data-stu-id="a88fe-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a88fe-136">См. также</span><span class="sxs-lookup"><span data-stu-id="a88fe-136">See also</span></span>



- [<span data-ttu-id="a88fe-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a88fe-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a88fe-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="a88fe-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

