---
title: иснотсуппортед
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
description: Элемент Иснотсуппортед указывает, не может ли правило измениться с помощью API управляемого кода.
ms.openlocfilehash: e2d0c506209978fd5e8702e0de6cddf2e9c4b7fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465837"
---
# <a name="isnotsupported"></a><span data-ttu-id="193a2-103">иснотсуппортед</span><span class="sxs-lookup"><span data-stu-id="193a2-103">IsNotSupported</span></span>

<span data-ttu-id="193a2-104">Элемент **иснотсуппортед** указывает, не может ли правило измениться с помощью API управляемого кода.</span><span class="sxs-lookup"><span data-stu-id="193a2-104">The **IsNotSupported** element indicates whether the rule cannot be modified by using the managed code APIs.</span></span> 
  
```XML
<IsNotSupported/>
```

 <span data-ttu-id="193a2-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="193a2-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="193a2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="193a2-106">Attributes and elements</span></span>

<span data-ttu-id="193a2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="193a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="193a2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="193a2-108">Attributes</span></span>

<span data-ttu-id="193a2-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="193a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="193a2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="193a2-110">Child elements</span></span>

<span data-ttu-id="193a2-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="193a2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="193a2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="193a2-112">Parent elements</span></span>

|<span data-ttu-id="193a2-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="193a2-113">**Element**</span></span>|<span data-ttu-id="193a2-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="193a2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="193a2-115">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="193a2-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="193a2-116">Представляет правило в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="193a2-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="193a2-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="193a2-117">Text value</span></span>

<span data-ttu-id="193a2-118">Текстовое значение **true** указывает, что правило невозможно изменить с помощью API управляемого кода.</span><span class="sxs-lookup"><span data-stu-id="193a2-118">A text value of **true** indicates that the rule cannot be modified by using the managed code APIs.</span></span> <span data-ttu-id="193a2-119">Значение **false** указывает, что правило можно изменить с помощью API управляемого кода.</span><span class="sxs-lookup"><span data-stu-id="193a2-119">A value of **false** indicates that the rule can be modified by using the managed code APIs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="193a2-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="193a2-120">Remarks</span></span>

<span data-ttu-id="193a2-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="193a2-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="193a2-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="193a2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="193a2-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="193a2-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="193a2-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="193a2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="193a2-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="193a2-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="193a2-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="193a2-126">Validation File</span></span>  <br/> |<span data-ttu-id="193a2-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="193a2-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="193a2-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="193a2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="193a2-129">True</span><span class="sxs-lookup"><span data-stu-id="193a2-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="193a2-130">См. также</span><span class="sxs-lookup"><span data-stu-id="193a2-130">See also</span></span>



- [<span data-ttu-id="193a2-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="193a2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

