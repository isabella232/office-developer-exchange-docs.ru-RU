---
title: CreateAssociated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAssociated
api_type:
- schema
ms.assetid: 742a6136-6015-4924-bae4-f3868127e966
description: Элемент CreateAssociated указывает ли клиента можно создать таблицу связанного содержимого. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: ec6e55ed2423ff5849f6d19aee29f790572ddda6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761854"
---
# <a name="createassociated"></a><span data-ttu-id="3b3ea-104">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="3b3ea-104">CreateAssociated</span></span>

<span data-ttu-id="3b3ea-105">Элемент **CreateAssociated** указывает ли клиента можно создать таблицу связанного содержимого.</span><span class="sxs-lookup"><span data-stu-id="3b3ea-105">The **CreateAssociated** element indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="3b3ea-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3b3ea-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateAssociated>true or false</CreateAssociated>
```

 <span data-ttu-id="3b3ea-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="3b3ea-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b3ea-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3b3ea-108">Attributes and elements</span></span>

<span data-ttu-id="3b3ea-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3b3ea-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b3ea-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3b3ea-110">Attributes</span></span>

<span data-ttu-id="3b3ea-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b3ea-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b3ea-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3b3ea-112">Child elements</span></span>

<span data-ttu-id="3b3ea-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b3ea-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b3ea-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3b3ea-114">Parent elements</span></span>

|<span data-ttu-id="3b3ea-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3b3ea-115">**Element**</span></span>|<span data-ttu-id="3b3ea-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3b3ea-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b3ea-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="3b3ea-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="3b3ea-118">Содержит правами клиент, построенный на параметры разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="3b3ea-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="3b3ea-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="3b3ea-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3b3ea-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3b3ea-120">Text value</span></span>

<span data-ttu-id="3b3ea-121">Текстовое значение **true,** указывает, что клиент может создать таблицу связанного содержимого.</span><span class="sxs-lookup"><span data-stu-id="3b3ea-121">A text value of **true** indicates that a client can create an associated contents table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3b3ea-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="3b3ea-122">Remarks</span></span>

<span data-ttu-id="3b3ea-123">Это свойство используется только для объектов папки.</span><span class="sxs-lookup"><span data-stu-id="3b3ea-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="3b3ea-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3b3ea-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b3ea-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3b3ea-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b3ea-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3b3ea-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b3ea-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3b3ea-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3b3ea-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3b3ea-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b3ea-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3b3ea-129">Validation File</span></span>  <br/> |<span data-ttu-id="3b3ea-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3b3ea-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b3ea-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3b3ea-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b3ea-132">False</span><span class="sxs-lookup"><span data-stu-id="3b3ea-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b3ea-133">См. также</span><span class="sxs-lookup"><span data-stu-id="3b3ea-133">See also</span></span>



- [<span data-ttu-id="3b3ea-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3b3ea-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="3b3ea-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="3b3ea-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

