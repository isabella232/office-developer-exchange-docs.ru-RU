---
title: IsNotSupported
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotSupported
api_type:
- schema
ms.assetid: 4db469ae-1515-47ea-9905-6aabf199febd
description: Элемент IsNotSupported указывает, не может быть изменения правила с помощью управляемого кода API-интерфейсы.
ms.openlocfilehash: 2468d47dbfdcaf1a28ed1a4afb1e7ea60147d1dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834057"
---
# <a name="isnotsupported"></a><span data-ttu-id="78023-103">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="78023-103">IsNotSupported</span></span>

<span data-ttu-id="78023-104">Элемент **IsNotSupported** указывает, не может быть изменения правила с помощью управляемого кода API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="78023-104">The **IsNotSupported** element indicates whether the rule cannot be modified by using the managed code APIs.</span></span> 
  
```XML
<IsNotSupported/>
```

 <span data-ttu-id="78023-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="78023-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78023-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="78023-106">Attributes and elements</span></span>

<span data-ttu-id="78023-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="78023-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78023-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="78023-108">Attributes</span></span>

<span data-ttu-id="78023-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="78023-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78023-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="78023-110">Child elements</span></span>

<span data-ttu-id="78023-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="78023-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78023-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="78023-112">Parent elements</span></span>

|<span data-ttu-id="78023-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="78023-113">**Element**</span></span>|<span data-ttu-id="78023-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="78023-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78023-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="78023-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="78023-116">Представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="78023-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="78023-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="78023-117">Text value</span></span>

<span data-ttu-id="78023-118">Текстовое значение **true,** указывает, что правило не может изменяться с помощью управляемого кода API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="78023-118">A text value of **true** indicates that the rule cannot be modified by using the managed code APIs.</span></span> <span data-ttu-id="78023-119">Значение **false** указывает, что правило можно изменить с помощью управляемого кода API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="78023-119">A value of **false** indicates that the rule can be modified by using the managed code APIs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="78023-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="78023-120">Remarks</span></span>

<span data-ttu-id="78023-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="78023-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78023-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="78023-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78023-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="78023-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="78023-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="78023-124">Schema Name</span></span>  <br/> |<span data-ttu-id="78023-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="78023-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="78023-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="78023-126">Validation File</span></span>  <br/> |<span data-ttu-id="78023-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="78023-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="78023-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="78023-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="78023-129">True</span><span class="sxs-lookup"><span data-stu-id="78023-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78023-130">См. также</span><span class="sxs-lookup"><span data-stu-id="78023-130">See also</span></span>



- [<span data-ttu-id="78023-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="78023-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

