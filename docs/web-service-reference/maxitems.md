---
title: MaxItems
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4ddba6b8-0f38-42cd-96a1-0d4283f6375b
description: Элемент MaxItems указывает максимальное число элементов, возвращаемых в запросе.
ms.openlocfilehash: dffb9ba4e29915a65fe2a57b6e7a7b4468028fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834384"
---
# <a name="maxitems"></a><span data-ttu-id="31b2a-103">MaxItems</span><span class="sxs-lookup"><span data-stu-id="31b2a-103">MaxItems</span></span>

<span data-ttu-id="31b2a-104">Элемент **MaxItems** указывает максимальное число элементов, возвращаемых в запросе.</span><span class="sxs-lookup"><span data-stu-id="31b2a-104">The **MaxItems** element specifies the maximum number of items to return in the request.</span></span> 
  
```XML
<MaxItems/>
```

 <span data-ttu-id="31b2a-105">**int**</span><span class="sxs-lookup"><span data-stu-id="31b2a-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31b2a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="31b2a-106">Attributes and elements</span></span>

<span data-ttu-id="31b2a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="31b2a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31b2a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="31b2a-108">Attributes</span></span>

<span data-ttu-id="31b2a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="31b2a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31b2a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="31b2a-110">Child elements</span></span>

<span data-ttu-id="31b2a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="31b2a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="31b2a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="31b2a-112">Parent elements</span></span>

[<span data-ttu-id="31b2a-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="31b2a-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="31b2a-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="31b2a-114">Text value</span></span>

<span data-ttu-id="31b2a-115">Текстовое значение элемента **MaxItems** — это максимальное число элементов, возвращаемых в запросе.</span><span class="sxs-lookup"><span data-stu-id="31b2a-115">The text value of the **MaxItems** element is the maximum number of items to return in the request.</span></span> <span data-ttu-id="31b2a-116">Это число не может быть меньше нуля или больше, чем 200.</span><span class="sxs-lookup"><span data-stu-id="31b2a-116">This number cannot be less than zero or greater than 200.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="31b2a-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="31b2a-117">Remarks</span></span>

<span data-ttu-id="31b2a-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="31b2a-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="31b2a-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="31b2a-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31b2a-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="31b2a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31b2a-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="31b2a-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="31b2a-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="31b2a-122">Schema Name</span></span>  <br/> |<span data-ttu-id="31b2a-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="31b2a-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="31b2a-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="31b2a-124">Validation File</span></span>  <br/> |<span data-ttu-id="31b2a-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="31b2a-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="31b2a-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="31b2a-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="31b2a-127">False</span><span class="sxs-lookup"><span data-stu-id="31b2a-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31b2a-128">См. также</span><span class="sxs-lookup"><span data-stu-id="31b2a-128">See also</span></span>



[<span data-ttu-id="31b2a-129">GetReminders</span><span class="sxs-lookup"><span data-stu-id="31b2a-129">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="31b2a-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="31b2a-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

