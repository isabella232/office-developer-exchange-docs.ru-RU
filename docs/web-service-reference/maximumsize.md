---
title: максимумсизе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fb7c3ab3-ef97-44c7-83e0-93cfe8c48e84
description: Элемент Максимумсизе представляет максимальный размер сообщения, которое должно быть применено к определенному условию или исключению.
ms.openlocfilehash: 250e0c6aed37b934f5cf6eaed9d93b9f56159d93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461753"
---
# <a name="maximumsize"></a><span data-ttu-id="4874b-103">максимумсизе</span><span class="sxs-lookup"><span data-stu-id="4874b-103">MaximumSize</span></span>

<span data-ttu-id="4874b-104">Элемент **максимумсизе** представляет максимальный размер сообщения, которое должно быть применено к определенному условию или исключению.</span><span class="sxs-lookup"><span data-stu-id="4874b-104">The **MaximumSize** element represents the maximum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<Maximum/>
```

 <span data-ttu-id="4874b-105">**int**</span><span class="sxs-lookup"><span data-stu-id="4874b-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4874b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4874b-106">Attributes and elements</span></span>

<span data-ttu-id="4874b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4874b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4874b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4874b-108">Attributes</span></span>

<span data-ttu-id="4874b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4874b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4874b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4874b-110">Child elements</span></span>

<span data-ttu-id="4874b-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4874b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4874b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4874b-112">Parent elements</span></span>

|<span data-ttu-id="4874b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4874b-113">**Element**</span></span>|<span data-ttu-id="4874b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4874b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4874b-115">висинсизеранже</span><span class="sxs-lookup"><span data-stu-id="4874b-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="4874b-116">Указывает минимальный и максимальный размеры для входящих сообщений, для которых необходимо применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="4874b-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4874b-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4874b-117">Text value</span></span>

<span data-ttu-id="4874b-118">Текстовое значение — это целое число, определяющее максимальный размер сообщения в байтах.</span><span class="sxs-lookup"><span data-stu-id="4874b-118">The text value is an integer that identifies the maximum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4874b-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="4874b-119">Remarks</span></span>

<span data-ttu-id="4874b-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4874b-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4874b-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4874b-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4874b-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4874b-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4874b-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4874b-123">Schema Name</span></span>  <br/> |<span data-ttu-id="4874b-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4874b-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4874b-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4874b-125">Validation File</span></span>  <br/> |<span data-ttu-id="4874b-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4874b-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4874b-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4874b-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="4874b-128">True</span><span class="sxs-lookup"><span data-stu-id="4874b-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4874b-129">См. также</span><span class="sxs-lookup"><span data-stu-id="4874b-129">See also</span></span>



[<span data-ttu-id="4874b-130">минимумсизе</span><span class="sxs-lookup"><span data-stu-id="4874b-130">MinimumSize</span></span>](minimumsize.md)


- [<span data-ttu-id="4874b-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4874b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

