---
title: нотсенттоме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotSentToMe
api_type:
- schema
ms.assetid: 7cb63269-622c-4198-9a21-f5a021bf6901
description: Элемент Нотсенттоме указывает, должно ли владелец почтового ящика отсутствовать в свойстве ToRecipients входящих сообщений, чтобы применить условие или исключение.
ms.openlocfilehash: 58efe4381fe0c9f5bd0645a9eba471a13b5e4064
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462614"
---
# <a name="notsenttome"></a><span data-ttu-id="f6d6c-103">нотсенттоме</span><span class="sxs-lookup"><span data-stu-id="f6d6c-103">NotSentToMe</span></span>

<span data-ttu-id="f6d6c-104">Элемент **нотсенттоме** указывает, должно ли владелец почтового ящика отсутствовать в свойстве **ToRecipients** входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="f6d6c-104">The **NotSentToMe** element indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
```xml
<NotSentToMe>true | false</NotSentToMe>
```

 <span data-ttu-id="f6d6c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f6d6c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6d6c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f6d6c-106">Attributes and elements</span></span>

<span data-ttu-id="f6d6c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f6d6c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6d6c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f6d6c-108">Attributes</span></span>

<span data-ttu-id="f6d6c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f6d6c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6d6c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f6d6c-110">Child elements</span></span>

<span data-ttu-id="f6d6c-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f6d6c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f6d6c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f6d6c-112">Parent elements</span></span>

|<span data-ttu-id="f6d6c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6d6c-113">**Element**</span></span>|<span data-ttu-id="f6d6c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6d6c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6d6c-115">Условия</span><span class="sxs-lookup"><span data-stu-id="f6d6c-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="f6d6c-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="f6d6c-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="f6d6c-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="f6d6c-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="f6d6c-118">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="f6d6c-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f6d6c-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f6d6c-119">Text value</span></span>

<span data-ttu-id="f6d6c-120">Текстовое значение **true** указывает, что владелец почтового ящика не должен находиться в свойстве **ToRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="f6d6c-120">A text value of **true** indicates that the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="f6d6c-121">Значение **false** указывает, что владелец почтового ящика должен находиться в свойстве **ToRecipients** входящего сообщения, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="f6d6c-121">A value of **false** indicates that the owner of the mailbox must be in the **ToRecipients** property of the incoming message in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f6d6c-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="f6d6c-122">Remarks</span></span>

<span data-ttu-id="f6d6c-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6d6c-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6d6c-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f6d6c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6d6c-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f6d6c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6d6c-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f6d6c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f6d6c-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f6d6c-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6d6c-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f6d6c-128">Validation File</span></span>  <br/> |<span data-ttu-id="f6d6c-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f6d6c-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6d6c-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f6d6c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6d6c-131">True</span><span class="sxs-lookup"><span data-stu-id="f6d6c-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6d6c-132">См. также</span><span class="sxs-lookup"><span data-stu-id="f6d6c-132">See also</span></span>



- [<span data-ttu-id="f6d6c-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f6d6c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

