---
title: Сообщение об ошибке
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cec33a6-4b10-4259-8ac3-3f39a642b34c
description: Сообщение об ошибке элемент представляет причину ошибки проверки.
ms.openlocfilehash: d1869041254ef7c661fb2acb7c9c2ccaf628b394
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762390"
---
# <a name="errormessage"></a><span data-ttu-id="28808-103">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="28808-103">ErrorMessage</span></span>

<span data-ttu-id="28808-104">**Сообщение об ошибке** элемент представляет причину ошибки проверки.</span><span class="sxs-lookup"><span data-stu-id="28808-104">The **ErrorMessage** element represents the reason for the validation error.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="28808-105">**Строка**</span><span class="sxs-lookup"><span data-stu-id="28808-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28808-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="28808-106">Attributes and elements</span></span>

<span data-ttu-id="28808-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="28808-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28808-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="28808-108">Attributes</span></span>

<span data-ttu-id="28808-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="28808-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28808-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="28808-110">Child elements</span></span>

<span data-ttu-id="28808-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="28808-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="28808-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="28808-112">Parent elements</span></span>

|<span data-ttu-id="28808-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28808-113">**Element**</span></span>|<span data-ttu-id="28808-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28808-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28808-115">Error</span><span class="sxs-lookup"><span data-stu-id="28808-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="28808-116">Представляет ошибку одной проверки на значение свойства определенное правило, значение свойства предиката или значение свойства действия.</span><span class="sxs-lookup"><span data-stu-id="28808-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28808-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="28808-117">Text value</span></span>

<span data-ttu-id="28808-118">Сообщение об ошибке, связанный с ошибкой правила проверки.</span><span class="sxs-lookup"><span data-stu-id="28808-118">The error message associated with the rule validation error.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28808-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="28808-119">Remarks</span></span>

<span data-ttu-id="28808-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="28808-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28808-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="28808-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28808-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="28808-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28808-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="28808-123">Schema Name</span></span>  <br/> |<span data-ttu-id="28808-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="28808-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="28808-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="28808-125">Validation File</span></span>  <br/> |<span data-ttu-id="28808-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="28808-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28808-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="28808-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="28808-128">True</span><span class="sxs-lookup"><span data-stu-id="28808-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28808-129">См. также</span><span class="sxs-lookup"><span data-stu-id="28808-129">See also</span></span>



- [<span data-ttu-id="28808-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="28808-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

