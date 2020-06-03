---
title: исаутоматикфорвард
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAutomaticForward
api_type:
- schema
ms.assetid: 6876b849-a648-482e-8934-93eb5a0c465f
description: Элемент Исаутоматикфорвард указывает, должны ли входящие сообщения быть автоматически пересылаться, чтобы применялось условие или исключение.
ms.openlocfilehash: 800d38bab30245d88b3c09609e6235e6de8fed25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455578"
---
# <a name="isautomaticforward"></a><span data-ttu-id="87701-103">исаутоматикфорвард</span><span class="sxs-lookup"><span data-stu-id="87701-103">IsAutomaticForward</span></span>

<span data-ttu-id="87701-104">Элемент **исаутоматикфорвард** указывает, должны ли входящие сообщения быть автоматически пересылаться, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="87701-104">The **IsAutomaticForward** element indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span> 
  
```XML
<IsAutomaticForward/> true | false</IsAutomaticForward>
```

 <span data-ttu-id="87701-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="87701-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87701-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="87701-106">Attributes and elements</span></span>

<span data-ttu-id="87701-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="87701-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87701-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="87701-108">Attributes</span></span>

<span data-ttu-id="87701-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="87701-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87701-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="87701-110">Child elements</span></span>

<span data-ttu-id="87701-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="87701-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="87701-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="87701-112">Parent elements</span></span>

|<span data-ttu-id="87701-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="87701-113">**Element**</span></span>|<span data-ttu-id="87701-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="87701-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87701-115">Условия</span><span class="sxs-lookup"><span data-stu-id="87701-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="87701-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="87701-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="87701-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="87701-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="87701-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="87701-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="87701-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="87701-119">Text value</span></span>

<span data-ttu-id="87701-120">Текстовое значение **true** указывает, что сообщение должно быть автоматически пересылаться для того, чтобы условие или исключение применялось.</span><span class="sxs-lookup"><span data-stu-id="87701-120">A text value of **true** indicates that the message must be an automatic forward in order for the condition or exception to apply.</span></span> <span data-ttu-id="87701-121">Значение **false** указывает на то, что сообщение не должно быть автоматически пересылаться, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="87701-121">A value of **false** indicates that the message must not be an automatic forward in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="87701-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="87701-122">Remarks</span></span>

<span data-ttu-id="87701-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="87701-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87701-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="87701-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87701-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="87701-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="87701-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="87701-126">Schema Name</span></span>  <br/> |<span data-ttu-id="87701-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="87701-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="87701-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="87701-128">Validation File</span></span>  <br/> |<span data-ttu-id="87701-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="87701-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="87701-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="87701-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="87701-131">True</span><span class="sxs-lookup"><span data-stu-id="87701-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87701-132">См. также</span><span class="sxs-lookup"><span data-stu-id="87701-132">See also</span></span>



- [<span data-ttu-id="87701-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="87701-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

