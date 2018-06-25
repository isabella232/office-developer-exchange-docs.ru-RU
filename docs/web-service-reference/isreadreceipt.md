---
title: IsReadReceipt
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReadReceipt
api_type:
- schema
ms.assetid: e60e525f-c136-469a-b68b-b3dc01f400a6
description: Элемент IsReadReceipt указывает ли входящих сообщений должны быть прочтении в порядке для условие или исключение для применения.
ms.openlocfilehash: 78714aafb116a609a69d77b3b4f0fd15695bda34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834094"
---
# <a name="isreadreceipt"></a><span data-ttu-id="35660-103">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="35660-103">IsReadReceipt</span></span>

<span data-ttu-id="35660-104">Элемент **IsReadReceipt** указывает ли входящих сообщений должны быть прочтении в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="35660-104">The **IsReadReceipt** element indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span> 
  
```XML
<IsReadReceipt> true | false</IsReadReceipt>
```

 <span data-ttu-id="35660-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="35660-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35660-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="35660-106">Attributes and elements</span></span>

<span data-ttu-id="35660-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="35660-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35660-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="35660-108">Attributes</span></span>

<span data-ttu-id="35660-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="35660-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35660-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="35660-110">Child elements</span></span>

<span data-ttu-id="35660-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="35660-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="35660-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="35660-112">Parent elements</span></span>

|<span data-ttu-id="35660-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="35660-113">**Element**</span></span>|<span data-ttu-id="35660-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="35660-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35660-115">Условия</span><span class="sxs-lookup"><span data-stu-id="35660-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="35660-116">Представляет условия, если выполнены, запустит действия правил для этого правила.</span><span class="sxs-lookup"><span data-stu-id="35660-116">Represents the conditions that, when fulfilled, will trigger the rule actions for that rule.</span></span>  <br/> |
|[<span data-ttu-id="35660-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="35660-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="35660-118">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="35660-118">Represents all the available rule exception conditions for the Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="35660-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="35660-119">Text value</span></span>

<span data-ttu-id="35660-120">Текстовое значение **true,** указывает, что сообщения должны быть прочтении в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="35660-120">A text value of **true** indicates that the message must be a read receipt in order for the condition or exception to apply.</span></span> <span data-ttu-id="35660-121">Если сообщение не прочтении условие или исключение вступили в силу, значение — **false**.</span><span class="sxs-lookup"><span data-stu-id="35660-121">If the message does not have to be a read receipt for the condition or exception to apply, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="35660-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="35660-122">Remarks</span></span>

<span data-ttu-id="35660-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="35660-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35660-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="35660-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35660-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="35660-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="35660-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="35660-126">Schema Name</span></span>  <br/> |<span data-ttu-id="35660-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="35660-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="35660-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="35660-128">Validation File</span></span>  <br/> |<span data-ttu-id="35660-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="35660-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="35660-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="35660-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="35660-131">True</span><span class="sxs-lookup"><span data-stu-id="35660-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="35660-132">См. также</span><span class="sxs-lookup"><span data-stu-id="35660-132">See also</span></span>



- [<span data-ttu-id="35660-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="35660-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

