---
title: Чтение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Read
api_type:
- schema
ms.assetid: b14637e9-1695-4b7e-b078-ae527c2e4303
description: Элемент чтения указывает ли клиента могут читать папку или элемент. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: cd9c2c9802c78b202418e3947f5b5718b0f676cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834948"
---
# <a name="read"></a><span data-ttu-id="edbc5-104">Чтение</span><span class="sxs-lookup"><span data-stu-id="edbc5-104">Read</span></span>

<span data-ttu-id="edbc5-105">Элемент **чтения** указывает ли клиента могут читать папку или элемент.</span><span class="sxs-lookup"><span data-stu-id="edbc5-105">The **Read** element indicates whether a client can read a folder or item.</span></span> <span data-ttu-id="edbc5-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="edbc5-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Read>true or false</Read>
```

 <span data-ttu-id="edbc5-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="edbc5-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="edbc5-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="edbc5-108">Attributes and elements</span></span>

<span data-ttu-id="edbc5-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="edbc5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="edbc5-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="edbc5-110">Attributes</span></span>

<span data-ttu-id="edbc5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="edbc5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="edbc5-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="edbc5-112">Child elements</span></span>

<span data-ttu-id="edbc5-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="edbc5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="edbc5-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="edbc5-114">Parent elements</span></span>

|<span data-ttu-id="edbc5-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="edbc5-115">**Element**</span></span>|<span data-ttu-id="edbc5-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="edbc5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edbc5-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="edbc5-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="edbc5-118">Содержит правами клиент, построенный на параметры разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="edbc5-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="edbc5-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="edbc5-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="edbc5-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="edbc5-120">Text value</span></span>

<span data-ttu-id="edbc5-121">Текстовое значение **true,** указывает, что клиент могут читать элемент папки.</span><span class="sxs-lookup"><span data-stu-id="edbc5-121">A text value of **true** indicates that a client can read an item of folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="edbc5-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="edbc5-122">Remarks</span></span>

<span data-ttu-id="edbc5-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="edbc5-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="edbc5-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="edbc5-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="edbc5-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="edbc5-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="edbc5-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="edbc5-126">Schema Name</span></span>  <br/> |<span data-ttu-id="edbc5-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="edbc5-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="edbc5-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="edbc5-128">Validation File</span></span>  <br/> |<span data-ttu-id="edbc5-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="edbc5-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="edbc5-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="edbc5-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="edbc5-131">False</span><span class="sxs-lookup"><span data-stu-id="edbc5-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="edbc5-132">См. также</span><span class="sxs-lookup"><span data-stu-id="edbc5-132">See also</span></span>



- [<span data-ttu-id="edbc5-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="edbc5-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="edbc5-134">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="edbc5-134">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

