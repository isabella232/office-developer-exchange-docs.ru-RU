---
title: сентккме
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
description: Элемент Сентккме указывает, должен ли владелец почтового ящика быть указан в свойстве CcRecipients входящих сообщений, чтобы применялось условие или исключение.
ms.openlocfilehash: 1fae56a8e7d4e56c56884e5fff051ecd9f138a6d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465480"
---
# <a name="sentccme"></a><span data-ttu-id="512a9-103">сентккме</span><span class="sxs-lookup"><span data-stu-id="512a9-103">SentCcMe</span></span>

<span data-ttu-id="512a9-104">Элемент **сентккме** указывает, должен ли владелец почтового ящика быть указан в свойстве **CcRecipients** входящих сообщений, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="512a9-104">The **SentCcMe** element indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentCcMe>true | false</SentCcMe>
```

 <span data-ttu-id="512a9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="512a9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="512a9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="512a9-106">Attributes and elements</span></span>

<span data-ttu-id="512a9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="512a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="512a9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="512a9-108">Attributes</span></span>

<span data-ttu-id="512a9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="512a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="512a9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="512a9-110">Child elements</span></span>

<span data-ttu-id="512a9-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="512a9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="512a9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="512a9-112">Parent elements</span></span>

|<span data-ttu-id="512a9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="512a9-113">**Element**</span></span>|<span data-ttu-id="512a9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="512a9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="512a9-115">Условия</span><span class="sxs-lookup"><span data-stu-id="512a9-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="512a9-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="512a9-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="512a9-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="512a9-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="512a9-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="512a9-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="512a9-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="512a9-119">Text value</span></span>

<span data-ttu-id="512a9-120">Текстовое значение **true** указывает, что владелец почтового ящика должен находиться в свойстве **CcRecipients** входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="512a9-120">A text value of **true** indicates that the owner of the mailbox must be in the **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="512a9-121">Значение **false** указывает, что владелец почтового ящика не должен находиться в свойстве **CcRecipients** входящих сообщений, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="512a9-121">A value of **false** indicates that the owner of the mailbox must not be in the **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="512a9-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="512a9-122">Remarks</span></span>

<span data-ttu-id="512a9-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="512a9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="512a9-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="512a9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="512a9-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="512a9-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="512a9-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="512a9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="512a9-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="512a9-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="512a9-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="512a9-128">Validation File</span></span>  <br/> |<span data-ttu-id="512a9-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="512a9-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="512a9-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="512a9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="512a9-131">True</span><span class="sxs-lookup"><span data-stu-id="512a9-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="512a9-132">См. также</span><span class="sxs-lookup"><span data-stu-id="512a9-132">See also</span></span>



- [<span data-ttu-id="512a9-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="512a9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

