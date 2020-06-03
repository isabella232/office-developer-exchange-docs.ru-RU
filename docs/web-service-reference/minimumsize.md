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
ms.openlocfilehash: b43a8b5916747c4e3e4ca9b66cf8b9d73f5f8942
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464205"
---
# <a name="minimumsize"></a><span data-ttu-id="bc623-103">минимумсизе</span><span class="sxs-lookup"><span data-stu-id="bc623-103">MinimumSize</span></span>

<span data-ttu-id="bc623-104">Элемент **минимумсизе** представляет минимальный размер сообщения, которое должно быть применено к определенному условию или исключению.</span><span class="sxs-lookup"><span data-stu-id="bc623-104">The **MinimumSize** element represents the minimum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<MinimumSize/>
```

 <span data-ttu-id="bc623-105">**int**</span><span class="sxs-lookup"><span data-stu-id="bc623-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc623-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc623-106">Attributes and elements</span></span>

<span data-ttu-id="bc623-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bc623-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc623-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc623-108">Attributes</span></span>

<span data-ttu-id="bc623-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc623-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc623-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc623-110">Child elements</span></span>

<span data-ttu-id="bc623-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc623-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc623-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc623-112">Parent elements</span></span>

|<span data-ttu-id="bc623-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc623-113">**Element**</span></span>|<span data-ttu-id="bc623-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc623-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc623-115">висинсизеранже</span><span class="sxs-lookup"><span data-stu-id="bc623-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="bc623-116">Указывает минимальный и максимальный размеры для входящих сообщений, для которых необходимо применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="bc623-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc623-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bc623-117">Text value</span></span>

<span data-ttu-id="bc623-118">Текстовое значение — это целое число, определяющее минимальный размер сообщения в байтах.</span><span class="sxs-lookup"><span data-stu-id="bc623-118">The text value is an integer that identifies the minimum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bc623-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="bc623-119">Remarks</span></span>

<span data-ttu-id="bc623-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc623-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc623-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc623-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc623-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc623-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc623-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc623-123">Schema Name</span></span>  <br/> |<span data-ttu-id="bc623-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bc623-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc623-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc623-125">Validation File</span></span>  <br/> |<span data-ttu-id="bc623-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bc623-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc623-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc623-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc623-128">True</span><span class="sxs-lookup"><span data-stu-id="bc623-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc623-129">См. также</span><span class="sxs-lookup"><span data-stu-id="bc623-129">See also</span></span>



[<span data-ttu-id="bc623-130">максимумсизе</span><span class="sxs-lookup"><span data-stu-id="bc623-130">MaximumSize</span></span>](maximumsize.md)


- [<span data-ttu-id="bc623-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc623-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

