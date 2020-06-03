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
ms.openlocfilehash: 08ea36820b2680bb2c7e5695eb2dd481154c05eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530022"
---
# <a name="isapprovalrequest"></a><span data-ttu-id="69259-103">исаппровалрекуест</span><span class="sxs-lookup"><span data-stu-id="69259-103">IsApprovalRequest</span></span>

<span data-ttu-id="69259-104">Элемент **исаппровалрекуест** указывает, должны ли входящие сообщения быть запросами на утверждение, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="69259-104">The **IsApprovalRequest** element indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span> 
  
```XML
<IsApprovalRequest/>
```

 <span data-ttu-id="69259-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="69259-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69259-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="69259-106">Attributes and elements</span></span>

<span data-ttu-id="69259-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="69259-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69259-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="69259-108">Attributes</span></span>

<span data-ttu-id="69259-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="69259-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69259-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="69259-110">Child elements</span></span>

<span data-ttu-id="69259-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="69259-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="69259-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="69259-112">Parent elements</span></span>

|<span data-ttu-id="69259-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69259-113">**Element**</span></span>|<span data-ttu-id="69259-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69259-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69259-115">Условия</span><span class="sxs-lookup"><span data-stu-id="69259-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="69259-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="69259-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="69259-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="69259-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="69259-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="69259-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="69259-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="69259-119">Text value</span></span>

<span data-ttu-id="69259-120">Текстовое значение **true** указывает, что сообщение должно быть запросом утверждения, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="69259-120">A text value of **true** indicates that the message must be an approval request in order for the condition or exception to apply.</span></span> <span data-ttu-id="69259-121">Значение **false** указывает, что сообщение не должно быть запросом на утверждение, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="69259-121">A value of **false** indicates that the message must not be an approval request in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="69259-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="69259-122">Remarks</span></span>

<span data-ttu-id="69259-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="69259-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69259-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="69259-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69259-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="69259-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="69259-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="69259-126">Schema Name</span></span>  <br/> |<span data-ttu-id="69259-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="69259-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="69259-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="69259-128">Validation File</span></span>  <br/> |<span data-ttu-id="69259-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="69259-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="69259-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="69259-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="69259-131">True</span><span class="sxs-lookup"><span data-stu-id="69259-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69259-132">См. также</span><span class="sxs-lookup"><span data-stu-id="69259-132">See also</span></span>



- [<span data-ttu-id="69259-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="69259-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

