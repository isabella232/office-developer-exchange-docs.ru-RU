---
title: ErrorMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cec33a6-4b10-4259-8ac3-3f39a642b34c
description: Элемент ErrorMessage представляет причину ошибки проверки.
ms.openlocfilehash: a35dc6af12e71c8437c13024a254000e8f477a15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526195"
---
# <a name="errormessage"></a><span data-ttu-id="682f1-103">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="682f1-103">ErrorMessage</span></span>

<span data-ttu-id="682f1-104">Элемент **ErrorMessage** представляет причину ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="682f1-104">The **ErrorMessage** element represents the reason for the validation error.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="682f1-105">**String**</span><span class="sxs-lookup"><span data-stu-id="682f1-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="682f1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="682f1-106">Attributes and elements</span></span>

<span data-ttu-id="682f1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="682f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="682f1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="682f1-108">Attributes</span></span>

<span data-ttu-id="682f1-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="682f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="682f1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="682f1-110">Child elements</span></span>

<span data-ttu-id="682f1-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="682f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="682f1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="682f1-112">Parent elements</span></span>

|<span data-ttu-id="682f1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="682f1-113">**Element**</span></span>|<span data-ttu-id="682f1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="682f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="682f1-115">Error</span><span class="sxs-lookup"><span data-stu-id="682f1-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="682f1-116">Представляет одну ошибку проверки для определенного значения свойства правила, значения свойства предиката или значения свойства Action.</span><span class="sxs-lookup"><span data-stu-id="682f1-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="682f1-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="682f1-117">Text value</span></span>

<span data-ttu-id="682f1-118">Сообщение об ошибке, связанное с ошибкой проверки правила.</span><span class="sxs-lookup"><span data-stu-id="682f1-118">The error message associated with the rule validation error.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="682f1-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="682f1-119">Remarks</span></span>

<span data-ttu-id="682f1-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="682f1-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="682f1-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="682f1-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="682f1-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="682f1-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="682f1-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="682f1-123">Schema Name</span></span>  <br/> |<span data-ttu-id="682f1-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="682f1-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="682f1-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="682f1-125">Validation File</span></span>  <br/> |<span data-ttu-id="682f1-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="682f1-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="682f1-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="682f1-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="682f1-128">True</span><span class="sxs-lookup"><span data-stu-id="682f1-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="682f1-129">См. также</span><span class="sxs-lookup"><span data-stu-id="682f1-129">See also</span></span>



- [<span data-ttu-id="682f1-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="682f1-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

