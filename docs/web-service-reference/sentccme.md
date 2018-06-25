---
title: SentCcMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentCcMe
api_type:
- schema
ms.assetid: bf5044e4-cbdf-4e24-a16f-b6454a51fcd5
description: Элемент SentCcMe указывает, имеет ли владельца почтового ящика в свойство CcRecipients входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 634a83d477efbe8683255c4fab71e3f7f1ab2191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835354"
---
# <a name="sentccme"></a><span data-ttu-id="b3429-103">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="b3429-103">SentCcMe</span></span>

<span data-ttu-id="b3429-104">Элемент **SentCcMe** указывает, имеет ли владельца почтового ящика в свойство **CcRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="b3429-104">The **SentCcMe** element indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentCcMe>true | false</SentCcMe>
```

 <span data-ttu-id="b3429-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b3429-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3429-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b3429-106">Attributes and elements</span></span>

<span data-ttu-id="b3429-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b3429-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3429-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b3429-108">Attributes</span></span>

<span data-ttu-id="b3429-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b3429-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3429-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b3429-110">Child elements</span></span>

<span data-ttu-id="b3429-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b3429-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b3429-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b3429-112">Parent elements</span></span>

|<span data-ttu-id="b3429-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b3429-113">**Element**</span></span>|<span data-ttu-id="b3429-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b3429-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3429-115">Условия</span><span class="sxs-lookup"><span data-stu-id="b3429-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="b3429-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="b3429-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="b3429-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="b3429-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="b3429-118">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="b3429-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b3429-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b3429-119">Text value</span></span>

<span data-ttu-id="b3429-120">Текстовое значение **true,** указывает, что владелец почтового ящика должны быть в свойстве **CcRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="b3429-120">A text value of **true** indicates that the owner of the mailbox must be in the **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="b3429-121">Значение **false** указывает, что владелец почтового ящика не должна быть в свойстве **CcRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="b3429-121">A value of **false** indicates that the owner of the mailbox must not be in the **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b3429-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="b3429-122">Remarks</span></span>

<span data-ttu-id="b3429-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3429-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3429-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b3429-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3429-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b3429-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b3429-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b3429-126">Schema Name</span></span>  <br/> |<span data-ttu-id="b3429-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b3429-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b3429-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b3429-128">Validation File</span></span>  <br/> |<span data-ttu-id="b3429-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b3429-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b3429-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b3429-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="b3429-131">True</span><span class="sxs-lookup"><span data-stu-id="b3429-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3429-132">См. также</span><span class="sxs-lookup"><span data-stu-id="b3429-132">See also</span></span>



- [<span data-ttu-id="b3429-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b3429-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

