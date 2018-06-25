---
title: UnknownEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownEntry
api_type:
- schema
ms.assetid: 3cb4c62e-052a-4326-8639-8c41dfd047b2
description: Элемент UnknownEntry представляет элемент одного Неизвестный разрешения, которая не может быть относительно службы каталогов Active Directory. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 11939ad39c83ac2d15ec7fface6f530d3f60e12a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840298"
---
# <a name="unknownentry"></a><span data-ttu-id="f0ad5-104">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="f0ad5-104">UnknownEntry</span></span>

<span data-ttu-id="f0ad5-105">Элемент **UnknownEntry** представляет элемент одного Неизвестный разрешения, которая не может быть относительно службы каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0ad5-105">The **UnknownEntry** element represents a single unknown permission entry that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="f0ad5-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f0ad5-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntry/>
```

 <span data-ttu-id="f0ad5-107">**string**</span><span class="sxs-lookup"><span data-stu-id="f0ad5-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0ad5-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f0ad5-108">Attributes and elements</span></span>

<span data-ttu-id="f0ad5-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f0ad5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0ad5-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f0ad5-110">Attributes</span></span>

<span data-ttu-id="f0ad5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f0ad5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0ad5-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f0ad5-112">Child elements</span></span>

<span data-ttu-id="f0ad5-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="f0ad5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f0ad5-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f0ad5-114">Parent elements</span></span>

|<span data-ttu-id="f0ad5-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f0ad5-115">**Element**</span></span>|<span data-ttu-id="f0ad5-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0ad5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0ad5-117">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="f0ad5-117">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="f0ad5-118">Содержит массив элементов Неизвестный разрешений, которые не удалось разрешить с Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0ad5-118">Contains an array of unknown permission entries that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="f0ad5-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="f0ad5-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f0ad5-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f0ad5-120">Text value</span></span>

<span data-ttu-id="f0ad5-121">Текстовое значение представляет элемент разрешения, который не может быть разрешен с Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0ad5-121">The text value represents a permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="f0ad5-122">Текстовое значение представляет идентификатор безопасности (SID).</span><span class="sxs-lookup"><span data-stu-id="f0ad5-122">The text value represents a security identifier (SID).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f0ad5-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="f0ad5-123">Remarks</span></span>

<span data-ttu-id="f0ad5-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f0ad5-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0ad5-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f0ad5-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0ad5-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f0ad5-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f0ad5-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f0ad5-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f0ad5-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f0ad5-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="f0ad5-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f0ad5-129">Validation File</span></span>  <br/> |<span data-ttu-id="f0ad5-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f0ad5-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f0ad5-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f0ad5-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0ad5-132">False</span><span class="sxs-lookup"><span data-stu-id="f0ad5-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0ad5-133">См. также</span><span class="sxs-lookup"><span data-stu-id="f0ad5-133">See also</span></span>



- [<span data-ttu-id="f0ad5-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f0ad5-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f0ad5-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="f0ad5-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

