---
title: MaximumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fb7c3ab3-ef97-44c7-83e0-93cfe8c48e84
description: Элемент максимальный_размер представляет максимальный размер, который должен быть сообщение в порядке для условие или исключение для применения.
ms.openlocfilehash: 37e3d377b105534fe34b54e262bd47bc450706da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834387"
---
# <a name="maximumsize"></a><span data-ttu-id="6e2fa-103">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="6e2fa-103">MaximumSize</span></span>

<span data-ttu-id="6e2fa-104">Элемент **максимальный_размер** представляет максимальный размер, который должен быть сообщение в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="6e2fa-104">The **MaximumSize** element represents the maximum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<Maximum/>
```

 <span data-ttu-id="6e2fa-105">**int**</span><span class="sxs-lookup"><span data-stu-id="6e2fa-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e2fa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6e2fa-106">Attributes and elements</span></span>

<span data-ttu-id="6e2fa-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6e2fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e2fa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6e2fa-108">Attributes</span></span>

<span data-ttu-id="6e2fa-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6e2fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e2fa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6e2fa-110">Child elements</span></span>

<span data-ttu-id="6e2fa-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6e2fa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e2fa-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6e2fa-112">Parent elements</span></span>

|<span data-ttu-id="6e2fa-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6e2fa-113">**Element**</span></span>|<span data-ttu-id="6e2fa-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6e2fa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e2fa-115">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="6e2fa-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="6e2fa-116">Указывает минимальный и максимальный размеры, которые должны быть входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="6e2fa-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e2fa-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6e2fa-117">Text value</span></span>

<span data-ttu-id="6e2fa-118">Текстовое значение представляет собой целое число, указывающее максимальный размер сообщения в байтах.</span><span class="sxs-lookup"><span data-stu-id="6e2fa-118">The text value is an integer that identifies the maximum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e2fa-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="6e2fa-119">Remarks</span></span>

<span data-ttu-id="6e2fa-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e2fa-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e2fa-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6e2fa-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e2fa-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6e2fa-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6e2fa-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6e2fa-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6e2fa-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6e2fa-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6e2fa-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6e2fa-125">Validation File</span></span>  <br/> |<span data-ttu-id="6e2fa-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6e2fa-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e2fa-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6e2fa-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e2fa-128">True</span><span class="sxs-lookup"><span data-stu-id="6e2fa-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e2fa-129">См. также</span><span class="sxs-lookup"><span data-stu-id="6e2fa-129">See also</span></span>



[<span data-ttu-id="6e2fa-130">Минимальный размер</span><span class="sxs-lookup"><span data-stu-id="6e2fa-130">MinimumSize</span></span>](minimumsize.md)


- [<span data-ttu-id="6e2fa-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6e2fa-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

