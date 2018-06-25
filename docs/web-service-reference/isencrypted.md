---
title: IsEncrypted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEncrypted
api_type:
- schema
ms.assetid: 68a30e92-c2b1-4af5-bb16-ba38afb80c43
description: Элемент IsEncrypted указывает, должен ли входящих сообщений S/MIME шифруются в порядке для условие или исключение для применения.
ms.openlocfilehash: 582a1f197d4ee6b60af91b1a178d79163b50052c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834003"
---
# <a name="isencrypted"></a><span data-ttu-id="5466f-103">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="5466f-103">IsEncrypted</span></span>

<span data-ttu-id="5466f-104">Элемент **IsEncrypted** указывает, должен ли входящих сообщений S/MIME шифруются в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="5466f-104">The **IsEncrypted** element indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span> 
  
```XML
<IsEncrypted>true | false</IsEncrypted>
```

 <span data-ttu-id="5466f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5466f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5466f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5466f-106">Attributes and elements</span></span>

<span data-ttu-id="5466f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5466f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5466f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5466f-108">Attributes</span></span>

<span data-ttu-id="5466f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5466f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5466f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5466f-110">Child elements</span></span>

<span data-ttu-id="5466f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5466f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5466f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5466f-112">Parent elements</span></span>

|<span data-ttu-id="5466f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5466f-113">**Element**</span></span>|<span data-ttu-id="5466f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5466f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5466f-115">Условия</span><span class="sxs-lookup"><span data-stu-id="5466f-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="5466f-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="5466f-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="5466f-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="5466f-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="5466f-118">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="5466f-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5466f-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5466f-119">Text value</span></span>

<span data-ttu-id="5466f-120">Текстовое значение **true,** указывает, что сообщение должен быть зашифрован в порядке для условие или исключение для применения S/MIME.</span><span class="sxs-lookup"><span data-stu-id="5466f-120">A text value of **true** indicates that the message must be S/MIME encrypted in order for the condition or exception to apply.</span></span> <span data-ttu-id="5466f-121">Значение **false** указывает, что сообщение не обязательно S/MIME для условие или исключение того, чтобы применить.</span><span class="sxs-lookup"><span data-stu-id="5466f-121">A value of **false** indicates that the message does not have to be S/MIME in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5466f-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="5466f-122">Remarks</span></span>

<span data-ttu-id="5466f-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5466f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5466f-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5466f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5466f-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5466f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5466f-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5466f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="5466f-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5466f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5466f-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5466f-128">Validation File</span></span>  <br/> |<span data-ttu-id="5466f-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5466f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5466f-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5466f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="5466f-131">True</span><span class="sxs-lookup"><span data-stu-id="5466f-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5466f-132">См. также</span><span class="sxs-lookup"><span data-stu-id="5466f-132">See also</span></span>



- [<span data-ttu-id="5466f-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5466f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

