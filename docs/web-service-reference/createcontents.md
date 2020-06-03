---
title: креатеконтентс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateContents
api_type:
- schema
ms.assetid: 8a9cd241-0d73-4be8-a563-a945898d1a0e
description: Элемент Креатеконтентс указывает, может ли клиент создать таблицу содержимого. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 409e0e566c5fa39830707c199f8e3783411c7334
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458917"
---
# <a name="createcontents"></a><span data-ttu-id="08d94-104">креатеконтентс</span><span class="sxs-lookup"><span data-stu-id="08d94-104">CreateContents</span></span>

<span data-ttu-id="08d94-105">Элемент **креатеконтентс** указывает, может ли клиент создать таблицу содержимого.</span><span class="sxs-lookup"><span data-stu-id="08d94-105">The **CreateContents** element indicates whether a client can create a contents table.</span></span> <span data-ttu-id="08d94-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="08d94-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateContents>true or false</CreateContents>
```

 <span data-ttu-id="08d94-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="08d94-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08d94-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="08d94-108">Attributes and elements</span></span>

<span data-ttu-id="08d94-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="08d94-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08d94-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="08d94-110">Attributes</span></span>

<span data-ttu-id="08d94-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="08d94-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08d94-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="08d94-112">Child elements</span></span>

<span data-ttu-id="08d94-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="08d94-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08d94-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="08d94-114">Parent elements</span></span>

|<span data-ttu-id="08d94-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08d94-115">**Element**</span></span>|<span data-ttu-id="08d94-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08d94-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08d94-117">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="08d94-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="08d94-118">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="08d94-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="08d94-119">Этот элемент был введен в Exchange 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="08d94-119">This element was introduced inExchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="08d94-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="08d94-120">Text value</span></span>

<span data-ttu-id="08d94-121">Текстовое значение **true** указывает, что клиент может создать таблицу содержимого.</span><span class="sxs-lookup"><span data-stu-id="08d94-121">A text value of **true** indicates that a client can create a contents table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="08d94-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="08d94-122">Remarks</span></span>

<span data-ttu-id="08d94-123">Это свойство используется только для объектов Folder.</span><span class="sxs-lookup"><span data-stu-id="08d94-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="08d94-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="08d94-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08d94-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="08d94-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08d94-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="08d94-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08d94-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="08d94-127">Schema Name</span></span>  <br/> |<span data-ttu-id="08d94-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="08d94-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="08d94-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="08d94-129">Validation File</span></span>  <br/> |<span data-ttu-id="08d94-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="08d94-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08d94-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="08d94-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="08d94-132">False</span><span class="sxs-lookup"><span data-stu-id="08d94-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08d94-133">См. также</span><span class="sxs-lookup"><span data-stu-id="08d94-133">See also</span></span>



- [<span data-ttu-id="08d94-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="08d94-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="08d94-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="08d94-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

