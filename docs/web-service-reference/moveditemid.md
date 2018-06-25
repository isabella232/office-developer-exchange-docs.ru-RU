---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: Элемент MovedItemId указывает идентификатор элемента, который был перемещен в MarkAsJunk операции.
ms.openlocfilehash: 17e20e8ca81f97b419fc4a2b413e21322e828ec9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834484"
---
# <a name="moveditemid"></a><span data-ttu-id="b07f7-103">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="b07f7-103">MovedItemId</span></span>

<span data-ttu-id="b07f7-104">Элемент **MovedItemId** указывает идентификатор элемента, который был перемещен в **MarkAsJunk** операции.</span><span class="sxs-lookup"><span data-stu-id="b07f7-104">The **MovedItemId** element specifies the identifier of the item that was moved by the **MarkAsJunk** operation.</span></span> 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="b07f7-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="b07f7-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b07f7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b07f7-106">Attributes and elements</span></span>

<span data-ttu-id="b07f7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b07f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b07f7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b07f7-108">Attributes</span></span>

|<span data-ttu-id="b07f7-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b07f7-109">**Attribute**</span></span>|<span data-ttu-id="b07f7-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b07f7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b07f7-111">Id</span><span class="sxs-lookup"><span data-stu-id="b07f7-111">Id</span></span>  <br/> |<span data-ttu-id="b07f7-112">Значение атрибута **Id** является идентификатор элемента, который перемещается операцией **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="b07f7-112">The value of the **Id** attribute is the item identifier of the item that is moved by the **MarkAsJunk** operation.</span></span> <span data-ttu-id="b07f7-113">Идентификатор элемента не изменится после перемещения.</span><span class="sxs-lookup"><span data-stu-id="b07f7-113">The item identifier will remain the same after the move.</span></span>  <br/> |
|<span data-ttu-id="b07f7-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="b07f7-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="b07f7-115">Значение атрибута **ChangeKey** — ключ изменения перемещаемый элемент.</span><span class="sxs-lookup"><span data-stu-id="b07f7-115">The value of the **ChangeKey** attribute is the change key of the moved item.</span></span> <span data-ttu-id="b07f7-116">Изменения ключевых изменений после перемещено операцией **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="b07f7-116">The change key changes after the item is moved by the **MarkAsJunk** operation.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b07f7-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b07f7-117">Child elements</span></span>

<span data-ttu-id="b07f7-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="b07f7-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b07f7-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b07f7-119">Parent elements</span></span>

[<span data-ttu-id="b07f7-120">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b07f7-120">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="b07f7-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="b07f7-121">Remarks</span></span>

<span data-ttu-id="b07f7-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b07f7-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b07f7-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b07f7-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b07f7-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b07f7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b07f7-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b07f7-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b07f7-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b07f7-126">Schema name</span></span>  <br/> |<span data-ttu-id="b07f7-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b07f7-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b07f7-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b07f7-128">Validation file</span></span>  <br/> |<span data-ttu-id="b07f7-129">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b07f7-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b07f7-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b07f7-130">Can be empty</span></span>  <br/> ||
   

