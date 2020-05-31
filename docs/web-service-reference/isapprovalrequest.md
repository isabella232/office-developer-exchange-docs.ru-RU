---
title: исаппровалрекуест
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
description: Элемент Исаппровалрекуест указывает, должны ли входящие сообщения быть запросами на утверждение, чтобы применялось условие или исключение.
ms.openlocfilehash: 45b0836efff3ec9fe644cbaeb7ea7192346422bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833984"
---
# <a name="isapprovalrequest"></a><span data-ttu-id="f40a3-103">исаппровалрекуест</span><span class="sxs-lookup"><span data-stu-id="f40a3-103">IsApprovalRequest</span></span>

<span data-ttu-id="f40a3-104">Элемент **исаппровалрекуест** указывает, должны ли входящие сообщения быть запросами на утверждение, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="f40a3-104">The **IsApprovalRequest** element indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span> 
  
```XML
<IsApprovalRequest/>
```

 <span data-ttu-id="f40a3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f40a3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f40a3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f40a3-106">Attributes and elements</span></span>

<span data-ttu-id="f40a3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f40a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f40a3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f40a3-108">Attributes</span></span>

<span data-ttu-id="f40a3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f40a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f40a3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f40a3-110">Child elements</span></span>

<span data-ttu-id="f40a3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f40a3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f40a3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f40a3-112">Parent elements</span></span>

|<span data-ttu-id="f40a3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f40a3-113">**Element**</span></span>|<span data-ttu-id="f40a3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f40a3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f40a3-115">Условия</span><span class="sxs-lookup"><span data-stu-id="f40a3-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="f40a3-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="f40a3-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="f40a3-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="f40a3-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="f40a3-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="f40a3-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f40a3-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f40a3-119">Text value</span></span>

<span data-ttu-id="f40a3-120">Текстовое значение **true** указывает, что сообщение должно быть запросом утверждения, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="f40a3-120">A text value of **true** indicates that the message must be an approval request in order for the condition or exception to apply.</span></span> <span data-ttu-id="f40a3-121">Значение **false** указывает, что сообщение не должно быть запросом на утверждение, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="f40a3-121">A value of **false** indicates that the message must not be an approval request in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f40a3-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="f40a3-122">Remarks</span></span>

<span data-ttu-id="f40a3-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f40a3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f40a3-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f40a3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f40a3-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f40a3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f40a3-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f40a3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f40a3-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f40a3-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f40a3-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f40a3-128">Validation File</span></span>  <br/> |<span data-ttu-id="f40a3-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f40a3-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f40a3-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f40a3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f40a3-131">True</span><span class="sxs-lookup"><span data-stu-id="f40a3-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f40a3-132">См. также</span><span class="sxs-lookup"><span data-stu-id="f40a3-132">See also</span></span>



- [<span data-ttu-id="f40a3-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f40a3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

