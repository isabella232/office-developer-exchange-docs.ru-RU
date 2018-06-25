---
title: SentToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentToMe
api_type:
- schema
ms.assetid: f18aecd1-ad33-41c3-b275-4ca648ce1da0
description: Элемент SentToMe указывает, имеет ли владельца почтового ящика в свойство ToRecipients входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 7f4d24e985256b68d2c5f124f4130f03f35f26e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835365"
---
# <a name="senttome"></a><span data-ttu-id="40d0a-103">SentToMe</span><span class="sxs-lookup"><span data-stu-id="40d0a-103">SentToMe</span></span>

<span data-ttu-id="40d0a-104">Элемент **SentToMe** указывает, имеет ли владельца почтового ящика в свойство **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="40d0a-104">The **SentToMe** element indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToMe>true | false</SentToMe>
```

 <span data-ttu-id="40d0a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="40d0a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40d0a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="40d0a-106">Attributes and elements</span></span>

<span data-ttu-id="40d0a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="40d0a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40d0a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="40d0a-108">Attributes</span></span>

<span data-ttu-id="40d0a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="40d0a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40d0a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="40d0a-110">Child elements</span></span>

<span data-ttu-id="40d0a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="40d0a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="40d0a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="40d0a-112">Parent elements</span></span>

|<span data-ttu-id="40d0a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="40d0a-113">**Element**</span></span>|<span data-ttu-id="40d0a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="40d0a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40d0a-115">Условия</span><span class="sxs-lookup"><span data-stu-id="40d0a-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="40d0a-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="40d0a-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="40d0a-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="40d0a-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="40d0a-118">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="40d0a-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="40d0a-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="40d0a-119">Text value</span></span>

<span data-ttu-id="40d0a-120">Текстовое значение **true,** указывает, что владелец почтового ящика должны быть в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="40d0a-120">A text value of **true** indicates that the owner of the mailbox must be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="40d0a-121">Значение **false** указывает, что владелец почтового ящика не должна быть в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="40d0a-121">A value of **false** indicates that the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="40d0a-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="40d0a-122">Remarks</span></span>

<span data-ttu-id="40d0a-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d0a-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40d0a-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="40d0a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40d0a-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="40d0a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="40d0a-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="40d0a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="40d0a-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="40d0a-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="40d0a-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="40d0a-128">Validation File</span></span>  <br/> |<span data-ttu-id="40d0a-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="40d0a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="40d0a-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="40d0a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="40d0a-131">True</span><span class="sxs-lookup"><span data-stu-id="40d0a-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40d0a-132">См. также</span><span class="sxs-lookup"><span data-stu-id="40d0a-132">See also</span></span>



- [<span data-ttu-id="40d0a-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="40d0a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

