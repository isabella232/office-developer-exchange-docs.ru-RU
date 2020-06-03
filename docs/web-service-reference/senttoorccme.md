---
title: сенттурккме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentToOrCcMe
api_type:
- schema
ms.assetid: ca43e05d-df37-485b-9276-34678025f2b7
description: Элемент Сенттурккме указывает, должен ли владелец почтового ящика быть в свойстве ToRecipients или CcRecipients входящих сообщений, чтобы применялось условие или исключение.
ms.openlocfilehash: 906e5d9fd405b9aa6f772bcedbd1869b5023a05e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462082"
---
# <a name="senttoorccme"></a><span data-ttu-id="19e93-103">сенттурккме</span><span class="sxs-lookup"><span data-stu-id="19e93-103">SentToOrCcMe</span></span>

<span data-ttu-id="19e93-104">Элемент **сенттурккме** указывает, должен ли владелец почтового ящика быть в свойстве **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="19e93-104">The **SentToOrCcMe** element indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToOrCcMe>true | false</SentToOrCcMe>
```

 <span data-ttu-id="19e93-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="19e93-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19e93-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="19e93-106">Attributes and elements</span></span>

<span data-ttu-id="19e93-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="19e93-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19e93-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="19e93-108">Attributes</span></span>

<span data-ttu-id="19e93-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="19e93-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19e93-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="19e93-110">Child elements</span></span>

<span data-ttu-id="19e93-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="19e93-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19e93-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="19e93-112">Parent elements</span></span>

|<span data-ttu-id="19e93-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="19e93-113">**Element**</span></span>|<span data-ttu-id="19e93-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="19e93-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19e93-115">Условия</span><span class="sxs-lookup"><span data-stu-id="19e93-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="19e93-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="19e93-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="19e93-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="19e93-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="19e93-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="19e93-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19e93-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="19e93-119">Text value</span></span>

<span data-ttu-id="19e93-120">Текстовое значение **true** указывает, что владелец почтового ящика должен находиться в свойстве **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="19e93-120">A text value of **true** indicates that the owner of the mailbox must be in the **ToRecipients** or **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="19e93-121">Значение **false** указывает, что владелец почтового ящика не должен находиться в свойстве **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="19e93-121">A value of **false** indicates that the owner of the mailbox must not be in the **ToRecipients** or **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="19e93-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="19e93-122">Remarks</span></span>

<span data-ttu-id="19e93-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="19e93-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19e93-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="19e93-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19e93-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="19e93-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="19e93-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="19e93-126">Schema Name</span></span>  <br/> |<span data-ttu-id="19e93-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="19e93-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="19e93-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="19e93-128">Validation File</span></span>  <br/> |<span data-ttu-id="19e93-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="19e93-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="19e93-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="19e93-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="19e93-131">True</span><span class="sxs-lookup"><span data-stu-id="19e93-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19e93-132">См. также</span><span class="sxs-lookup"><span data-stu-id="19e93-132">See also</span></span>



- [<span data-ttu-id="19e93-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="19e93-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

