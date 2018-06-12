---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: Элемент ReturnNewItemIds указывает, возвращаются ли идентификаторы элементов новых элементов в ответе.
ms.openlocfilehash: 6d3bc83c05a82d6e448041167676f41c2620dcd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835232"
---
# <a name="returnnewitemids"></a><span data-ttu-id="3b97f-103">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="3b97f-103">ReturnNewItemIds</span></span>

<span data-ttu-id="3b97f-104">Элемент **ReturnNewItemIds** указывает, возвращаются ли идентификаторы элементов новых элементов в ответе.</span><span class="sxs-lookup"><span data-stu-id="3b97f-104">The **ReturnNewItemIds** element indicates whether the item identifiers of new items are returned in the response.</span></span> 
  
```XML
<ReturnNewItemIds/>
```

 <span data-ttu-id="3b97f-105">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="3b97f-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b97f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3b97f-106">Attributes and elements</span></span>

<span data-ttu-id="3b97f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3b97f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b97f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3b97f-108">Attributes</span></span>

<span data-ttu-id="3b97f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b97f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b97f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3b97f-110">Child elements</span></span>

<span data-ttu-id="3b97f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b97f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b97f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3b97f-112">Parent elements</span></span>

|<span data-ttu-id="3b97f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3b97f-113">**Element**</span></span>|<span data-ttu-id="3b97f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3b97f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b97f-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="3b97f-115">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="3b97f-116">Определяет запрос для копирования элемента в почтовом ящике в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b97f-116">Defines a request to copy an item in a mailbox in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3b97f-117">MoveItem</span><span class="sxs-lookup"><span data-stu-id="3b97f-117">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="3b97f-118">Определяет запрос на перемещение элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b97f-118">Defines a request to move an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3b97f-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3b97f-119">Text value</span></span>

<span data-ttu-id="3b97f-120">Текстовое значение **true** для элемента **ReturnNewItemIds** указывает, что новые идентификаторы элементов возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="3b97f-120">A text value of **true** for the **ReturnNewItemIds** element indicates that the new item identifiers are returned in the response.</span></span> <span data-ttu-id="3b97f-121">Значение **false** указывает, что новые идентификаторы элементов не возвращаются в ответе.</span><span class="sxs-lookup"><span data-stu-id="3b97f-121">A value of **false** indicates that the new item identifiers are not returned in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3b97f-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="3b97f-122">Remarks</span></span>

<span data-ttu-id="3b97f-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3b97f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b97f-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3b97f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b97f-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3b97f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3b97f-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3b97f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3b97f-127">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="3b97f-127">Message schema</span></span>  <br/> |
|<span data-ttu-id="3b97f-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3b97f-128">Validation File</span></span>  <br/> |<span data-ttu-id="3b97f-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3b97f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3b97f-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3b97f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b97f-131">False</span><span class="sxs-lookup"><span data-stu-id="3b97f-131">False</span></span>  <br/> |
   

