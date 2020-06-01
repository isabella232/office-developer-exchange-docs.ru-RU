---
title: исфолдеровнер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderOwner
api_type:
- schema
ms.assetid: 6541ee78-d6e6-42a7-8e7a-d8736172b245
description: Элемент Исфолдеровнер указывает, является ли пользователь владельцем папки. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 1a06682152b89f4b554b2dd99989a72f6fe49608
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457580"
---
# <a name="isfolderowner"></a><span data-ttu-id="364a0-104">исфолдеровнер</span><span class="sxs-lookup"><span data-stu-id="364a0-104">IsFolderOwner</span></span>

<span data-ttu-id="364a0-105">Элемент **исфолдеровнер** указывает, является ли пользователь владельцем папки.</span><span class="sxs-lookup"><span data-stu-id="364a0-105">The **IsFolderOwner** element indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="364a0-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="364a0-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderOwner/>
```

 <span data-ttu-id="364a0-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="364a0-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="364a0-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="364a0-108">Attributes and elements</span></span>

<span data-ttu-id="364a0-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="364a0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="364a0-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="364a0-110">Attributes</span></span>

<span data-ttu-id="364a0-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="364a0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="364a0-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="364a0-112">Child elements</span></span>

<span data-ttu-id="364a0-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="364a0-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="364a0-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="364a0-114">Parent elements</span></span>

|<span data-ttu-id="364a0-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="364a0-115">**Element**</span></span>|<span data-ttu-id="364a0-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="364a0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="364a0-117">Разрешение</span><span class="sxs-lookup"><span data-stu-id="364a0-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="364a0-p103">Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="364a0-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="364a0-120">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="364a0-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="364a0-p104">Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="364a0-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="364a0-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="364a0-123">Text value</span></span>

<span data-ttu-id="364a0-124">Текстовое значение **true** указывает, что пользователь является владельцем папки.</span><span class="sxs-lookup"><span data-stu-id="364a0-124">A text value of **true** indicates that the user is the owner of the folder.</span></span> <span data-ttu-id="364a0-125">Значение **false** указывает, что пользователь не является владельцем папки.</span><span class="sxs-lookup"><span data-stu-id="364a0-125">A value of **false** indicates that the user is not the owner of the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="364a0-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="364a0-126">Remarks</span></span>

<span data-ttu-id="364a0-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="364a0-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="364a0-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="364a0-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="364a0-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="364a0-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="364a0-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="364a0-130">Schema Name</span></span>  <br/> |<span data-ttu-id="364a0-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="364a0-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="364a0-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="364a0-132">Validation File</span></span>  <br/> |<span data-ttu-id="364a0-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="364a0-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="364a0-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="364a0-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="364a0-135">False</span><span class="sxs-lookup"><span data-stu-id="364a0-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="364a0-136">См. также</span><span class="sxs-lookup"><span data-stu-id="364a0-136">See also</span></span>



- [<span data-ttu-id="364a0-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="364a0-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="364a0-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="364a0-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

