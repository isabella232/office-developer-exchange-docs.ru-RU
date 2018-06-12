---
title: CreateHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateHierarchy
api_type:
- schema
ms.assetid: 630b5610-1c19-4d4a-a5df-8cebb9afd2f4
description: Элемент CreateHierarchy указывает ли клиента можно создать таблицу иерархии. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: a5b428fe453dbc31761309b017367a7d25a01b76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761881"
---
# <a name="createhierarchy"></a><span data-ttu-id="4a82b-104">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="4a82b-104">CreateHierarchy</span></span>

<span data-ttu-id="4a82b-105">Элемент **CreateHierarchy** указывает ли клиента можно создать таблицу иерархии.</span><span class="sxs-lookup"><span data-stu-id="4a82b-105">The **CreateHierarchy** element indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="4a82b-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4a82b-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateHierarchy>true or false</CreateHierarchy>
```

 <span data-ttu-id="4a82b-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="4a82b-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a82b-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4a82b-108">Attributes and elements</span></span>

<span data-ttu-id="4a82b-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4a82b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a82b-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4a82b-110">Attributes</span></span>

<span data-ttu-id="4a82b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="4a82b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a82b-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4a82b-112">Child elements</span></span>

<span data-ttu-id="4a82b-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="4a82b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a82b-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4a82b-114">Parent elements</span></span>

|<span data-ttu-id="4a82b-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4a82b-115">**Element**</span></span>|<span data-ttu-id="4a82b-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4a82b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a82b-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="4a82b-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="4a82b-118">Содержит правами клиент, построенный на параметры разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="4a82b-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="4a82b-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="4a82b-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a82b-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4a82b-120">Text value</span></span>

<span data-ttu-id="4a82b-121">Текстовое значение **true,** указывает, что клиент может создать таблицу иерархии.</span><span class="sxs-lookup"><span data-stu-id="4a82b-121">A text value of **true** indicates that a client can create a hierarchy table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4a82b-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="4a82b-122">Remarks</span></span>

<span data-ttu-id="4a82b-123">Это свойство используется только для объектов папки.</span><span class="sxs-lookup"><span data-stu-id="4a82b-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="4a82b-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4a82b-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a82b-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4a82b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a82b-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4a82b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a82b-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4a82b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4a82b-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4a82b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a82b-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4a82b-129">Validation File</span></span>  <br/> |<span data-ttu-id="4a82b-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4a82b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a82b-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4a82b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a82b-132">False</span><span class="sxs-lookup"><span data-stu-id="4a82b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a82b-133">См. также</span><span class="sxs-lookup"><span data-stu-id="4a82b-133">See also</span></span>



- [<span data-ttu-id="4a82b-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4a82b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="4a82b-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="4a82b-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

