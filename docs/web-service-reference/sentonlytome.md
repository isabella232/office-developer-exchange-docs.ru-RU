---
title: SentOnlyToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentOnlyToMe
api_type:
- schema
ms.assetid: b6d4dea5-812d-4b29-917d-071ebd7ddd92
description: Элемент SentOnlyToMe указывает, является ли владелец почтового ящика должен быть только один в свойстве ToRecipients входящих сообщений в порядке для условие или исключение для применения.
ms.openlocfilehash: 91c31069652a35dc7a38ad6b6e1512cc07d67a98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835353"
---
# <a name="sentonlytome"></a><span data-ttu-id="7f4eb-103">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="7f4eb-103">SentOnlyToMe</span></span>

<span data-ttu-id="7f4eb-104">Элемент **SentOnlyToMe** указывает, является ли владелец почтового ящика должен быть только один в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="7f4eb-104">The **SentOnlyToMe** element indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentOnlyToMe/>true | false</SentOnlyToMe>
```

 <span data-ttu-id="7f4eb-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7f4eb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f4eb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7f4eb-106">Attributes and elements</span></span>

<span data-ttu-id="7f4eb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7f4eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f4eb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7f4eb-108">Attributes</span></span>

<span data-ttu-id="7f4eb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7f4eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f4eb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7f4eb-110">Child elements</span></span>

<span data-ttu-id="7f4eb-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7f4eb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f4eb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7f4eb-112">Parent elements</span></span>

|<span data-ttu-id="7f4eb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7f4eb-113">**Element**</span></span>|<span data-ttu-id="7f4eb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7f4eb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f4eb-115">Условия</span><span class="sxs-lookup"><span data-stu-id="7f4eb-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="7f4eb-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="7f4eb-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="7f4eb-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="7f4eb-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="7f4eb-118">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="7f4eb-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7f4eb-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7f4eb-119">Text value</span></span>

<span data-ttu-id="7f4eb-120">Текстовое значение **true,** указывает, что владелец почтового ящика должен быть только один в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="7f4eb-120">A text value of **true** indicates that the owner of the mailbox must be the only one in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="7f4eb-121">Значение **false** указывает, что владелец почтового ящика не должна быть только один в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="7f4eb-121">A value of **false** indicates that the owner of the mailbox must not be the only one in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7f4eb-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="7f4eb-122">Remarks</span></span>

<span data-ttu-id="7f4eb-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f4eb-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f4eb-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7f4eb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f4eb-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7f4eb-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7f4eb-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7f4eb-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7f4eb-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7f4eb-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7f4eb-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7f4eb-128">Validation File</span></span>  <br/> |<span data-ttu-id="7f4eb-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7f4eb-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7f4eb-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7f4eb-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f4eb-131">True</span><span class="sxs-lookup"><span data-stu-id="7f4eb-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f4eb-132">См. также</span><span class="sxs-lookup"><span data-stu-id="7f4eb-132">See also</span></span>



- [<span data-ttu-id="7f4eb-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7f4eb-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

