---
title: минимумсизе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: Элемент Минимумсизе представляет минимальный размер сообщения, которое должно быть применено к определенному условию или исключению.
ms.openlocfilehash: 4f80bac3b9226019ec3d726cd2d6430e02cac423
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834480"
---
# <a name="minimumsize"></a><span data-ttu-id="116f7-103">минимумсизе</span><span class="sxs-lookup"><span data-stu-id="116f7-103">MinimumSize</span></span>

<span data-ttu-id="116f7-104">Элемент **минимумсизе** представляет минимальный размер сообщения, которое должно быть применено к определенному условию или исключению.</span><span class="sxs-lookup"><span data-stu-id="116f7-104">The **MinimumSize** element represents the minimum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<MinimumSize/>
```

 <span data-ttu-id="116f7-105">**int**</span><span class="sxs-lookup"><span data-stu-id="116f7-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="116f7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="116f7-106">Attributes and elements</span></span>

<span data-ttu-id="116f7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="116f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="116f7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="116f7-108">Attributes</span></span>

<span data-ttu-id="116f7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="116f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="116f7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="116f7-110">Child elements</span></span>

<span data-ttu-id="116f7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="116f7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="116f7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="116f7-112">Parent elements</span></span>

|<span data-ttu-id="116f7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="116f7-113">**Element**</span></span>|<span data-ttu-id="116f7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="116f7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="116f7-115">висинсизеранже</span><span class="sxs-lookup"><span data-stu-id="116f7-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="116f7-116">Указывает минимальный и максимальный размеры для входящих сообщений, для которых необходимо применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="116f7-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="116f7-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="116f7-117">Text value</span></span>

<span data-ttu-id="116f7-118">Текстовое значение — это целое число, определяющее минимальный размер сообщения в байтах.</span><span class="sxs-lookup"><span data-stu-id="116f7-118">The text value is an integer that identifies the minimum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="116f7-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="116f7-119">Remarks</span></span>

<span data-ttu-id="116f7-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="116f7-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="116f7-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="116f7-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="116f7-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="116f7-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="116f7-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="116f7-123">Schema Name</span></span>  <br/> |<span data-ttu-id="116f7-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="116f7-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="116f7-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="116f7-125">Validation File</span></span>  <br/> |<span data-ttu-id="116f7-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="116f7-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="116f7-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="116f7-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="116f7-128">True</span><span class="sxs-lookup"><span data-stu-id="116f7-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="116f7-129">См. также</span><span class="sxs-lookup"><span data-stu-id="116f7-129">See also</span></span>



[<span data-ttu-id="116f7-130">максимумсизе</span><span class="sxs-lookup"><span data-stu-id="116f7-130">MaximumSize</span></span>](maximumsize.md)


- [<span data-ttu-id="116f7-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="116f7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

