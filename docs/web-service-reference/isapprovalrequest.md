---
title: IsApprovalRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsApprovalRequest
api_type:
- schema
ms.assetid: 293ed01b-f6a4-4459-819c-933bbfaa2dd7
description: Элемент IsApprovalRequest указывает, должен ли входящих сообщений запросов на утверждение в порядке для условие или исключение для применения.
ms.openlocfilehash: 45b0836efff3ec9fe644cbaeb7ea7192346422bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833984"
---
# <a name="isapprovalrequest"></a><span data-ttu-id="14996-103">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="14996-103">IsApprovalRequest</span></span>

<span data-ttu-id="14996-104">Элемент **IsApprovalRequest** указывает, должен ли входящих сообщений запросов на утверждение в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="14996-104">The **IsApprovalRequest** element indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span> 
  
```XML
<IsApprovalRequest/>
```

 <span data-ttu-id="14996-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="14996-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14996-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="14996-106">Attributes and elements</span></span>

<span data-ttu-id="14996-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="14996-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14996-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="14996-108">Attributes</span></span>

<span data-ttu-id="14996-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="14996-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14996-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="14996-110">Child elements</span></span>

<span data-ttu-id="14996-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="14996-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="14996-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="14996-112">Parent elements</span></span>

|<span data-ttu-id="14996-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="14996-113">**Element**</span></span>|<span data-ttu-id="14996-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="14996-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14996-115">Условия</span><span class="sxs-lookup"><span data-stu-id="14996-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="14996-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="14996-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="14996-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="14996-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="14996-118">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="14996-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="14996-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="14996-119">Text value</span></span>

<span data-ttu-id="14996-120">Текстовое значение **true,** указывает, что сообщения должны быть об утверждении, чтобы условие или исключение можно применить.</span><span class="sxs-lookup"><span data-stu-id="14996-120">A text value of **true** indicates that the message must be an approval request in order for the condition or exception to apply.</span></span> <span data-ttu-id="14996-121">Значение **false** указывает, что сообщение не должна быть об утверждении, чтобы условие или исключение можно применить.</span><span class="sxs-lookup"><span data-stu-id="14996-121">A value of **false** indicates that the message must not be an approval request in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="14996-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="14996-122">Remarks</span></span>

<span data-ttu-id="14996-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="14996-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14996-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="14996-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14996-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="14996-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="14996-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="14996-126">Schema Name</span></span>  <br/> |<span data-ttu-id="14996-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="14996-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="14996-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="14996-128">Validation File</span></span>  <br/> |<span data-ttu-id="14996-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="14996-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="14996-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="14996-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="14996-131">True</span><span class="sxs-lookup"><span data-stu-id="14996-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14996-132">См. также</span><span class="sxs-lookup"><span data-stu-id="14996-132">See also</span></span>



- [<span data-ttu-id="14996-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="14996-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

